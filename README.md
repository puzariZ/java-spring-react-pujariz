# eCommerce Application

This repository contains a full-stack eCommerce application built using **Java Spring Boot** for the backend and **React** for the frontend. The application includes basic CRUD operations, a search functionality, and image handling to display product details on the website.

## Features

- **Product Management**: Add, edit, delete, and view products.
- **Search Functionality**: Search for products by name, category, or description.
- **Image Handling**: Upload and display product images on the website.
- **Responsive Design**: Ensures optimal user experience across devices.

---

## Technologies Used

### Backend
- Java Spring Boot
- Spring Data JPA
- Hibernate
- MySQL Database
- Maven
- REST APIs

### Frontend
- React
- React Router
- Axios (for API calls)
- Bootstrap / TailwindCSS (for UI styling)

### Additional Tools
- Postman (for API testing)
- Git (for version control)

---

## Prerequisites

- Java 11 or higher
- Node.js and npm
- MySQL database
- IDEs: IntelliJ IDEA / VS Code
- Postman (optional, for testing APIs)

---

## Getting Started

### Clone the Repository
```bash
$ git clone https://github.com/your-username/ecommerce-app.git
$ cd ecommerce-app
```

### Backend Setup

1. Navigate to the backend directory:
    ```bash
    cd backend
    ```

2. Configure the database connection in `application.properties`:
    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce_db
    spring.datasource.username=your-username
    spring.datasource.password=your-password
    ```

3. Run the application:
    ```bash
    ./mvnw spring-boot:run
    ```

### Frontend Setup

1. Navigate to the frontend directory:
    ```bash
    cd frontend
    ```

2. Install dependencies:
    ```bash
    npm install
    ```

3. Start the development server:
    ```bash
    npm start
    ```

4. Access the application at `http://localhost:3000`.

---

## API Endpoints

### Product Management
| Method | Endpoint             | Description               |
|--------|----------------------|---------------------------|
| GET    | `/api/products`      | Get all products          |
| GET    | `/api/products/{id}` | Get a product by ID       |
| POST   | `/api/products`      | Add a new product         |
| PUT    | `/api/products/{id}` | Update a product          |
| DELETE | `/api/products/{id}` | Delete a product          |

### Search Functionality
| Method | Endpoint           | Description                 |
|--------|--------------------|-----------------------------|
| GET    | `/api/products?q=` | Search products by keyword |

### Image Upload
| Method | Endpoint               | Description                 |
|--------|------------------------|-----------------------------|
| POST   | `/api/products/upload` | Upload product image        |

---

## Folder Structure

### Backend
```
backend/
├── src/main/java/com/example/ecommerce
│   ├── controller
│   ├── model
│   ├── repository
│   ├── service
│   └── EcommerceApplication.java
└── src/main/resources
    ├── application.properties
    └── static
```

### Frontend
```
frontend/
├── src/
│   ├── components/
│   ├── pages/
│   ├── services/
│   ├── App.js
│   ├── index.js
└── public/
```

---

## Screenshots

### Home Page
![Home Page](screenshots/homepage.png)

### Product Details
![Product Details](screenshots/product-details.png)

---

## Future Enhancements

- User authentication and authorization (login, signup)
- Shopping cart and checkout functionality
- Payment gateway integration
- Advanced search and filters

---

## Contribution

Contributions are welcome! Please follow the steps below:

1. Fork this repository.
2. Create a new branch (`git checkout -b feature-branch-name`).
3. Commit your changes (`git commit -m 'Add feature'`).
4. Push to the branch (`git push origin feature-branch-name`).
5. Create a pull request.

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

## Contact

For any questions or suggestions, feel free to reach out at `your-email@example.com`.
