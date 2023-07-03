# 🏜️ events.drbi.org

This project involves enhancing the existing SvelteKit website for event booking at the Desert Rose Baha’i Center (DRBI). The website should allow users to book tickets for events, purchase meals, and select accommodations. The website should also provide admin and manager login for managing bookings and signups.

## 🚀 Getting Started

Clone the existing repository:

```bash
git clone https://github.com/chadananda/events.drbi.org.git
cd events.drbi.org
```

Install the project dependencies:

```bash
npm install
```

## 🛠️ Development Instructions

### 🔥 Firebase Setup

Connect your Sveltekit project to your Firebase project. Set up the necessary cloud functions for accessing data. You'll need to create a new Firebase project and enable Cloud Functions.

### 💳 Square Setup

Integrate Square into your Sveltekit project for payment processing. You'll need to create a Square account and get your API keys.

### 🏗️ Building the website

#### 1. 🔐 Admin and Manager Login

Create a secure login for admins and managers. They should be able to view and manage bookings and signups.

#### 2. 📅 Event Creation

Admins should be able to create new events with the following details:

- Event name
- Event dates
- Event description
- Event hosts
- Facilities used for the event
- Available accommodations
- Meals provided each day
- Other services provided (like airport shuttles)

#### 3. 📜 Event Display

The website should display all the details of the event in a clear and organized manner. Users should be able to see the event name, dates, description, hosts, facilities, available accommodations, meals, and other services.

#### 4. 🎟️ Booking Process

On the Event Detail Page, users should be able to select the number of event tickets, choose meals, and select accommodations. After booking, users should receive a receipt and a follow-up email before the event with access code instructions based on their booked room(s).

#### 5. 📧 Email Notifications

When a user books a ticket for an event, an email summary of the booking should be sent to the event contacts. The email should include the user's details, the details of their booking, and the total number of signups for the event.

#### 6. 📦 Inventory Management

The website should keep track of the inventory of available accommodations for each event. When a user books an accommodation, the inventory should be updated accordingly. If an accommodation is fully booked, it should be marked as unavailable.

## 🧪 Testing

Make sure to thoroughly test your website before deployment. This includes testing the booking process, payment processing, email notifications, and admin and manager login.

## 🚀 Deployment

Once you're satisfied with your website, you can deploy it to a static site hosting service of your choice.

## 🛠️ Maintenance

Regularly update your dependencies to keep your website secure and performant. Monitor your website's performance and fix any issues that arise.

## 📋 Non-Functional Requirements

### 🚀 Performance

The website should load quickly and perform well under high traffic. Regularly monitor the website's performance and optimize as necessary.

### 🔒 Security

User data should be stored securely, and all transactions should be encrypted. Regularly update your dependencies and follow best practices for web security.

### 🦻 Accessibility

The website should be accessible to users with disabilities and comply with WCAG 2.1 guidelines. Use tools like aXeor Lighthouse to test your website's accessibility.

### 📱 Responsiveness

The website should be responsive and work well on a variety of devices and screen sizes. Test your website on different devices and screen sizes to ensure a good user experience.

================================================================

## 🛠️ Implementation

## 🌳 Feature Branches

### 1. `feature/admin-login`

**Tasks:**
- Set up authentication using Firebase.
- Create login page.
- Implement role-based access control.

**Test:**
- Test successful login.
- Test unsuccessful login with incorrect credentials.
- Test role-based access control.

**Merge:**
Once the feature is implemented and all tests pass, merge `feature/admin-login` into `main`.

### 2. `feature/event-creation`

**Tasks:**
- Create event creation form.
- Implement Firebase cloud function to save event data.

**Test:**
- Test form submission with valid data.
- Test form submission with invalid data.
- Test Firebase cloud function.

**Merge:**
Once the feature is implemented and all tests pass, merge `feature/event-creation` into `main`.

### 3. `feature/event-display`

**Tasks:**
- Fetch event data from Firebase.
- Display event data on event detail page.

**Test:**
- Test fetching of event data.
- Test display of event data.

**Merge:**
Once the feature is implemented and all tests pass, merge `feature/event-display` into `main`.

### 4. `feature/booking-process`

**Tasks:**
- Create booking form.
- Implement Firebase cloud function to save booking data.
- Integrate Square for payment processing.

**Test:**
- Test form submission with valid data.
- Test form submission with invalid data.
- Test Firebase cloud function.
- Test payment processing.

**Merge:**
Once the feature is implemented and all tests pass, merge `feature/booking-process` into `main`.

### 5. `feature/email-notifications`

**Tasks:**
- Implement Firebase cloud function to send email notifications.

**Test:**
- Test sending of email notifications.

**Merge:**
Once the feature is implemented and all tests pass, merge `feature/email-notifications` into `main`.

### 6. `feature/inventory-management`

**Tasks:**
- Update inventory when a booking is made.
- Display available accommodations on event detail page.

**Test:**
- Test updating of inventory.
- Test display of available accommodations.

**Merge:**
Once the feature is implemented and all tests pass, merge `feature/inventory-management` into `main`.
