# Analyze-And-Model-Airline-System

This repository contains the documentation and code for the Data Warehouse Project. The project aims to develop a robust and scalable data warehouse to support various business processes in the airline industry. The data warehouse will facilitate efficient data storage, retrieval, and analysis, enabling better decision-making and improving operational efficiency.

## Business Processes

The data warehouse project encompasses the following key business processes:

1. **Ticket Reservation**: This process involves the reservation of tickets for passengers. It includes the booking reference, passenger journey details (departure and arrival airports, dates), payment form (credit or cash), seat number and class, fare basis, ticket promotion eligibility, flyer's program enrollment status, ticket type (refundable or not), and cancellation information.

2. **Customer Services**: This process focuses on handling passenger complaints before, during, and after their journey. It includes tracking the type and severity of complaints to enhance performance and assess agent interactions and response.

3. **Special Requests**: This process addresses special service requests made by passengers, such as wheelchair assistance at the airport. It utilizes a coding system called SSR (Special Service Request) to manage and fulfill these requests.

4. **Accommodation Support**: Some passengers require overnight accommodations during long journeys with transition times between flights. This process manages the booking of hotels, including details such as hotel name, address, rating, room specifications (suite or standard), and meal options (full-board or not).

5. **Customer Loyalty Program**: This process focuses on customer loyalty programs offered by the airline. Specifically, it tracks frequent flyer program details, including earned points, ways to accumulate points, and redemption options for rewards.

6. **Flight Activity**: This process tracks flight departures, arrivals, and associated revenue calculations. It factors in expenses incurred during the journey and calculates overall profitability.

## Data Model

The data model utilized for this project is the **Data Vault**. Several reasons influenced the choice of Data Vault as the model:

- Business focus: The Data Vault model is designed to align with business requirements and supports scalability to accommodate future changes and opportunities.
- Scalability and real-time changes: The model allows for fast and scalable data integration, making it suitable for handling near real-time data changes.
- Project management efficacy: The Data Vault methodology has proven effective in data warehousing project management, particularly when combined with agile methodologies like Scrum and CMMI.

## Table of Contents

- **Hubs**: Contains the hub tables representing the core entities in the data model.
- **Links**: Includes the link tables that connect the hub tables and capture relationships between entities.
- **Satellites**: Stores the satellite tables providing additional context and descriptive attributes for hub entities.

**Note**: Color coding is used in the table of contents for better visualization:

- Blue: Hubs
- Yellow: Links
- Green: Satellites

## Business Terminologies

To better understand the project, here are some important business terminologies:

- **SSR**: Special Service Request - A coding system that represents specific services requested by passengers.
- **PNR**: Passenger Name Record - A unique code generated for individual or group passenger bookings, containing passenger details, itinerary, ticket information, and contact information.
- **Frequent Flyer**: A loyalty program offered by the airline to frequent travelers. It involves earning points based on miles traveled, status levels (gold, platinum, titanium), and various privileges. Points can be redeemed for rewards such as shopping or award flights.

In our Data Vault Model, we have made certain assumptions about the business:

- Revenue and profit calculations are based on actual flights and total ticket sales.
- Severity levels for customer care tickets have been defined.
- Assumptions have been made regarding the acquisition of complaint time.

For more details on the project implementation, please refer to
