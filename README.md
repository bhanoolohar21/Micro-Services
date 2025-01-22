# Microservices with Node.js

## Project Description

This repository demonstrates how to build microservices using **Node.js**. It includes two separate microservices:

1. **User Service**: Manages user-related operations.
2. **Post Service**: Handles operations related to posts.

The microservices communicate with each other efficiently and leverage modern tools and libraries for secure and scalable operations.

---

## Features

- **Microservices Architecture**: Built two independent microservices for User and Post.
- **Database Integration**:
  - **MongoDB** for User Service.
  - **PostgreSQL** for Post Service.
- **ORM**: Utilized **Prisma** for seamless database interactions.
- **Authentication**: Implemented using **JWT (JSON Web Tokens)**.
- **Security**: Passwords are encrypted using **Bcrypt**.
- **Efficient Communication**: Services communicate via APIs with proper routing and error handling.
- **Dockerized Services**: Ready-to-deploy services using Docker.

---

## Technologies Used

### Backend:
- **Node.js**
- **Express.js**

### Databases:
- **MongoDB**
- **PostgreSQL**

### Libraries:
- **Prisma**
- **JWT**
- **Bcrypt**
- **Axios**

### Other Tools:
- **Docker**
- **Postman** (for API testing)

---

## How to Run

### Prerequisites:
1. Install **Node.js**.
2. Install **Docker** (optional for containerized deployment).
3. Set up MongoDB and PostgreSQL instances (local or cloud-based).

### Steps:
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Install dependencies for each service:
   ```bash
   cd user-service
   npm install

   cd ../post-service
   npm install
   ```
3. Configure environment variables:
   - Create `.env` files for both services.
   - Add database connection strings and JWT secrets.
4. Start the services:
   ```bash
   npm start
   ```
   or use Docker:
   ```bash
   docker-compose up
   ```

---

## API Endpoints

### User Service:
| Endpoint       | Method | Description            |
|----------------|--------|------------------------|
| `/users`       | GET    | Get all users          |
| `/users/signup`| POST   | Create a new user      |
| `/users/login` | POST   | Authenticate a user    |

### Post Service:
| Endpoint       | Method | Description            |
|----------------|--------|------------------------|
| `/posts`       | GET    | Get all posts          |
| `/posts/create`| POST   | Create a new post      |

---

## Future Enhancements

- Add more microservices for comments and notifications.
- Implement gRPC for communication between services.
- Use Redis for caching frequently accessed data.

---

## Contributing

Feel free to fork this repository, open an issue, or submit pull requests for improvements and features.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
