# Settings

Required environment variables:
* **DOCKER_IP** - docker ip for gitlab runner
* **DOCKER_USER** - docker username to access docker registry on image publish
* **DOCKER_PASS** - docker password to access docker registry on image publish
* **RETRY** - set true to restart pipeline in case of falure on npm install

Variables for piptemplates-devops-buildtasks:
* **GITLAB_URL** - gitlab url
* **API_TOKEN** - gitlab api token
* **BUILD_NUMBER** - automatically incremented build number