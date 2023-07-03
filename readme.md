# Desert Rose Baha’i Center (DRBI) Event Booking Website

This project involves building a static Sveltekit website for event booking at the Desert Rose Baha’i Center (DRBI). The website should allow users to book tickets for events, purchase meals, and select accommodations. The website should also provide admin and manager login for managing bookings and signups.

## Technical Stack

- **Frontend**: Sveltekit with TailwindCSS for styling
- **Backend**: Firebase for data management and cloud functions for accessing data
- **Payment Processing**: Square (with the flexibility to plug in other payment processors in the future)

## Development Instructions

### Setting up the development environment

1. Install Node.js and npm on your machine.
2. Install Sveltekit and TailwindCSS.
3. Set up a Firebase project and enable Cloud Functions.
4. Set up a Square account and get your API keys.

### Building the website

#### 1. Set up the Sveltekit project

Create a new Sveltekit project and install the necessary dependencies.

#### 2. Set up Firebase

Connect your Sveltekit project to your Firebase project. Set up the necessary cloud functions for accessing data.

#### 3. Set up Square

Integrate Square into your Sveltekit project for payment processing.

#### 4. Create the website pages

Create the following pages for your website:

- Home Page
- Event List Page
- Event Detail Page
- Booking Page
- Checkout Page
- Confirmation Page

#### 5. Implement the booking process

On the Event Detail Page, users should be able to select the number of event tickets, choose meals, and select accommodations. After booking, users should receive a receipt and a follow-up email before the event with access code instructions based on their booked room(s).

#### 6. Implement the admin and manager login

Create a secure login for admins and managers. They should be able to view and manage bookings and signups.

#### 7. Implement the event creation process

Admins should be able to create new events with the following details:

- Event name
- Event dates
- Event description
- Event hosts
- Facilities used for the event
- Available accommodations
- Meals provided each day
- Other services provided (like airport shuttles)

#### 8. Implement email notifications

When a user books a ticket for an event, an email summary of the booking should be sent to the event contacts. The email should include the user's details, the details of their booking, and the total number of signups for the event.

#### 9. Implement inventory management

The website should keep track of the inventory of available accommodations for each event. When a user books an accommodation, the inventory should be updated accordingly. If an accommodation is fully booked, it should be marked as unavailable.

## Testing

Make sure to thoroughly test your website before deployment. This includes testing the booking process, payment processing, email notifications, and admin and manager login.

## Deployment

Once you're satisfied with your website, you can deploy it to a static site hosting service of your choice.

## Maintenance

Regularly update your dependencies to keep your website secure and performant. Monitor your website's performance and fix any issues that arise.

## Diagrams

You can use tools like Mermaid to create diagrams of your website's architecture and data flow. This can be helpful for understanding how different parts of your website interact with each other.



## Non-Functional Requirements

### Performance
The website should load quickly and perform well under high traffic. Regularly monitor the website's performance and optimize as necessary.

### Security
User data should be stored securely, and all transactions should be encrypted. Regularly update your dependencies and follow best practices for web security.

### Accessibility
The website should be accessible to users with disabilities and comply with WCAG 2.1 guidelines. Use tools like aXe or Lighthouse to test your website's accessibility.

### Responsiveness
The website should be responsive and work well on a variety of devices and screen sizes. Test your website on different devices and screen sizes to ensure a good user experience.

## Diagrams

You can use tools like Mermaid to create diagrams of your website's architecture and data flow. This can be helpful for understanding how different parts of your website interact with each other.

For example, here's a basic diagram of the booking process:

```mermaid
sequenceDiagram
    User->>Website: Select event
    Website->>User: Display event details
    User->>Website: Select tickets, meals, and accommodations
    Website->>User: Display total cost
    User->>Website: Enter payment information
    Website->>Payment Processor: Process payment
    Payment Processor->>Website: Confirm payment
    Website->>User: Display receipt
    Website->>Email System: Send receipt and booking details



