# CircleCI Pipeline Steps

## Jobs

### Build

1. Enviroment Variables are prepared
2. Node.js and CLIs are installed
3. The build process is triggered.
4. Frontend dependencies are installed.
5. Backend dependencies are installed.
6. Frontend is built.
7. Backend is built.

### Test

1. Enviroment Variables are prepared
2. Node.js and CLIs are installed
3. The build process is triggered.
4. Install Google Chrome.
5. Install Chrome driver.
6. Frontend is built.
7. Frontend unit test.

### Deploy

1. Installs Node, EB CLI, AWS CLI.
2. Checkout code.
3. Deploys frontend code to S3.
4. Deployed backend code to EB.

## Workflows

### udagram workflow

1. Calls the build job above.
1. Calls the test job above but require build job.
1. Waits for user's approval to deploy the code after test.
1. If approved, the deploy job above is called.
