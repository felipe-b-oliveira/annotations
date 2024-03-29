## General Annotations

### Architecture

* **BFF**: The Backend for Frontend it's a pattern thar brings a proposal when we have one backend for each user experience that we can have (web, mobile, TV, etc), on the contrary to having just one generical backend api to attend every client. This patterns remembers me of the GraphQL proposal of making easier to work with multiple frontend clients at the same time but in the BFF we separate one backend for each use. Ref: https://aws.amazon.com/blogs/mobile/backends-for-frontends-pattern/#:~:text=According%20to%20Sam%20Newman%2C%20the,one%20general%2Dpurpose%20API%20backend.

* **Serveless Web Application**: In this type of architecture the infrastructure management is made through a plataform. Example: Firebase. Ref: https://aws.amazon.com/serverless/build-a-web-app/#:~:text=Serverless%20Web%20Application&text=Serverless%20computing%20allows%20you%20to,management%20is%20done%20by%20AWS.

* **Data-Driven Development**: When the modeling starts thinking about the database (representing the database tables). This approach don't takes the benefits of Object Orientation.

* **Domain-Driven Development**: Have a idea of using a purer Object-Orientation modelling. This approach have less focus on how the data are persisted and instead looks to representing the business needs in a more clearly way through classes and benhaviors (methods). Ref(Portuguese): https://pt.stackoverflow.com/questions/19548/o-que-realmente-%C3%A9-ddd-e-quando-ele-se-aplica

 - In some cases we just need a CRUD, the DDD should be used to organize the modeling of the central classes in the application.

### Data Structures

.

### Design Patterns

* https://www.patterns.dev/posts/classic-design-patterns/
