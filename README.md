# Java-Nimap-Task

1. Spring Boot Setup:

    A . Spring Boot provides a convenient way to create stand-alone, production-grade Spring-based applications. You can start by creating a new Spring Boot project using Spring Initializr or your preferred IDE.
    B . Make sure to include the necessary dependencies for Spring Web, Spring Data JPA, and any database driver (e.g., H2, MySQL, PostgreSQL).
2. REST Controllers:

  A . Create REST controllers to handle the CRUD operations for both categories and products.
  B . Annotate your controller methods with @GetMapping, @PostMapping, @PutMapping, and @DeleteMapping to define the API endpoints.
3. Database Configuration (RDB):

  A . Configure your database connection in the application.properties or application.yml file.
  B .  Use an RDBMS (Relational Database Management System) like MySQL, PostgreSQL, or H2 (for development/testing).
4 . Annotation-Based Configuration:

  A . Spring Boot encourages annotation-based configuration over XML.
  B   .Use annotations like @Entity, @Table, @Column, and @OneToMany to define your data model and relationships.
5 . Category CRUD Operations:

6. Implement the following APIs for categories:
      GET /api/categories?page=3: Retrieve all categories (with pagination).
      POST /api/categories: Create a new category.
      GET /api/categories/{id}: Retrieve a category by ID.
      PUT /api/categories/{id}: Update a category by ID.
      DELETE /api/categories/{id}: Delete a category by ID.
7. Product CRUD Operations:

      Implement similar APIs for products:
      GET /api/products?page=2: Retrieve all products (with pagination).
      POST /api/products: Create a new product.
      GET /api/products/{id}: Retrieve a product by ID.
      PUT /api/products/{id}: Update a product by ID.
      DELETE /api/products/{id}: Delete a product by ID.
8. One-to-Many Relationship:

      Define a one-to-many relationship between categories and products.
      Annotate the appropriate fields in your entities (e.g., @OneToMany in the Category entity).
9. Server-Side Pagination:

     Implement server-side pagination by using query parameters (e.g., page, size, sort).
     In your repository, use methods like findAll(Pageable pageable) to retrieve paginated results.

Test the API Using the following way

using swagger URL in Chrome(not need Postman)
URL - http://localhost:8080/swagger-ui/index.html
![image](https://github.com/user-attachments/assets/b353068e-d6a7-4ddb-89c6-525a48e3689f)

2.USING POSTMAN IMAGE
![image](https://github.com/user-attachments/assets/de922ba2-7b94-4f9e-8653-d3e6739a394b)

3. DATABASE IMAGE
   ![image](https://github.com/user-attachments/assets/76a12408-a8b3-4605-bd51-759b961c9966)
   ![image](https://github.com/user-attachments/assets/c20098f5-9206-4fcc-b01b-dd7cf49433b2)
   ![image](https://github.com/user-attachments/assets/c1439b91-f684-4b16-836b-7331e3209cea)



 



