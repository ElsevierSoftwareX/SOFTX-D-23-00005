# Overview
---
This is a repository for an open-source project of the local authorization entity, Auth, for security of the Internet of Things (IoT). Auth is a local point of authorization, whose main roles are 1) providing authentication/authorization for its locally registered entities or devices, and 2) working as a bridge of authorization between its local entities and the Internet. 

[Our conference paper](https://chess.eecs.berkeley.edu/pubs/1175/KimEtAl_IoT_Security_FiCloud_2016.pdf) describes a secure network architecture with key distribution mechanisms using Auth (local, automated authorization entity). The architecture provides security guarantees while addressing IoT-related issues including resource constraints and intermittent connectivity.

This repository includes 1) an open-source Java implementation of Auth and 2) sample codes for local entities to use Auth (authentication/authorization) services provided by Auth in various programming languages for different platforms.

# Prerequisites
---

1. OpenSSL command line tools for creating certificates and keystores of Auths and example entities
2. Java 1.8 or above
3. [IntelliJ IDEA](https://www.jetbrains.com/idea/) for managing Java project of Auth
4. [Maven CLI (command line interface)](http://maven.apache.org/ref/3.1.0/maven-embedder/cli.html) for building Auth from command line
5. Node.js for running example server and client entities

# Directory structure
---
- **accessors**: Directory for accessors to use Auth service (*under development*) for details of accessors see [this website](https://www.terraswarm.org/accessors/)
- **auth**: Directory for the Java implementation of Auth (local authentication/authorization entity), IntelliJ IDEA project
- **entity**: Directory for entities in the IoT, to be authenticated/authorized by Auth
- **examples**: Directory for scripts and descriptions to run example Auths and entities.
- **experiments**: Directory for data, results and instructions for conducting experiments used in our conference paper
- **lib**: External libraries used in this project. Currently, this directory includes source code for node-v4.3.2

# Quick start with example Auths and entities
---
See "How to run examples" in [README.md under *examples/*](https://github.com/iotauth/iotauth/blob/master/examples/README.md).

# Contributors
---
- [Hokeun Kim](http://eecs.berkeley.edu/~hokeunkim) (Project manager & initiator)
- Salomon Lee

# Disclaimer
---
This project is still in its infancy and currently intended for academic and research purposes, although the ultimate goal of this project is to build a secure and robust network architecture for the Internet of Things. Therefore, users must use the provided source codes with caution at their own risk, when the tools provided in this project are used for commercial or safety-critical purposes.

*Last updated on August 29, 2016*
