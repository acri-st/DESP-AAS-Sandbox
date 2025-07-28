# DESP-AAS Sandbox

This project contains multiple microservices designed to simulate our production environment.

## Table of Contents
- [🧪 What is the Sandbox?](https://github.com/acri-st/DESP-AAS-Sandbox#-what-is-the-sandbox)
- [⚙️ Technical description](https://github.com/acri-st/DESP-AAS-Sandbox#%EF%B8%8F-technical-description)
  - [🗺️ Architecture](https://github.com/acri-st/DESP-AAS-Sandbox#%EF%B8%8F-architecture)
  - [📄 Microservices description](https://github.com/acri-st/DESP-AAS-Sandbox#-microservices-description)
    - [📦 Sandbox UI](https://github.com/acri-st/DESP-AAS-Sandbox#-what-is-the-sandbox-ui-back-to-architecture)
    - [📦 Project Management](https://github.com/acri-st/DESP-AAS-Sandbox#-what-is-the-project-management-back-to-architecture)
    - [📦 VM Management](https://github.com/acri-st/DESP-AAS-Sandbox#-what-is-the-vm-management-back-to-architecture)
    - [📦 Storage](https://github.com/acri-st/DESP-AAS-Sandbox#-what-is-the-storage-back-to-architecture)
    - [📦 UI Framework](https://github.com/acri-st/DESP-AAS-Sandbox#-what-is-the-ui-framework-back-to-architecture)
    - [📦 Admin UI](https://github.com/acri-st/DESP-AAS-Sandbox#-what-is-the-admin-ui-back-to-architecture)
- [🧰 Setup](https://github.com/acri-st/DESP-AAS-Sandbox#-setup)

## 🧪 What is the Sandbox?

Sandbox is a service that allows users to develop applications and models using cloud based services and to ease the deployment to the collaborative platform.

## ⚙️ Technical description
### 🗺️ Architecture
The Microservices that make up the Sandbox project are the following: 
- **Authentication** (to be provided by each contributor)
- **Sandbox UI** [📄Description](https://github.com/acri-st/DESP-AAS-Sandbox#-what-is-the-sandbox-ui-back-to-architecture) [🔗Repository](https://github.com/acri-st/sandbox-ui)  
- **Project management** [📄Description](https://github.com/acri-st/DESP-AAS-Sandbox#-what-is-the-project-management-back-to-architecture) [🔗Repository](https://github.com/acri-st/project-management)
- **VM management** [📄Description](https://github.com/acri-st/DESP-AAS-Sandbox#-what-is-the-vm-management-back-to-architecture) [🔗Repository](https://github.com/acri-st/vm-management)
- **Storage** [📄Description](https://github.com/acri-st/DESP-AAS-Sandbox#-what-is-the-storage-back-to-architecture) [🔗Repository](https://github.com/acri-st/storage)
- **UI Framework** [📄Description](https://github.com/acri-st/DESP-AAS-Sandbox#-what-is-the-ui-framework-back-to-architecture) [🔗Repository](https://github.com/acri-st/ui-fwk)
- **Admin UI** [📄Description](https://github.com/acri-st/DESP-AAS-Sandbox#-what-is-the-admin-ui-back-to-architecture) [🔗Repository](https://github.com/acri-st/admin-ui)

![Sandbox Architecture](https://github.com/acri-st/sandbox-ui/blob/main/docs/architecture.png?raw=true)

### 📄 Microservices description

#### 📦 What is the Sandbox UI? [Back to Architecture](https://github.com/acri-st/DESP-AAS-Sandbox#%EF%B8%8F-architecture)

The sandbox UI is a web application that interfaces with the microservices that comprise the Sandbox ecosystem. It provides a user-friendly interface for testing, debugging, and interacting with various microservices in a controlled sandbox environment.
The Sandbox UI also uses a common library that contains interfaces to services and styling.  

#### 📦 What is the Project Management? [Back to Architecture](https://github.com/acri-st/DESP-AAS-Sandbox#%EF%B8%8F-architecture)

Project Management is a microservice that serves as the central hub for managing projects. It provides a comprehensive interface for creating, organizing, and overseeing sandbox project.

The Project Management UI enables users to:
- Create and configure new projects
- Manage project settings and configurations
- Monitor project status and resources
- Coordinate with other microservices (Auth, VM management, Storage)
- Access project development environments and tools  

#### 📦 What is the VM Management? [Back to Architecture](https://github.com/acri-st/DESP-AAS-Sandbox#%EF%B8%8F-architecture)

The VM Management service is a microservice that manages virtual machines for projects. It provides the infrastructure and tools necessary for users to create, configure, and manage virtual machines where they develop and run their applications and models.

The VM Management service handles:
- **VM Provisioning** Creating and deploying virtual machines for user projects
- **Resource Management** Allocating and monitoring compute resources (CPU, memory, storage)
- **Lifecycle Management** Starting, stopping, and terminating VMs as needed
- **Configuration Management** Setting up development environments and required software
- **Integration** Working with other microservices like Project Management and Storage

This service is a critical component of the Sandbox, providing the development environment where users can build and test their applications before deploying to the main collaborative platform.  

#### 📦 What is the Storage? [Back to Architecture](https://github.com/acri-st/DESP-AAS-Sandbox#%EF%B8%8F-architecture)

The Storage service is a microservice that handles file storage and repository management. It provides the infrastructure and tools necessary for users to store, manage, and access files, Git repositories, and metadata associated with their projects.

The Storage Management service handles:
- **Git Repository Management** Creating, managing, and accessing Git repositories for project files
- **File Storage** Storing and retrieving files with support for various formats and binary content
- **Metadata Management** Handling thumbnails, avatars, and other metadata associated with assets
- **Image Processing** Resizing, cropping, and optimizing images for thumbnails and avatars
- **Content Delivery** Streaming file content and serving static assets
- **Integration** Working with other microservices like Asset Management and Auth

#### 📦 What is the UI framework? [Back to Architecture](https://github.com/acri-st/DESP-AAS-Sandbox#%EF%B8%8F-architecture)

The UI framework is the library that is used in collaborative-ui, sandbox-ui and admin-ui for utilities, React components, API interfaces, typings and more.  

#### 📦 What is the Admin UI? [Back to Architecture](https://github.com/acri-st/DESP-AAS-Sandbox#%EF%B8%8F-architecture)

The admin UI is a web application that interfaces with the microservices that comprise the collaborative platform and the sandbox for administrators to manipulate and moderate.  

## 🧰 Setup

See each microservice's README for local development instructions.
