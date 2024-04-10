# AsciiArtify Kubernetes Deployment Tools Evaluation

## Introduction
AsciiArtify, a burgeoning startup dedicated to crafting innovative software solutions for converting images into ASCII art through Machine Learning algorithms, encounters the daunting task of choosing the optimal tool for local Kubernetes cluster development. With a team consisting of two adept young programmers skilled in software engineering but relatively inexperienced in DevOps, the venture deliberates among three alternatives: minikube, kind, and k3d.

## Characteristics
### Minikube
- `Supported OS and Architectures:` Works on multiple operating systems, including Windows, macOS, and Linux. Supports various architectures.  
- `Automation Capability:` Offers automation for cluster creation and management.
- `Additional Features:` Suitable for local development and testing. Concerns arise regarding scalability limitations.  

### Kind (Kubernetes IN Docker)
- `Supported OS and Architectures:` Compatible with Windows, macOS, and Linux. Works within Docker containers.  
- `Automation Capability:` Allows the creation of local Kubernetes clusters in Docker containers.  
- `Additional Features:` Considered for local testing purposes.

### k3d
- `Supported OS and Architectures:` Works on multiple operating systems. Uses Rancher Kubernetes Engine (RKE) in Docker containers.
- `Automation Capability:` Facilitates quick creation and testing of Kubernetes clusters in Docker containers.
- `Additional Features:` Chosen for preparing Proof of Concept (PoC).

### Characteristic

| **Pros and Cons**                               | **Minikube**                                     | **Kind**                                         | **k3d**                                                                               
|--------------------------------------------------|--------------------------------------------------|--------------------------------------------------|--------------------------------------------------
| **Pros**                                      | + Easy to use<br>+ Suitable for local development and testing | + Suitable for local development and testing<br>+ Works within Docker containers<br>+ Possibility for local testing | + Suitable for local development and testing<br>+ Works within Docker containers<br>+ Fast cluster creation and testing | 
| **Cons**                                      | - Doubts about scalability<br>- Potential limitations | - Limited information on scalability<br>- Limited community documentation | - Limited documentation<br>- Potential scalability concerns |


## Demonstration
Recommended Tool: k3d Deployment of "Hello World" Application on Kubernetes  

![Application on Kubernetes]( https://github.com/GRYz1n/AsciiArtify/raw/master/doc/demo1.gif )


## Conclusion
Following thorough practical analysis, k3d emerges as the prime candidate for AsciiArtify's Proof of Concept (PoC). Its swift cluster instantiation and user-friendly interface render it ideal for the initial developmental phase. Nevertheless, it's paramount to take into account the sparse community documentation and potential scalability challenges.
AsciiArtify must meticulously evaluate the advantages and drawbacks before reaching a definitive conclusion.
