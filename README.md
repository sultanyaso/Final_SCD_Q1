# Healthcare Appointment System - Backend Microservices

This project is a cloud-ready backend system for managing doctor appointments. It is built using a microservices architecture and provides a unified API interface via an API Gateway.  

Each microservice is independent, can run locally or in containers, and communicates securely with other services.

---

##  Microservices Overview

1. API Gateway
   - Single entry point for all client requests
   - Routes requests to the correct backend service
   - Hides internal service details from clients

2. Authentication Service (auth-service)
   - Handles user registration and login
   - Generates and validates JWT tokens
   - Secures communication between services and ensures only authenticated users can access protected resources

3. Patient Service (patient-service)
   - Manages patient information
   - Provides APIs to create new patient records and fetch existing patient data

4. Doctor Service (doctor-service)
   - Maintains doctor profiles and availability status
   - Enables the system to check doctor availability

5. Appointment Service (appointment-service)**
   - Manages appointment scheduling between patients and doctors

6. Notification Service (notification-service)
   - Sends notifications to patients and doctors (e.g., appointment reminders)



