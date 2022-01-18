
# General introduction
A Software Bill of Materials, (or an SBOM), is a complete, formally structured list of components, libraries, and modules that are required to build (i.e. compile and link) a given piece of software and the supply chain relationships between them.
That's why using Syft can be really useful.
Syft is a CLI tool and Go library for generating a Software Bill of Materials (SBOM) from container images and filesystems. 
# Some basic functionalities
## Why using Syft
Adding Syft scans to the workflow keeps us informed of the used packages. Once we’ve got this information, we can begin assessing each package to determine whether it’s really needed. If we find a lot of packages that aren’t used by our workload, we consider switching to a minimal base image and layering only essential software on top.
## How it works

Syft’s functionality is currently exposed by a single sub-command, syft packages.
Pass it an image tag to generate an SBOM for:
```
syft <image>
```
or
```
syft packages <image>
```
### Demo
![](https://user-images.githubusercontent.com/590471/90277200-2a253000-de33-11ea-893f-32c219eea11a.gif)
# Advantages
* Many output formats available
	* json
	* cyclonedx / cyclonedx-json
	* spdx / spdx-json
	* table
* Supports many popular package formats.
* Easy CI/CD scans thanks to the standardized CycloneDX and SPDX formats .
* Also useful for arbitrary filesystem paths.
# Disadvantages
* Some packages may not be supported
* 
# Useful links

[1](https://en.wikipedia.org/wiki/Software_bill_of_materials)
[2](https://github.com/anchore/syft)
[3](https://www.cloudsavvyit.com/14680/how-to-index-your-docker-images-dependencies-with-syft/)
[4](https://thenewstack.io/generate-a-software-bill-of-materials-for-a-container-image-with-syft/)
[5](https://www.youtube.com/watch?v=9oj3BC3vOtc)
