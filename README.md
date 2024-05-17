# Smart India Hackathon Workshop
# Date:16-05-2024
## Register Number:212223040137
## Name:NIVETHA.S
## Problem Title
E-Waste Facility Locator
## Problem Description
Website that tells you the location of the nearest e-waste collection and recycling facility. Offers educational pop-ups on the harmful components of your e-waste and their effects on the environment and human health if not disposed correctly. There could be an option to input the model of your old device and earn credit points relative to the amount of precious metals recovered from the device if disposed correctly.
## Problem Creater's Organization
Ministry of Environment

## Idea

![alt text](<IMG 1.jpeg>)

Objective:
To develop an online platform and mobile application that helps users locate nearby e-waste disposal facilities.

Key Features:

Interactive map showing e-waste disposal facilities
Search function by location (ZIP code, city, etc.)
Detailed information on each facility (address, contact info, accepted items, hours of operation)
User reviews and ratings for facilities
Educational resources on e-waste recycling
2. Research and Data Collection
Identify Data Sources:

Government environmental agencies (EPA in the US, etc.)
Local municipalities
Recycling companies and e-waste handlers
Environmental NGOs and non-profits
Data Points to Collect:

Facility addresses
Contact details
Types of e-waste accepted
Operational hours
Special instructions or services (e.g., pickup services)
3. Platform Development
Technology Stack:

Frontend: React or Angular for the web application; React Native or Flutter for the mobile application.
Backend: Node.js with Express or Django; use RESTful APIs to connect the frontend with the backend.
Database: MongoDB or PostgreSQL to store facility data.
Mapping: Google Maps API or OpenStreetMap for the interactive map.
User Interface Design:

Simple and intuitive interface
Search bar at the top for easy location input
Map as the main visual component
Sidebar or pop-up details for facility information
Filters to refine search results (e.g., type of e-waste)
4. Features and Functionality
Core Features:

Search and Locate: Users can search for facilities by entering their location.
Map Integration: Interactive map with pins marking e-waste facilities.
Facility Details: Clicking on a pin shows details such as address, contact, accepted items, etc.
Filters: Options to filter results by type of e-waste, distance, ratings, etc.
User Reviews: Users can leave reviews and ratings for facilities based on their experiences.

## Proposed Solution / Architecture Diagram

![alt text](<IMG 2.png>)

Frontend (Web & Mobile App):

Frameworks: React for web, React Native for mobile.
Features:
Search bar for location input.
Interactive map displaying e-waste facilities.
Facility details with contact info, accepted items, and hours.
Filters for refining search results.
User reviews and ratings.
Educational content section.
Backend Services (API Layer):

Frameworks: Node.js with Express or Django.
Features:
RESTful APIs for handling frontend requests.
Endpoints for fetching facility data, handling user reviews, and managing user accounts.
Integration with external APIs for mapping and notifications.
Database:

Options: MongoDB (NoSQL) or PostgreSQL (SQL).
Data Stored:
Facility information (address, contact details, items accepted).
User accounts and authentication details.
Reviews and ratings.
Educational resources.
Mapping Services:

Provider: Google Maps API or OpenStreetMap.
Features:
Displaying facilities on an interactive map.
Geocoding for converting addresses into geographic coordinates.
Directions and distance calculation.
Notifications System:

Channels: Email, SMS, Push notifications.
Providers: Twilio (SMS), Firebase Cloud Messaging (Push).
Features:
Alerts for upcoming e-waste collection events.
Reminders for users about e-waste pickup requests.
Authentication:

Methods: OAuth for social logins (Google, Facebook), JWT for session management.
Features:
Secure user login and registration.
Token-based authentication for API access.
User Reviews and Rating System:

Features:
Allow users to submit reviews and ratings for facilities.
Moderation tools for managing inappropriate content.
Display average ratings and recent reviews for each facility.
Educational Resources:

Content Management System (CMS): WordPress or a custom-built solution.
Features:
Articles, videos, and guides on e-waste recycling.
FAQs and tips for reducing e-waste.
Searchable database of educational materials.

## Use Cases

![alt text](<IMG 3.jpeg>)

Flow:
User enters their location (ZIP code, city, or uses GPS).
System displays a map with nearby e-waste facilities marked.
User clicks on a facility pin to view details.
User reviews facility details (address, contact info, accepted items).
User navigates to the facility using provided directions.
1.2 Submit a Review for a Facility

Actors: Registered User
Preconditions: User has visited an e-waste facility.
Postconditions: Review is submitted and visible to other users.
Flow:
User logs into their account.
User selects the facility they visited from the map or search results.
User clicks on "Submit Review."
User rates the facility and writes a review.
User submits the review.
System stores the review and displays it on the facility's detail page.
1.3 Request E-Waste Pickup Service

Actors: Registered User
Preconditions: User logs into their account.
Postconditions: Pickup request is submitted and confirmed.
Flow:
User logs into their account.
User navigates to the "Request Pickup" section.
User enters details about the e-waste items and pickup location.
User selects a preferred pickup date and time.
User submits the pickup request.
System confirms the request and notifies the user of the scheduled pickup.
1.4 Receive Notifications about Collection Drives

Actors: Registered User
Preconditions: User opts in for notifications.
Postconditions: User receives notifications about upcoming e-waste collection events.
Flow:
User logs into their account.
User opts in for event notifications in their profile settings.
System sends notifications about upcoming collection drives via email or SMS.
User receives and views the notification.
User can navigate to the event details and plan to attend.
1.5 Access Educational Resources

