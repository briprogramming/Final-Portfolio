## Project #5 - Inventory App

A full-stack RESTful CRUD application designed for e-commerce inventory tracking. This comprehensive application enables users to manage item inventory with complete create, read, update, and delete operations, featuring a user-friendly interface, shopping cart functionality, and responsive mobile design.

- **What are the users?**  
  E-commerce inventory managers, warehouse staff, and administrators who need to track, manage, and update product inventory in real-time.

- **What job does it form for them?**  
  The Inventory App serves as a complete inventory management system that allows users to view all items, inspect individual item details, add new products, edit existing inventory, remove items, search through inventory data, and simulate purchase workflows with shopping cart functionality. It provides a comprehensive solution for tracking items with details including name, description, price, category, and images.

- **What inspired you to make it?**  
  The project was inspired by real-world e-commerce inventory challenges where teams need to rebuild legacy systems with modern technology stacks. The goal was to create a full-stack application that demonstrates RESTful architecture, database management, and user-friendly interfaces while addressing practical inventory tracking needs.

- **What features are the most important?**
  - **Complete CRUD Operations**: Full Create, Read, Update, Delete functionality for inventory items
  - **View All Items**: Dynamic front-end display showing entire inventory in real-time
  - **Individual Item Details**: Detailed view for each item with comprehensive information
  - **Add New Items**: User-friendly form to add products to the inventory database
  - **Edit Items**: Update existing item details through an intuitive edit form
  - **Delete Items**: Remove items from inventory with delete functionality
  - **Search Functionality**: Search through inventory based on custom criteria
  - **Shopping Cart**: Add items to cart and simulate purchase workflow
  - **User & Order Management**: Additional models and routes for users and order tracking
  - **Mobile Responsive**: Fully functional on mobile browsers for on-the-go inventory management
  - **RESTful API**: Express routes following REST conventions (GET, POST, PUT, DELETE)

- **Include relevant screenshots**  
  _(Add screenshots of the inventory list view, individual item details, add/edit forms, shopping cart, and mobile view)_

## Technologies

### Backend
- Node.js (runtime environment)
- Express.js (RESTful API framework)
- Sequelize ORM (database modeling and operations)
- Sequelize CLI (migrations and model generation)

### Database
- SQL database (managed through Sequelize)
- Sequelize models for Items, Users, and Orders

### Frontend
- HTML/CSS/JavaScript
- Dynamic front-end rendering
- Responsive design for mobile compatibility
- Interactive forms and UI elements

### Testing
- Jest (testing framework)
- Unit and integration tests

### Development Tools
- npm (package management)
- Node.js
- RESTful API design patterns

### Key Features
- RESTful CRUD endpoints
- Form-based data entry
- Real-time inventory updates
- Search and filter capabilities
- Shopping cart simulation
- Mobile-responsive design

## Competencies

### JF 2.2: Can create simple data models to effectively communicate understanding of data structures
- **Situation**: The inventory application required designing a comprehensive data structure to represent items, users, and orders with proper relationships and fields that would support all CRUD operations and business logic.
- **Actions**: I designed Sequelize models for the core entities: Item model with fields for Name, Description, Price, Category, and Image to capture complete product information; User model to track customer accounts and authentication; Order model to manage purchase transactions and link users to items. I established proper data types, validations, and relationships between models to ensure data integrity. The models were structured to support efficient queries and updates while maintaining clear separation of concerns.
- **Results**: Successfully created a well-structured database schema that supports all application features including inventory management, user accounts, and order processing. The Sequelize models provide clean abstractions for database operations, making it easy to add, update, retrieve, and delete records. The data structure efficiently handles relationships between users, items, and orders while maintaining data integrity through proper constraints and validations.
- **Connection**: This project demonstrates database modeling skills through creation of comprehensive Sequelize models, proper field definitions and data types, relationship mapping between entities, and implementation of a schema that supports complex business logic and CRUD operations.

### JF 2.6: Can implement a RESTful API
- **Situation**: The project required a complete RESTful backend API to handle all inventory operations, following REST conventions and HTTP standards for a full CRUD application accessible from the front-end.
- **Actions**: I implemented RESTful Express routes following standard conventions: GET routes to retrieve all items and individual item details, POST route to add new items from form submissions, PUT route to update existing item information, and DELETE route to remove items from inventory. I ensured proper HTTP methods, status codes, and response formats. Additionally, I created routes for Users and Orders to support the complete e-commerce workflow. All routes follow RESTful principles with clear endpoint structures and appropriate error handling.
- **Results**: Delivered a fully functional RESTful API that powers all inventory operations. The API successfully handles form submissions, data retrieval, updates, and deletions with proper HTTP semantics. The front-end seamlessly integrates with backend routes through fetch requests, and all CRUD operations work reliably. The API design allows for easy extension and testing of individual endpoints.
- **Connection**: This project demonstrates RESTful API implementation skills through proper HTTP method usage (GET, POST, PUT, DELETE), adherence to REST architectural principles, clear endpoint design, integration between front-end forms and backend routes, and comprehensive coverage of CRUD operations.

### JF 3.7: Can effectively use a version control system and follow best practices
- **Situation**: Building a full-stack application with multiple features (items, users, orders, search, cart) required careful version control to track incremental development from basic CRUD to bonus features while maintaining code quality.
- **Actions**: I used Git for version control with a structured development approach: implementing core features first (Sequelize models, basic CRUD routes), then adding bonus functionality incrementally (user/order models, search, cart, mobile responsiveness). I maintained a clear commit history tracking the progression from minimum viable product to enhanced features. I documented features clearly in the repository and organized code with proper separation between models, routes, and front-end components.
- **Results**: Successfully managed the development lifecycle from basic inventory CRUD to a feature-rich e-commerce application with users, orders, search, and cart functionality. The version control history clearly shows the evolution of the project, making it easy to understand how features were built and integrated. The organized repository structure allows for easy navigation and future enhancements.
- **Connection**: This project demonstrates version control proficiency through systematic Git usage for feature development, incremental implementation tracking from core to bonus features, clear commit history documenting project evolution, and organized repository structure that supports maintainability and collaboration.

### JF 4.3: Is able to build, manage and deploy code into the relevant environment
- **Situation**: The inventory application needed to be built as a full-stack application with proper setup procedures, dependency management, database configuration, and deployment-ready structure that other developers could clone and run.
- **Actions**: I established a complete development environment setup with Node.js and npm for package management, configured Sequelize CLI for database migrations and model generation, integrated Jest for testing the application, created clear prerequisites and setup documentation, and structured the application for easy deployment. I ensured all dependencies were properly managed through package.json and that the application could be easily installed and run following standard npm workflows.
- **Results**: Created a fully deployable application with clear setup instructions and proper dependency management. The project can be easily cloned and run by other developers following the documented prerequisites (Node.js, npm, Sequelize CLI, Jest). All components (front-end, back-end, database) integrate seamlessly, and the application is ready for deployment to production environments. The testing infrastructure ensures code quality and reliability.
- **Connection**: This project demonstrates build and deployment skills through proper environment configuration, dependency management with npm, database setup with Sequelize CLI, testing integration with Jest, and creation of a deployment-ready application structure with clear documentation for setup and installation.
