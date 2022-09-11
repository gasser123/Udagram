# Infrastracture description
 ### Built With

- [Angular] Single Page Application Framework
- [Node] Javascript Runtime
- [Express] Javascript API Framework


 ### Unit Tests:

 Unit tests are using the Jasmine Framework.

 ### End to End Tests:

 The e2e tests are using Protractor and Jasmine.

 version of ChromeDriver should be compatible with chrome version inorder for the test to run successfully.



## Dependencies

```
- Node v14.15.1 (LTS) 

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project.

- AWS CLI v2.

- EB CLI.

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

- A S3 bucket for hosting the static website.

```
## Pipeline process
```
- CI/CD pipeline is done using CircleCI connected to github repo.
- configuration of the pipeline lies is in .circleci/config.yml
- changes are detected by CircleCI when pushing to the main branch.
- installation then is started and building the app and if successful CircleCI waits for manual approval inorder to start the     deploy process.

```