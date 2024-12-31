# Product-Management-System
A Spring Boot application that provides a RESTful API for managing products. This application allows users to create, read, update, and delete product records and uses Hibernate for database operations with MySQL.
<hr>
<h3>Features</h3>
<ul>
  <li>Add new products with details such as name, category, and price.</li>
  <li>Update existing product details by ID.</li>
  <li>Delete a product from the database by ID.</li>
  <li>Retrieve all products or fetch details of a specific product by ID.</li>
  <li>Comprehensive exception handling for better user experience.</li>
  <li>Configurable database integration using Hibernate and JPA.</li>
</ul>
<hr>
<h3>Technologies Used</h3>
<ul>
  <li>Spring Boot (Framework)</li>
  <li>Hibernate (ORM tool)</li>
  <li>MySQL (Database)</li>
  <li>JPA (Java Persistence API)</li>
  <li>Postman (API Testing)</li>
</ul>
<hr>
<h3>Prerequisites</h3>
Before running this application, ensure you have:
<ul>
  <li>Java Development Kit (JDK 17 or later)</li>
  <li>MySQL Server</li>
  <li>Spring Tool Suite (STS) or any IDE with Maven support</li>
  <li>Postman (optional, for API testing)</li>
</ul>
<hr>
<h3>Installation and Setup</h3>
<ol>
  <li>
    <h4>Clone the Repositriy</h4></li>
    <pre>git clone https://github.com/yourusername/product-management.git
    cd product-management</pre>
  <li>
    <h4>Set Up the MySQL Database</h4>
    <ul>
      <li>Open your MySQL client and create a database:</li>
          CREATE DATABASE product_management;
      <li>Update the application.yml file with your MySQL credentials.</li>
    </ul>
  </li>
  <li>
    <h4>Build and Run the Application</h4>
     <ul>
      <li>Use the following Maven command:</li>
          mvn spring-boot:run
      <li>Alternatively, run the application from your IDE.</li>
    </ul>
  </li>
    <li>
    <h4>Access the API</h4>
     <ul>
      <li>Open Postman or your preferred API testing tool.</li>
      <li>Use the endpoints listed in the API Endpoints section.</li>
    </ul>
  </li>
</ol>
<hr>
<h3>Configuration</h3>
<p>
  The database connection details are configured in the     src/main/resources/application.yml file:
</p>
<pre>
server:
  port: 8081
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/product_management
    username: root
    password: yourpassword
    driver-class-name: com.mysql.cj.jdbc.Driver
  jpa:
    hibernate:
      ddl-auto: update
    show-sql: true
    </pre>


