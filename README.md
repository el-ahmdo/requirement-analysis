# Requirement Analysis in Software Development

## Introduction

This repository contains research and documentation focused on the **requirement analysis phase** of software development. It explores how large-scale systems, like hotel booking applications (e.g., Airbnb, Booking.com, and OYO), are architected to deliver smooth user experiences. The purpose is to understand how various services—like hotel listing, searching, booking, and payments—are handled efficiently using modern software practices such as microservices, messaging queues, caching, and distributed databases.

This repository is part of the ALX software engineering program and aims to provide clear, simplified explanations of complex system designs.

## What is Requirement Analysis?

**Requirement Analysis** is a critical phase in the Software Development Life Cycle (SDLC) where developers, stakeholders, and business analysts work together to **identify, gather, analyze, and document** the functional and non-functional requirements of a software system.

This phase ensures that everyone involved has a **clear and shared understanding** of what the software should do, who will use it, how it will be used, and the conditions it must meet to be considered successful.

### 🔍 Key Activities in Requirement Analysis:

- **Requirements Gathering**: Collecting needs from stakeholders (users, clients, business teams).
- **Requirements Elicitation**: Interviewing, observing, or sending questionnaires to stakeholders to discover true needs.
- **Requirements Specification**: Documenting the requirements in a clear and structured format (e.g., SRS – Software Requirements Specification).
- **Requirements Validation**: Ensuring that the documented requirements accurately reflect what the client wants and are feasible.
- **Requirements Management**: Handling changes to requirements throughout the project lifecycle.

### 📌 Why is Requirement Analysis Important?

1. **Avoids Miscommunication**: Helps ensure all stakeholders are aligned before development begins.
2. **Improves Project Planning**: Clearly defined requirements help estimate timelines, costs, and resources more accurately.
3. **Reduces Rework and Costs**: Mistakes caught early in the requirement phase are cheaper to fix than those discovered during development or after deployment.
4. **Ensures Quality**: Well-defined requirements lead to a product that meets the users’ needs and expectations.
5. **Supports Testing**: Test cases and acceptance criteria are based on well-written requirements.

### 🌀 Role in the SDLC:

In the SDLC, requirement analysis comes right after the project initiation phase and lays the foundation for:

- System design
- Architecture planning
- Implementation
- Testing strategies
- Deployment planning


## Key Activities in Requirement Analysis

The requirement analysis phase involves several essential activities that ensure a complete and accurate understanding of what the software system should do. Below are the five key activities typically performed during this phase:

- **📝 Requirement Gathering**  
  - This involves collecting information from stakeholders such as clients, users, business managers, and technical teams.
  - The goal is to understand the needs, expectations, and constraints for the software product.
  - Techniques include interviews, questionnaires, observation, and reviewing existing systems.

- **🎯 Requirement Elicitation**  
  - Elicitation goes beyond gathering to uncover the actual needs behind what stakeholders say they want.
  - It focuses on discovering hidden or conflicting requirements through brainstorming, workshops, prototyping, and use case analysis.

- **📄 Requirement Documentation**  
  - The gathered and elicited requirements are documented clearly, often in a Software Requirements Specification (SRS) document.
  - Documentation should include functional and non-functional requirements, constraints, assumptions, and acceptance criteria.

- **📊 Requirement Analysis and Modeling**  
  - This step involves evaluating the requirements for completeness, consistency, feasibility, and clarity.
  - Modeling techniques like data flow diagrams, use case diagrams, and wireframes may be used to represent the system visually and logically.

- **✅ Requirement Validation**  
  - The documented requirements are reviewed and validated with stakeholders to ensure they accurately reflect their needs.
  - This step helps identify any errors, ambiguities, or missing requirements before the development begins.

---

Performing these activities thoroughly helps create a solid foundation for system design and development, reducing the chances of project failure and increasing the likelihood of delivering a successful product.

Without proper requirement analysis, projects risk **failure, scope creep, misalignment**, and **user dissatisfaction**.

---

In the context of this repository, understanding requirement analysis helps break down complex systems like hotel booking platforms into smaller, manageable services, ensuring a clear roadmap before development starts.


## Types of Requirements

In software development, requirements are typically categorized into two main types: **Functional Requirements** and **Non-functional Requirements**. Both are essential to building a system that works as expected and delivers a smooth user experience.

