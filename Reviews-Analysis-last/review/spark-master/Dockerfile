FROM bitnami/spark:3.1.3

# Install pip and required packages
USER root
#RUN apt-get update && apt-get install -y python3-pip

# Copy your requirements file
COPY requirements.txt /opt/bitnami/spark/requirements.txt
COPY test.py /review/test.py
COPY train.py /review/train.py
COPY Data.json /review/Data.json


# Install Python dependencies
RUN pip install --no-cache-dir -r /opt/bitnami/spark/requirements.txt
RUN pip install nltk && \
    python -m nltk.downloader -d /usr/share/nltk_data stopwords punkt wordnet punkt_tab
ENV NLTK_DATA=/usr/share/nltk_data

USER root
