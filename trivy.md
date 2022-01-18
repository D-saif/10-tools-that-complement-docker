# General introduction
 When it comes to secutity, Trivy is a really useful tool for scanning vulnerabilities in container images, file systems, and Git repositories, as well as IaC files (ex. terraform, k8s..).
# Some basic functionalities
## Scan Image for Vulnerabilities
Simply we should specify an image name (and a tag).

```
$ trivy image [IMAGE_NAME]
```

For example:

```
$ trivy image python:3.4-alpine
```
# Advantages
* Easy to use
* Fast 
* Suitable for DevSecOps
    * Suitable for CI such as GitHub Actions, Jenkins, GitLab CI, etc.
* Easy integration (GitHub Actions, Visual Studio Code)
* Supports local and remote images

# Disadvantages

# Useful links

[1](https://www.cloudsavvyit.com/12027/how-to-use-trivy-to-find-vulnerabilities-in-docker-containers/)
[2](https://github.com/aquasecurity/trivy)
[3](https://www.hacking.land/2019/11/trivy-simple-and-comprehensive.html?m=1)
