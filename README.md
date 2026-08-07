# QIWI Financial Chatbot

## Overview

QIWI is a full-stack financial chatbot developed to demonstrate the principles of conversational AI, software architecture, and full-stack web development. The application enables users to ask questions about financial products through an intuitive chat interface, while a Python backend interprets user intent and returns relevant responses.

Rather than relying on large language models, QIWI uses a custom-built, rule-based Natural Language Processing (NLP) engine to classify user intent. This approach provides transparent, explainable decision-making while showcasing the fundamentals of chatbot development and backend system design.

The project was built as a practical exercise in designing scalable software using a layered architecture, separating presentation, business logic, intent processing, and data access into independent components.

---

## Features

* Interactive React-based chat interface
* Real-time communication between frontend and backend
* Rule-based Natural Language Processing (NLP) for intent recognition
* Intent classification with support for greetings, common phrases, and financial product queries
* Automatic scrolling and typing indicator for an improved user experience
* FastAPI REST API for frontend-backend communication
* Data Access Object (DAO) architecture for database interactions
* Modular, object-oriented backend design
* Error handling and fallback responses for unknown user queries

---

## System Architecture

```
React Frontend
       │
       ▼
 FastAPI REST API
       │
       ▼
 Intent Parser
       │
       ▼
 Response Service
       │
       ▼
 ProductDAO
       │
       ▼
 PostgreSQL Database
```

The application follows a layered architecture, ensuring that each component has a single responsibility. This improves maintainability, testing, and future scalability.

---

## Technologies Used

### Frontend

* React
* JavaScript (ES6)
* HTML5
* CSS3

### Backend

* Python
* FastAPI
* Pydantic

### Database

* PostgreSQL

### Software Engineering Principles

* Object-Oriented Programming (OOP)
* Layered Architecture
* REST API Design
* Data Access Object (DAO) Pattern
* Rule-Based Natural Language Processing (NLP)

---

## Project Highlights

* Designed and implemented a modular full-stack chatbot from scratch.
* Built a custom intent parser capable of classifying user requests and routing them to the appropriate backend services.
* Implemented a clean separation between the API layer, business logic, and database access using reusable software components.
* Developed an interactive React user interface featuring message history, automatic scrolling, and a typing indicator.
* Improved intent classification by replacing substring matching with word-level tokenisation, eliminating false-positive matches (for example, preventing the word "which" from being incorrectly classified as the greeting "hi").
* Successfully integrated the React frontend with the FastAPI backend using RESTful API communication and resolved CORS-related integration challenges during development.

---

## Future Improvements

* Context-aware conversations and short-term conversation memory
* Machine learning-based intent classification
* Authentication and personalised user sessions
* Voice input and speech synthesis
* Integration with external financial APIs
* Sentiment analysis
* Deployment using Docker and cloud services

---

## Learning Outcomes

This project strengthened my understanding of full-stack software development by combining frontend engineering, backend API development, database integration, software architecture, and conversational AI principles. It also provided valuable experience in debugging distributed applications, designing maintainable systems, and improving user experience through iterative development.
