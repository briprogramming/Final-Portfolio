## Project #3 - The Wish Granting API

The Wish Granting API is a RESTful backend service that allows users to authenticate, create and manage "Wishes," assign "Fairies" to grant them, and receive humorous AI-generated ironic outcomes via Google Gemini. This collaborative project demonstrates comprehensive backend development with multiple authentication strategies, role-based access control, and AI integration.

**Contributors**: Mohammad Jamal, Juan Figueroa, Phoung Troung, Briana Daniels

- **What are the users?**  
  End users who want to create and track wishes with AI-generated humorous twists, and administrators who manage the entire system and all user data.

- **What job does it form for them?**  
  The API provides a secure backend service for wish management with dual authentication options (Google OAuth 2.0 or local username/password), JWT-based authorization, and AI-powered content generation. It handles user registration, authentication, authorization, data persistence, and integrates with Google Gemini to generate playful genie-style ironic twists for each wish.

- **What inspired you to make it?**  
  The inspiration came from wanting to build a comprehensive RESTful API that combines modern authentication strategies with creative AI integration. By implementing progressive authorization tiers and AI-generated content, we created a backend service that's both technically robust and entertaining.

- **What features are the most important?**
  - **Dual Authentication**: Google OAuth 2.0 with JWT tokens and local username/password with bcrypt hashing and salting
  - **RESTful CRUD Operations**: Complete Create, Read, Update, Delete operations for Wishes, Fairies, and Users
  - **Authorization & Ownership**: JWT middleware protecting routes, users can only access/modify their own data
  - **Role-Based Access Control**: Admin users have elevated privileges to view, edit, and delete all entities
  - **AI-Powered Content**: Google Gemini integration generates humorous ironic outcomes for wishes with playful genie prompts
  - **Data Associations**: Related data included in responses (user associations with wishes, fairy links)
  - **Comprehensive Testing**: Jest and Supertest suite with database isolation, API mocking, and error scenario coverage
  - **Security Best Practices**: Password hashing, JWT tokens, protected endpoints, helpful error messages

- **Include relevant screenshots**  
  _(Add screenshots of API responses, Postman/Thunder Client testing, authentication flow, and Gemini-generated outcomes)_

## Technologies

### Runtime & Framework
- Node.js
- Express.js (RESTful API framework)

### Authentication & Security
- Passport.js (Google OAuth 2.0 strategy)
- jsonwebtoken (JWT for authorization)
- bcrypt (password hashing and salting)

### Database & ORM
- Sequelize ORM (data modeling and migrations)
- SQLite (development and testing database)

### AI Integration
- Google Gemini API (@google/generative-ai)
- AI-generated wish outcomes with ironic twists

### Testing
- Jest (testing framework)
- Supertest (HTTP endpoint testing)
- Database isolation per test
- API mocking for consistent results

### Development Tools
- npm (package management)
- Sequential test execution for database safety

## Competencies

### JF 1.5: Can work effectively and contribute appropriately on a team to produce software
- **Situation**: As part of a four-person development team, we needed to build a comprehensive RESTful API with multiple authentication strategies, role-based access control, and AI integration while ensuring code quality and collaboration.
- **Actions**: I collaborated with Mohammad Jamal, Juan Figueroa, and Phoung Troung to divide responsibilities across authentication implementation, CRUD operations, AI integration, and testing. We established clear API contracts, implemented consistent error handling middleware, created modular route structures, and used Git for version control. We conducted code reviews and maintained documentation to ensure all team members understood the codebase.
- **Results**: Successfully delivered a fully functional API with dual authentication (Google OAuth + local), complete CRUD operations, admin role implementation, and Google Gemini integration. Our collaborative approach enabled parallel development without conflicts, and our comprehensive test suite (Jest + Supertest) achieved coverage across all endpoints and authentication flows.
- **Connection**: This project demonstrates effective team software development through clear division of responsibilities, consistent coding standards, collaborative problem-solving on authentication and authorization challenges, and shared ownership of testing and documentation.

### JF 2.6: Can implement a RESTful API
- **Situation**: The project required a complete RESTful backend implementing CRUD operations for multiple resources (Wishes, Fairies, Users) with proper HTTP methods, status codes, and resource relationships while adhering to REST principles.
- **Actions**: I designed and implemented RESTful endpoints following REST conventions: GET for reading entries, POST for creating new resources, PUT/PATCH for updates, and DELETE for removal. I structured routes logically (/wishes, /fairies, /users), implemented proper HTTP status codes (200, 201, 400, 401, 404), created associated data responses (wishes include user information), and established resource ownership patterns.
- **Results**: The API exposes comprehensive RESTful CRUD operations across all core resources with proper HTTP semantics. Endpoints are protected with JWT middleware, return appropriate status codes, include helpful error messages via error middleware, and support data associations as specified in Tier 5 requirements. The API successfully handles both authenticated and unauthenticated requests with clear responses.
- **Connection**: This project demonstrates RESTful API implementation skills through proper endpoint design, HTTP method usage, status code handling, resource relationships, authentication/authorization integration, and adherence to REST architectural principles.

### JF 3.7: Can effectively use a version control system and follow best practices
- **Situation**: Working with a distributed team on a multi-tiered API project required effective version control to manage concurrent development, track progressive feature implementation (Tiers 1-6), and maintain code quality across multiple contributors.
- **Actions**: We used Git for version control with feature branches for different tiers (authentication, CRUD, admin roles, AI integration), implemented commit messages describing tier requirements and features, conducted pull request reviews before merging, and maintained a clear project structure separating routes, models, middleware, and tests. We documented the codebase comprehensively and tracked feature-to-tier mappings.
- **Results**: Successfully managed collaborative development across four team members with minimal merge conflicts. Our tier-based approach allowed incremental feature delivery from MVP (Tier 1 CRUD) through advanced authorization (Tier 6 admin roles) and bonus features (Gemini integration, comprehensive testing). The repository history clearly tracks progression through specification requirements.
- **Connection**: This project demonstrates version control proficiency through team-based Git workflows, feature branch management, collaborative code reviews, progressive feature implementation tracking, and maintaining clean commit history that aligns with project specifications and tier requirements.

### JF 4.4: Can interpret and implement a given design while remaining compliant with security and maintainability requirements
- **Situation**: The project specification outlined a progressive tier system (Tiers 1-6) with specific security requirements including authentication, authorization, password hashing, role-based access control, and protected endpoints while maintaining code quality and error handling.
- **Actions**: I systematically implemented each tier requirement: basic CRUD (Tier 1), bcrypt password hashing and salting (Tier 2), user registration with JWT authorization (Tier 3), protected routes with ownership filtering and error middleware (Tier 4), associated data in responses (Tier 5), and admin versus user role separation (Tier 6). I integrated security best practices including JWT middleware for protected endpoints, bcrypt for password security, ownership validation ensuring users only access their own data, comprehensive error handling, and isolated test databases.
- **Results**: Successfully implemented all six tiers plus bonus features (Gemini AI, comprehensive Jest/Supertest testing with database isolation and API mocking). The API enforces security through authentication requirements, authorization checks, password hashing, role-based access control, and helpful error responses. The test suite validates all security scenarios including 400/401/404 responses and edge cases.
- **Connection**: This project demonstrates the ability to interpret specifications and implement secure, maintainable solutions through progressive tier-based development, comprehensive security implementation (authentication, authorization, encryption), role-based access patterns, error handling middleware, and extensive testing for security validation and code maintainability.