# General introduction
 **Ha**skell **do**cker **lint** is a smarter Dockerfile linter that helps you build best practice Docker images. 
 
# Some basic functionalities
The linter parses the Dockerfile into an AST and performs rules on top of the AST. Hadolint not only lints the docker instructions, but it also incorporates ShellCheck which lints any bash or sh code used in the docker RUN instructions.
### How it works?
* **locally**
```bash
hadolint <Dockerfile>
hadolint --ignore DL3003 --ignore DL3006 <Dockerfile> # exclude specific rules
hadolint --trusted-registry my-company.com:500 <Dockerfile> # Warn when using untrusted FROM images
```
* **In a Docker container**
Just pipe your `Dockerfile` to `docker run`:

```bash
docker run --rm -i hadolint/hadolint < Dockerfile
# OR
docker run --rm -i ghcr.io/hadolint/hadolint < Dockerfile
```


# Advantages
* Open source
* lightweight
* Simple to use
* Flexible integration
	*Can be implemented inside a GitLab CI Pipeline.
	* Available as VS code extention
* Insure a clean Dockerfile
# Disadvantages
* None
# Useful links

[1](https://medium.com/@david.w.elliott/dockerfile-linting-every-time-everywhere-d8d271a1e650)
[2](https://osvaldo-gonzalez-venegas.medium.com/hadolint-slim-and-smart-dockerfile-linter-ba9bdad2145b)
[3](https://github.com/hadolint/hadolint)