### 🔧 Functional Requirements

Functional requirements define **what the system should do** — the specific features, behaviors, and operations it must support.

For the hotel booking management project, some functional requirements include:

- **Hotel Listing Management**  
  - Hotel managers must be able to add, update, or delete hotel information such as room types, prices, and availability.

- **Search Functionality**  
  - Customers must be able to search for hotels using filters like location, price range, amenities, and availability dates.

- **Hotel Booking**  
  - Users should be able to book a selected hotel, specifying the check-in and check-out dates.

- **Payment Integration**  
  - The system should integrate with third-party payment gateways to process transactions securely.

- **View Bookings**  
  - Both hotel managers and customers should be able to view current and past booking history.

- **Notification System**  
  - The system should notify customers about successful bookings and managers about new reservations.

### ⚙️ Non-functional Requirements

Non-functional requirements define **how the system should behave**. They are not about features but about qualities like performance, security, and usability.

For the hotel booking system, examples of non-functional requirements include:

- **Performance**  
  - The system should be able to handle thousands of user requests per second during peak booking seasons.

- **Scalability**  
  - The application must scale horizontally to support growing user traffic and hotel data.

- **Availability**  
  - The system should have a 99.9% uptime guarantee to ensure uninterrupted access for users worldwide.

- **Security**  
  - Sensitive data such as payment information and user credentials must be encrypted and comply with security standards (e.g., SSL/TLS, PCI-DSS).

- **Response Time**  
  - Search and booking results should load within 2 seconds to ensure a smooth user experience.

- **Maintainability**  
  - The system architecture should be modular and follow microservice principles to simplify updates and debugging.

---

Both types of requirements work together to guide the design and development of a robust and user-friendly hotel booking application.

## Use Case Diagrams

### What is a Use Case Diagram?

A **Use Case Diagram** is a type of Unified Modeling Language (UML) diagram used in requirement analysis to visually represent how **users (actors)** interact with a **system**. It shows the system's functionality from an end-user's perspective and helps identify the major features and interactions early in the software development process.

### 💡 Benefits of Use Case Diagrams

- **Clarifies system boundaries** — shows what is inside and outside the scope.
- **Identifies key system users (actors)** and their interactions.
- **Improves communication** between developers, designers, and stakeholders.
- **Helps in writing better user stories and test cases**.
- **Simplifies requirement validation** by making it visual and easy to understand.

### 🗂️ Use Case Diagram for the Booking System

Below is a sample use case diagram for a hotel booking management system like Airbnb or Booking.com. It includes two primary actors — the **Customer** and the **Hotel Manager** — and their main interactions with the system.

📌 **Actors:**
- Customer
- Hotel Manager

📌 **Use Cases:**
- Search Hotels
- View Hotel Details
- Make a Booking
- Make Payment
- View Booking History
- Add/Edit Hotel Listing
- Update Room Availability
- View New Bookings
- Receive Notifications

### 📷 Diagram

![Use Case Diagram](alx-booking-uc.png)

## Acceptance Criteria

### 📌 What is Acceptance Criteria?

**Acceptance Criteria** are specific conditions or requirements that a software feature must meet to be considered complete and accepted by stakeholders or users. They are written from the user’s perspective and help define **“done”** in a clear, testable, and measurable way.

Acceptance Criteria are essential in **Requirement Analysis** because they:

- Ensure the feature meets business goals and user needs.
- Provide a clear agreement between developers, testers, and stakeholders.
- Reduce ambiguity by setting expectations upfront.
- Serve as a basis for writing test cases and verifying functionality.

---

### ✅ Example: Acceptance Criteria for “Checkout” Feature

Let’s consider a **Checkout** feature in a hotel booking management system. Here's what its acceptance criteria might look like:

**Feature:** _Checkout and Payment for Hotel Booking_

**Acceptance Criteria:**

1. ✅ User must be able to review their booking summary before proceeding to payment.
2. ✅ User must be able to select from at least one supported payment method (e.g., card, PayPal, or bank transfer).
3. ✅ System must validate all required payment details before submitting.
4. ✅ Upon successful payment, user must see a confirmation page with booking reference.
5. ✅ A booking confirmation email and/or SMS must be sent to the user.
6. ✅ If the payment fails, the user must see a clear error message and be allowed to retry.

---





