## Additional information

### 1- Infrastructure description

The application runs on the following infrastructure.

- Postgres AWS RDS instance hosting the database.
!["Pipeline process"](../screenshots/rds/udagram_rds.png "rds")
- Elastic Beanstalk instance running the server app.
!["Pipeline process"](../screenshots/Elastic_Beanstalk/healthy.png "eb")
- S3 Bucket for static website hosting.
!["Pipeline process"](../screenshots/s3/bucket_s3_content.png "s3")

### 2- App dependencies

```
- Node v16.16 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.
```

### 3- Pipeline process
----
!["Pipeline process"](../screenshots/circleci_diagram.png "workflow")
--------------

!["Pipeline process"](../screenshots/circleci/workflow.png "workflow")
!["Pipeline process"](../screenshots/circleci/build_steps.png "build-steps")
!["Pipeline process"](../screenshots/circleci/test_steps.png "test-steps")
!["Pipeline process"](../screenshots/circleci/deploy_steps.png "deploy-steps")


### 4- AWS architecture diagram

!["AWS architecture diagram"](../screenshots/infrastructure_diagram.png "AWS architecture diagram")
!["AWS architecture diagram"](../screenshots/aws.png "AWS architecture diagram")
