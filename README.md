# CI/CD Pipeline

* This example shows a ci/cd pipeline that can be used for automating build/deployments.
* It contains a sample Jenkinsfile at `ci/Jenkinsfile` that shows how a specific branch (eg: `master`) can be built from git.
* I have specified a dummy script in the signing step, as I am not aware of the actual commands/tools used for signing.
* The assumption is that the Jenkins set up already has Windows worker nodes for building files for Windows platform. I am unfamiliar with building for macosx, but I suppose it could be cross built on a linux machine. In this case, we could configure parallel pipeline steps to build that simultaneously.
* Below is a sequence diagram that shows the steps in the pipeline:

## CI/CD Pipeline Sequence Diagram

![CI CD Sequence Diagram](cicd-seq.jpg?raw=true "CI/CD Sequence Diagram")
