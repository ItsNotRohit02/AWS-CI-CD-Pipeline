# CI/CD Pipeline for Java Application Using AWS Services

This project sets up a fully automated CI/CD (Continuous Integration/Continuous Deployment) pipeline for a Java web application using various AWS services. 

### Key Features

- **AWS Elastic Beanstalk** for scalable application deployment.
- **Amazon RDS** for a reliable, managed relational database.
- **GitHub** as the source control repository.
- **AWS CodeBuild** to compile source code, run tests, and produce deployment-ready packages.
- **AWS CodePipeline** to automate the entire CI/CD workflow, from source code commit to production deployment.

### Project Components

1. **Elastic Beanstalk**: Handles the deployment and management of the Java web application.
2. **Amazon RDS**: Provides the database instance, connected to the application.
3. **CodeBuild**: Executes the build process as defined in the `buildspec.yaml` file, compiling the Java code and running tests.
4. **CodePipeline**: Orchestrates the CI/CD process, integrating the CodeBuild jobs, GitHub repository, and Elastic Beanstalk environment.

### Build and Deployment Process

The build process is defined in the `buildspec.yaml` file, which includes:
- Installing required dependencies.
- Configuring the database connection settings.
- Compiling and packaging the Java application into a WAR file.
- Artifacts are stored and used by Elastic Beanstalk for deployment.
