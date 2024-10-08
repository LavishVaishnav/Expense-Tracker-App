# Expense Tracker App

## Status: Ongoing Project

This project is currently under development. The current focus is on implementing the **AuthService** with **JWT (JSON Web Token)** for authentication and **Refresh Token** functionality to ensure secure and efficient user login sessions.

**NOTE: Updating Repo Daily with the Current Status.**

## Overview
The **Expense Tracker App** helps users manage their personal finances by allowing them to log expenses, track categorized spending, and generate reports. It also offers future scope for automatic expense tracking via SMS parsing and notification features through WhatsApp and SMS.

## Functional Requirements
- **User Authentication**: Users can log in and sign up to the application.
- **Manual Expense Management**: Users can add or remove expenses manually.
- **Expense Overview**: Users can view categorized expenses.
- **Reports and Statistics**: Users can generate weekly, monthly, and yearly reports showing statistics about their spending.

## Non-Functional Requirements
- **Fault Tolerant and Scalable**: The system is designed to be fault-tolerant and scalable, ensuring a latency of less than 100ms.
- **Config-Driven**: The system should support a configuration-driven approach to minimize code changes in the future.

## Future Scope
- **Financial Behavior Tracking**: Users can track their financial behavior and receive tips for improvement.
- **Automated Expense Tracking**: The app will be able to automatically add expenses by reading and parsing SMS messages if the user grants the necessary permissions.
- **Notifications**: The app will send notifications via WhatsApp and SMS regarding overspending, financial risks, and other indicators.

## System Architecture
The system is built on microservices architecture with the following components:

- **Client**: The user interface through which users interact with the app.
- **API Gateway**: Manages all client requests and handles tokenization for security.
- **Auth Service**: Responsible for user authentication and authorization.
- **Notification Service**: Sends notifications to users via various channels.
- **Templatisation Service**: Manages notification templates for sending customized messages.
- **User Service**: Handles all user-related information and operations.
- **Billing Service**: Manages user billing and payments.
- **Ledger Service**: Records and maintains all transaction data for users.
- **Reporting Service**: Generates reports based on user data, providing insights into spending behavior.

### System Diagram
![System Architecture](https://github.com/LavishVaishnav/-Expense_Tracker/blob/main/HLD.png)

## Tools and Technologies Used

- **Redis**: In-memory data structure store, used for caching.
- **RabbitMQ**: Message broker for asynchronous communication between microservices.
- **Docker**: Containerization for easy deployment across environments.
- **Kafka**: Distributed streaming platform for handling real-time data pipelines.
- **Kubernetes**: Orchestrates and manages containerized applications, enabling scaling.
- **Kong**: An API gateway for managing and monitoring API traffic.

## Installation and Setup

1. Clone the repository:
   ```bash
   https://github.com/LavishVaishnav/Expense-Tracker-App
   cd expense-tracker-app
Here’s the text you wanted to copy:

---

### Set up Docker:

2. Ensure Docker and Docker Compose are installed.
3. Run the services with:

```bash
docker-compose up --build
```

### Run the application:

- The application runs on `http://localhost:8080` (or as defined in your configuration).
- Set up your environment variables for the required services (e.g., Redis, RabbitMQ, etc.).

---

### Future Enhancements:
- Adding support for multi-currency tracking.
- Integrating machine learning to predict user expenses.
- Providing more advanced financial insights and suggestions.

---

### Contact:
For any inquiries or issues, feel free to open an issue on GitHub or contact us directly at `vaishnavlavish27@gmail.com`.


