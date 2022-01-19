
![dive](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DuBd7QPvhLMU&psig=AOvVaw31JDTBTsZAZsJO691h-mH2&ust=1642709824218000&source=images&cd=vfe&ved=0CAsQjRxqFwoTCIjelJLRvvUCFQAAAAAdAAAAABAD)


# General introduction
 - In today's IT industry, there is a lot of methods for inspecting docker images like exorting the container filesyste, {creating a stoped container and then export it's filesystem}, saving images data directly, listing image layers with "docker image history " command ...

 - A better way of doing this is to use a 3rd party tools with graphical user interface and visualisation capabilities like Dive 
 
## How it works? 
-a tool expressly built for visualizing image content. It uses a layer-based approach and highlights the filesystem changes made with each new layer. You browse through the filesystem using a tree-based interactive terminal view.

![dive](https://www.google.com/url?sa=i&url=https%3A%2F%2Fblog.pentesteracademy.com%2Flearn-to-analyze-docker-image-with-dive-tool-4cdee4aeef6b&psig=AOvVaw31JDTBTsZAZsJO691h-mH2&ust=1642709824218000&source=images&cd=vfe&ved=0CAsQjRxqFwoTCIjelJLRvvUCFQAAAAAdAAAAABAK)


# Advantages
Dive come to the table to let u inspect docker image filesystem before running the container to asses the image suitability and avoid securty issues as that image could contains a malicious(malicious entrypoint script)# Disadvantages

# Useful links
[1](https://www.cloudsavvyit.com/14663/how-to-inspect-a-docker-images-content-without-starting-a-container/)
[2](https://github.com/wagoodman/dive)