Actors: General User
Preconditions: User accesses the platform.
Postconditions: User learns about e-waste recycling and best practices.
Flow:
User navigates to the "Educational Resources" section.
User browses through articles, videos, and guides.
User selects and reads an article or watches a video.
User applies learned knowledge to e-waste recycling practices.
2. Administrator Use Cases
2.1 Add New E-Waste Facility

Actors: Administrator
Preconditions: Administrator logs into the admin dashboard.
Postconditions: New facility is added to the database and visible to users.
Flow:
Administrator logs into the admin dashboard.
Administrator navigates to the "Add Facility" section.
Administrator enters facility details (name, address, contact info, items accepted, hours).
Administrator submits the new facility information.
System stores the facility details and updates the map.
2.2 Update Facility Information

Actors: Administrator
Preconditions: Administrator logs into the admin dashboard.
Postconditions: Facility information is updated and visible to users.
Flow:
Administrator logs into the admin dashboard.
Administrator selects a facility to update from the list.
Administrator edits the necessary information (address, contact info, accepted items).
Administrator saves the changes.
System updates the facility details in the database and on the map.
2.3 Moderate User Reviews

Actors: Administrator
Preconditions: Administrator logs into the admin dashboard.
Postconditions: Inappropriate reviews are removed, and appropriate reviews are displayed.
Flow:
Administrator logs into the admin dashboard.
Administrator navigates to the "Moderate Reviews" section.
Administrator reviews flagged or recent reviews.
Administrator decides to approve, edit, or delete reviews.
System updates the review status based on administrator action.


## Technology Stack

![alt text](<downloaIMG 4.jpeg>)

1. Frontend (Web & Mobile)
Web Application:

Framework: React
Reason: React is highly flexible, efficient, and has a strong community support. It enables fast rendering and a seamless user experience with its component-based architecture.
Styling: Tailwind CSS or Material-UI
Reason: Tailwind CSS offers utility-first CSS for rapid UI development. Material-UI provides pre-designed components adhering to Google’s Material Design principles.
Mobile Application:

Framework: React Native
Reason: React Native allows for code reuse between iOS and Android platforms, accelerating development and ensuring a consistent user experience across devices.
State Management:

Library: Redux or Context API
Reason: Redux provides a predictable state container for managing application state, which is particularly useful for large applications. Context API can be used for simpler state management needs.
Routing:

Library: React Router
Reason: React Router is a powerful and flexible routing library for React applications, allowing for dynamic routing and nested routes.
Forms and Validation:

Library: Formik with Yup
Reason: Formik simplifies form handling in React, and Yup provides schema-based validation, ensuring robust form validation.
2. Backend (API Layer)
Framework:

Option 1: Node.js with Express
Reason: Node.js is non-blocking and event-driven, making it ideal for handling multiple requests simultaneously. Express is a minimal and flexible Node.js web application framework.
Option 2: Django
Reason: Django is a high-level Python framework that encourages rapid development and clean, pragmatic design. It includes built-in features for security, ORM, and admin interface.
Authentication:

Library: JWT (JSON Web Tokens) with Passport.js (for Node.js) or Django Rest Framework JWT (for Django)
Reason: JWT provides a stateless and scalable way to handle authentication across different clients (web and mobile).
Data Fetching:

Library: Axios
Reason: Axios is a promise-based HTTP client that is simple to use for making asynchronous requests to the backend APIs.
3. Database
Options:

NoSQL: MongoDB
Reason: MongoDB is highly scalable and handles unstructured data well, which is beneficial for storing diverse facility information and user reviews.
SQL: PostgreSQL
Reason: PostgreSQL is a powerful, open-source relational database system known for its robustness, scalability, and compliance with ACID principles.
4. Mapping Services
Provider:

Option 1: Google Maps API
Reason: Google Maps API provides comprehensive mapping services, including geocoding, directions, and places API, ensuring a rich user experience.
Option 2: OpenStreetMap with Leaflet.js
Reason: OpenStreetMap is an open-source alternative to Google Maps, and Leaflet.js is a lightweight JavaScript library for interactive maps.
5. Notifications System
Providers:

Email: SendGrid or Amazon SES
Reason: Both provide reliable and scalable email sending capabilities.
SMS: Twilio
Reason: Twilio offers a robust API for sending SMS globally.
Push Notifications: Firebase Cloud Messaging (FCM)
Reason: FCM provides a reliable and cross-platform solution for sending push notifications to mobile devices.
6. Educational Content Management
CMS:

Option 1: WordPress with REST API
Reason: WordPress is a widely-used CMS with extensive plugin support and a REST API for integrating with other systems.
Option 2: Strapi
Reason: Strapi is a headless CMS that is highly customizable and integrates seamlessly with various frontend frameworks.
7. Cloud Hosting and DevOps
Cloud Providers:

Option 1: Amazon Web Services (AWS)
Reason: AWS offers a wide range of services, including EC2 for compute, S3 for storage, and RDS for managed databases.
Option 2: Google Cloud Platform (GCP)
Reason: GCP provides scalable infrastructure and services like App Engine, Cloud Storage, and BigQuery.
Containerization and Orchestration:

Containerization: Docker
Reason: Docker enables consistent development and deployment environments through containerization.
Orchestration: Kubernetes
Reason: Kubernetes provides powerful orchestration for managing containerized applications at scale.


## Dependencies

Mapping Services – 20 Days,Data Collection – 18 Days,Estimated Budget – Rs.45,0000

