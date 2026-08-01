#  ASP.NET Core Development Projects

A collection of **ASP.NET Core development projects** demonstrating web application development using **ASP.NET Core MVC**, **ASP.NET Core Web API**, and **xUnit automated testing**. These projects showcase backend development, database integration, RESTful API development, CRUD operations, and unit testing using modern .NET technologies.

---

##  About the Repository

This repository contains a collection of projects developed using the **ASP.NET Core framework**. It demonstrates different aspects of modern web and software development, including the **MVC architectural pattern**, **RESTful Web APIs**, database connectivity using **Entity Framework Core**, and automated unit testing with **xUnit.net**.

The projects are designed to demonstrate practical implementation of .NET technologies and software development practices.

---

##  Projects Included

### 1.  Help Desk Ticket Management System – ASP.NET Core MVC

A web-based Help Desk Ticket Management System designed to manage and track support requests efficiently.

**Key Features:**

* User authentication and authorization
* Create and submit support tickets
* View and manage tickets
* Ticket assignment
* Priority management
* Issue categorization
* Ticket status tracking
* Search and filtering
* Ticket history management

**Technologies:**

* ASP.NET Core MVC
* C#
* Entity Framework Core
* Microsoft SQL Server
* Razor Views
* HTML5
* CSS3
* Bootstrap

---

### 2.  ASP.NET Core Web API

A RESTful Web API project developed using **ASP.NET Core** to provide HTTP-based services for client applications.

The API demonstrates CRUD operations and follows REST principles for managing application data.

**Key Features:**

* RESTful API architecture
* GET, POST, PUT, and DELETE operations
* CRUD functionality
* Entity Framework Core integration
* SQL Server database connectivity
* JSON-based request and response
* Swagger/OpenAPI documentation
* API endpoint testing

**Example Endpoints:**

| Method   | Endpoint            | Description         |
| -------- | ------------------- | ------------------- |
| `GET`    | `/api/Example`      | Get all records     |
| `GET`    | `/api/Example/{id}` | Get record by ID    |
| `POST`   | `/api/Example`      | Create a new record |
| `PUT`    | `/api/Example/{id}` | Update a record     |
| `DELETE` | `/api/Example/{id}` | Delete a record     |

---

### 3.  xUnit Test Project

An automated unit testing project using **xUnit.net** to validate application functionality and ensure code reliability.

The test project follows the **Arrange-Act-Assert (AAA)** pattern and can be used to test ASP.NET Core MVC applications, Web APIs, services, and business logic.

**Key Features:**

* Unit testing with xUnit.net
* Automated test execution
* Arrange-Act-Assert pattern
* `[Fact]` and `[Theory]` test cases
* Parameterized testing with `[InlineData]`
* Visual Studio Test Explorer integration
* .NET CLI test execution
* CI/CD testing support

**Example Test:**

```csharp
[Fact]
public void Add_ShouldReturnCorrectResult()
{
    // Arrange
    var calculator = new Calculator();

    // Act
    var result = calculator.Add(10, 20);

    // Assert
    Assert.Equal(30, result);
}
```

---

##  Repository Architecture

```text
ASP.NET Core Projects
│
├── ASP.NET Core MVC
│   ├── Controllers
│   ├── Models
│   ├── Views
│   ├── Data
│   └── Entity Framework Core
│
├── ASP.NET Core Web API
│   ├── Controllers
│   ├── Models
│   ├── DTOs
│   ├── Services
│   └── Data
│
└── xUnit Test Project
    ├── Unit Tests
    ├── Test Fixtures
    └── Test Cases
```

---

##  Technologies Used

| Technology                | Purpose                     |
| ------------------------- | --------------------------- |
| **ASP.NET Core MVC**      | Web Application Development |
| **ASP.NET Core Web API**  | RESTful API Development     |
| **C#**                    | Programming Language        |
| **Entity Framework Core** | ORM and Database Operations |
| **Microsoft SQL Server**  | Database Management         |
| **Razor Views**           | Dynamic Web UI              |
| **HTML5**                 | Webpage Structure           |
| **CSS3**                  | Styling                     |
| **Bootstrap**             | Responsive UI               |
| **Swagger/OpenAPI**       | API Documentation           |
| **xUnit.net**             | Unit Testing                |
| **Visual Studio**         | Development Environment     |
| **.NET CLI**              | Build and Test Automation   |

---

##  Prerequisites

Before running the projects, make sure you have the following installed:

* [.NET SDK](https://dotnet.microsoft.com/download)
* [Visual Studio](https://visualstudio.microsoft.com/)
* Microsoft SQL Server
* SQL Server Management Studio (SSMS)
* Entity Framework Core CLI, if required

---

##  Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repository-name.git
```

### 2. Open the Project

Open the desired project in **Visual Studio**.

### 3. Configure the Database

Update the SQL Server connection string in the project's `appsettings.json` file.

Example:

```json
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=YOUR_SERVER;Database=YourDatabase;Trusted_Connection=True;TrustServerCertificate=True;"
  }
}
```

### 4. Apply Database Migrations

If the project uses Entity Framework Core migrations:

```bash
dotnet ef database update
```

To create a new migration:

```bash
dotnet ef migrations add InitialCreate
```

Then update the database:

```bash
dotnet ef database update
```

### 5. Run the Application

```bash
dotnet run
```

Alternatively, run the project using **Visual Studio** by pressing:

```text
F5
```

or

```text
Ctrl + F5
```

---

##  Running xUnit Tests

Navigate to the test project directory and run:

```bash
dotnet test
```

For detailed test output:

```bash
dotnet test --logger "console;verbosity=detailed"
```

---

##  API Documentation

The ASP.NET Core Web API project uses **Swagger/OpenAPI** for API documentation and testing.

Swagger provides an interactive interface to:

* View API endpoints
* Test HTTP requests
* Check request parameters
* View response formats
* Test CRUD operations

---

##  Learning Objectives

This repository demonstrates practical knowledge of:

* ASP.NET Core MVC architecture
* RESTful Web API development
* CRUD operations
* Entity Framework Core
* SQL Server database integration
* Razor Views
* Dependency Injection
* HTTP methods and status codes
* Swagger/OpenAPI
* Unit testing with xUnit
* Arrange-Act-Assert testing pattern
* Automated testing
* .NET CLI
* Software development best practices

---

##  Future Enhancements

* JWT Authentication and Authorization
* Role-Based Access Control
* Email Notifications
* Analytics and Reporting Dashboard
* Integration Testing
* Mocking using Moq
* Code Coverage
* CI/CD Pipeline Integration
* Docker Containerization
* Cloud Deployment

---

##  Author

**Rajarshi Debbarma**
B.Tech – Computer Science and Engineering
**VIT Bhopal University**

---

