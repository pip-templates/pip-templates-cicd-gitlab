# Overview

This is template for GitLab CI/CD pipeline for node js microservice. View dockerfiles in [Dockerization template](https://github.com/pip-templates/pip-templates-microservice-dockerization).

# Usage

Copy component.json, .gitlab-ci.yml and *.ps1 scripts to microservice folder and enable runner on gitlab repository Settings -> CI/CD -> Runners.

# Settings

Required environment variables:
* **DOCKER_IP** - docker ip for gitlab runner
* **DOCKER_USER** - docker username to access docker registry on image publish
* **DOCKER_PASS** - docker password to access docker registry on image publish
* **RETRY** - set true to restart pipeline in case of falure on npm install
* **NPM_USER** - credentials required for release script. npm username
* **NPM_PASS** - credentials required for release script. npm password
* **NPM_EMAIL** - credentials required for release script. npm email

Variables for piptemplates-devops-buildtasks:
* **GITLAB_URL** - gitlab url
* **API_TOKEN** - gitlab api token
* **BUILD_NUMBER** - automatically incremented build number

Set all of this variables on gitlab repository Settings -> CI/CD -> Variables.
