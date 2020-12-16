# CI/CD Pipeline

* This example shows a ci/cd pipelines that can be used for automating build/deployments.

Backend App:
* The Jenkinsfile at `ci/Jenkinsfile.backend` shows a skeleton pipeline outlining the steps to build and deploy the backend Node.js application.
* The pipeline has conditional stage to make deployments only from `master` branch.


Desktop App:
* A sample Jenkinsfile at `ci/Jenkinsfile` that shows how a specific branch (eg: `master`) can be built from git.
* I have specified a dummy script in the signing step, as I am not aware of the actual commands/tools used for signing.
* The assumption is that the Jenkins set up already has Windows and MacOS worker nodes for building files for Windows and Mac platforms. These two builds happen in parallel.
* Below is a sequence diagram that shows the steps in the pipeline:


## CI/CD Pipeline Sequence Diagram

![CI CD Sequence Diagram](cicd-seq.jpg?raw=true "CI/CD Sequence Diagram")
