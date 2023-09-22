# CI/CD Process & Elements & Flows

## Actually, what is CI/CD?

[CI/CD](https://en.wikipedia.org/wiki/CI/CD) is the combination of Continuous Integration (CI) and Continuous Delivery (CD), in order to offer a more efficient process for delivery the work of various contributors into the final product. 
In the realm of software development and DevOps, CI/CD embodies the continuous process of coding, testing, and delivering a software product by furnishing teams with a unified repository for their work, complemented by automation tools that uphold the consistent and frequent integration, testing, and deployment to production.

## CI/CD process flow

<center><img src="/img/ci-cd.png" width=70% /></center>

The CI/CD workflow represents a set of steps designed to facilitate the smooth integration, testing, and deployment of code for developers. Beside the Plan > Code > Build > Test > Deploy > Operate cycle, there are some key elements to establish a stable CI/CD process:

#### CI - Frequent commits
Every developers consistently commit and push their work to a VCS like Bitbucket/GitHub/GitLab. Each push to the VCS starts the CI process.

#### CI - Static code analysis
The CI process enforces static code analyse tools to check every commit in order to assure code quality.

#### CI - Unit tests
These tests focus on individual components and ensure that the code’s basic correctness without the need of ofter components. A failed unit test breaks the build process itself and the pipeline execution halts, and developers are notified. 

#### CI - Tests are automated
After compiling/packaging integration tests are automatically run, before generating the final artefact. Finally establishing an automated and standardized process for development, packaging, and testing.  
But there are additional automated tests needed, to ensure the build meets all functional and non-functional requirements:

- **Integration tests**  
These tests validate the interactions between different components of the application, so they can work seamlessly together.
- **Functional tests (user test and end-to-end tests)**  
These tests verify that the application behaves as expected from an end-user’s perspective.
- **Performance tests**  
Performance tests ensure the application responds quickly and remains stable under heavy load.
- **Security tests**  
Security scans and tests look for any potential vulnerabilities.


#### CD - starts after CI 
Continuous Delivery starts where Continuous Integration ends. It is responsible for deplyoing all code changes automatically to pre-defined environments (e.g. dev-, test- or pre-production-envirnonment). When there is manual interaction to deploy a build, this is called Continous Deployment.

### Benefits

The CI/CD pipeline allows developers to commit new code, that is checked through various testing stages like sourcing, building, staging, and production, and finally, release it as production-ready code.

Every stage in the CI/CD pipeline is like a checkpoint to confirm specific criterias. The pipeline assures that as the new code passes every checkpoint, its quality improves due to different attributes being validated.

Test results are communicated as fast as possible. If the code fails at any stage, the pipeline ist stopped and the developer informed that it failed.

Every organisations and project has different needs and requirements. So the the CI/CD process should be adjusted accordingly - like quality, security, and performance. Another importand key for a successful pipeline is to continuously review and update the CI/CD process.

## Best Practises

ToDo