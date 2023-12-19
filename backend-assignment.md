# Invoice Payment Collection System Backend API Task

## Project Description

The task at hand is to build a robust backend API for a payment collection system with three key components: a receiver, a payer, and an admin, as well as designing the corresponding database schema. This system is specifically designed for an invoice payment collection scenario. Imagine a system where invoices can be added, and they can be collected from someone else. Payment mode can be offline or online. Anyone can be a receiver and payer for simplicity. Keep the functionalities as simple and as open as possible. Be imaginative in terms of requirements of this system. Admin would be a person who would have super privileges to be every action in this system.

While this is a tech assignment, I would encourage you to not look at it just as an assignment to finish, but rather look at it from a product perspective. Imagine this backend to evolve and manage payment systems for a large scale of users. You might not implement it for the scale but should have a good understanding of how it can evolve into that.

## Requirements

### Technology Choices

While it is encouraged to use TypeScript and PostgreSQL with TypeORM for familiarity and efficiency, the engineer is free to choose alternative technologies if deemed more suitable for the project.

### Database Schema

Develop a well-structured database schema that supports the invoice payment collection system.
Define the tables, relationships, and data types required to store receiver, payer, and admin data, along with transaction records.
Consider scalability and data integrity.

### API Functionality

Create a set of API endpoints to manage the receiver, payer, and admin components.
Emphasize simplicity, while ensuring security and performance.
Include core operations such as creation, retrieval, updating, and deletion for each component.

### Payment Transactions

Implement secure and reliable invoice payment transactions.
Pay meticulous attention to error handling and validation for payment requests.
Allow for various payment methods (e.g., credit card, bank transfer) and maintain a record of the payment status.

### Authentication and Authorization

Create an efficient authentication and authorization system.
Restrict actions to authorized users.
Account for potential changes and adaptability.

### Bonus Points (Optional)

- **Testing and Reliability:** Develop a robust testing strategy, with a focus on automated testing. Ensure the reliability of the API even under early-stage conditions.
- **Future Features:** Explore and outline additional features that could be built on top of the system as the scale increases. Consider scalability, performance, and user experience improvements.
- **Webhooks for Online Payments:** Develop basic webhooks to efficiently handle online payments, with a focus on invoice-related events. Ensure that key events like payment success, failure, and refunds trigger real-time updates. Prioritize system stability.

## Evaluation Criteria

- Code quality, organization, and readability.
- Security, data integrity, scalability considerations, and the effectiveness of the database schema.
- Fulfillment of API requirements, including basic invoice payment functionality.
- Clarity of documentation and instructions.
- The stability and reliability of the webhook system.
- Adherence to best practices and coding standards.

## Submission

The engineer should provide a link to a public repository containing their code, along with clear setup instructions. They should also share relevant documentation, including the database schema, and testing resources to facilitate the evaluation.

**Note:** While deployment and Postman collections are encouraged, they are not mandatory for this task. The primary focus is on building a solid foundation for an invoice payment collection system with scalability and potential future enhancements in mind.
