# Overview
---
This is a repository for an open-source project of **SST (Secure Swarm Toolkit)** and the local authentication and authorization entity, **Auth**, for security of the Internet of Things (IoT). Auth is a local point of authorization, whose main roles are 1) providing authentication/authorization for its locally registered entities or devices, and 2) working as a bridge of authorization between its local entities and the Internet. 

Our conference papers [[IoTDI '17](https://dl.acm.org/citation.cfm?id=3054980)], [[FiCloud '16](http://ieeexplore.ieee.org/document/7575852/)] describe a secure network architecture with key distribution mechanisms using Auth (local, automated authorization entity). The architecture provides security guarantees while addressing IoT-related issues including resource constraints and intermittent connectivity. The architectural concept of locally centralized, globally distributed authentication and authorization is illustrated in our journal article [[IT Professional '17'](https://ieeexplore.ieee.org/document/8057722/)]. Our recent journal article [[ACM TIOT '20](https://dl.acm.org/doi/abs/10.1145/3375837)] presents a secure migration technique as a recovery mechanism from Denial-of-Service (DoS) attacks or failures.

This repository includes 1) an open-source Java implementation of Auth and 2) sample codes for local entities to use Auth (authentication/authorization) services provided by Auth in various programming languages for different platforms.

# Prerequisites
---

1. OpenSSL command line tools for creating certificates and keystores of Auths and example entities
2. Java 11 or above
3. [IntelliJ IDEA](https://www.jetbrains.com/idea/) for managing Java project of Auth
4. [Maven CLI (command line interface)](http://maven.apache.org/ref/3.1.0/maven-embedder/cli.html) for building Auth from command line
5. Node.js for running example server and client entities

# Directory structure
---
- **android**: Directory for SST's Auth and entities for Android platform (*currently under development*)
- **auth**: Directory for the Java implementation of Auth (local authentication/authorization entity), IntelliJ IDEA project
- **entity**: Directory for SST's C and JavaScript APIs and example IoT entities using SST to be authenticated/authorized by Auth. This direcotry also includes [a sub-directory](https://github.com/iotauth/iotauth/tree/master/entity/node/accessors) for *Secure Communication Accessors* as software building blocks for writing IoT applications.
- **examples**: Directory for scripts and descriptions to run example Auths and entities.

# Quick start with example Auths and entities
---
See "How to run examples" in [README.md under *examples/*](https://github.com/iotauth/iotauth/blob/master/examples/README.md) for a fully working example.

# Contributors
---
- [Hokeun Kim](https://hokeun.github.io/) (Assistant Professor at Hanyang University IoT Lab)
- [Salomon Lee](https://www.linkedin.com/in/salomon-lee-637b0921) (CTO at AlcaCruz Inc.)
- [Eunsuk Kang](https://eskang.github.io/) (Assistant Professor at Carnegie Mellon University)
- [Marten Lohstroh](https://people.eecs.berkeley.edu/~marten/) (Postdoctoral researcher at UC Berkeley)
- [Dongha Kim](https://github.com/Jakio815) (M.S./Ph.D. Student at Hanyang University IoT Lab)
- [Yeongbin Jo](https://github.com/yeongbin7) (M.S. Student at Hanyang University IoT Lab)
- [Taekyung Kim](https://github.com/LukeKimm) (M.S. Student at Hanyang University IoT Lab)
- [Hanyang University IoT Lab](https://hyu-iot.github.io/)

# External libraries
---
- **bluecove-2.1.2.jar**: For bluetooth APIs, exists under auth/library/jars

# Disclaimer
---
This project is still in its infancy and currently intended for academic and research purposes, although the ultimate goal of this project is to build a secure and robust network architecture for the Internet of Things. Therefore, users must use the provided source codes with caution at their own risk, when the tools provided in this project are used for commercial or safety-critical purposes.

# Acknowledgement
---
This work was supported in part by the TerraSwarm Research Center, one of six centers supported by the STARnet phase of the Focus Center Research Program (FCRP) a Semiconductor Research Corporation program sponsored by MARCO and DARPA.

*Last updated on September 26, 2022*
