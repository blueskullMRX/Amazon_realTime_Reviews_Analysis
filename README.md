Real-Time Review Analysis Platform
A comprehensive microservices-based solution for real-time sentiment analysis and review processing, featuring both static reporting and live streaming dashboards.
🏗️ Architecture Overview
This platform implements a distributed microservices architecture designed for high-throughput review processing and real-time analytics.
Technology Stack

![bigdata1](https://github.com/user-attachments/assets/45974e91-6c9b-4eda-9ca9-d7b7366c5d23)
![bigdata2](https://github.com/user-attachments/assets/6db6cd4d-b415-48c9-b5db-a5893ceb46c3)
![bigdata3](https://github.com/user-attachments/assets/bdc237aa-c3f4-4d6a-8051-5e000062f07b)

Backend Services

FastAPI - High-performance microservices for API endpoints
Apache Kafka - Distributed streaming platform for message queuing
Apache Spark Streaming - Real-time data processing engine
Spark MLlib - Machine learning library for sentiment analysis
Apache Zookeeper - Distributed coordination service

Data Storage

MongoDB - NoSQL database for flexible document storage and analytics

Frontend

React - Modern web application with real-time visualization capabilities

🚀 Features

Real-time Review Ingestion - Continuous processing of incoming reviews
Sentiment Analysis - ML-powered sentiment classification using Spark MLlib
Dual Dashboard System

Static dashboard for historical analytics
Real-time streaming dashboard for live insights


Scalable Architecture - Microservices design supporting horizontal scaling
Event-driven Processing - Kafka-based messaging for seamless data flow

📊 Data Flow

Ingestion → Reviews are received via FastAPI endpoints
Streaming → Kafka queues messages for processing
Processing → Spark Streaming analyzes sentiment using MLlib models
Storage → Processed data is stored in MongoDB
Visualization → React dashboards display real-time and historical insights

🐳 Containerized Architecture
All services run in separate Docker containers, providing complete isolation, scalability, and easy deployment.
Container Services

Zookeeper Container - Distributed coordination service
Kafka Container - Message streaming platform
MongoDB Container - NoSQL database
Spark Master Container - Spark cluster coordinator
Spark Worker Container(s) - Distributed computing nodes
Backend Container - Backend API microservices
Frontend Container - Frontend dashboard application
