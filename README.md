**CleanStart Harbor Registry Image
**
---

**📌 Introduction ** 
The `cleanstart/harbor-registry` image provides a secure, scalable, and production-ready container registry for managing Docker and OCI images.

✔️ Enterprise-grade container registry  
✔️ Security-focused with role-based access control (RBAC)  
✔️ Integrated vulnerability scanning  

It is designed for private container image storage, enabling teams to securely manage, sign, and scan container images.

---

**📌 Why Use `cleanstart/harbor-registry`?  **
✔️ Secure & Private → Role-based access control (RBAC) and image vulnerability scanning.  
🚀 Cloud Native → Optimized for Kubernetes and containerized environments.  
🛠️ Performance Optimized → Fast and efficient image storage and retrieval.  
📦 Flexible Deployment → Supports both on-premises and cloud environments.  

---

🚀 Getting Started  

🐳 Pulling the Harbor Registry Image  
To use Harbor, you first need to pull the Docker image:  

```
docker pull cleanstart/harbor-registry:latest
```

---

**🔹 Variants**
CleanStart provides two image variants:

harbor-registry:latest → Standard Harbor Registry for production.
harbor-registry:latest-dev → Development variant with additional tools.

---

**🔹 Standard Variant (Recommended for Production)**
To pull the standard production-ready image:

```
docker pull cleanstart/harbor-registry:latest
```
**🔹 Development Variant (For Debugging & Testing):**
To pull the development variant with additional tools image:

```
docker pull cleanstart/harbor-registry:latest-dev
```

---

**🛠️ Usage Examples**

💻 Running Harbor Registry as a Standalone Container

```
docker run -d --name harbor-registry -p 5000:5000 cleanstart/harbor-registry:latest
```
Access the registry at: http://localhost:5000⁠

---

**⚠️ Running as Root (for Debugging in -dev Variant)**

```
docker run -it --user root --entrypoint /bin/bash cleanstart/harbor-registry:latest-dev
```
📌 Note: Running as root is not recommended in production.

---

**🔗 Harbor Registry Container Image**
This image is available on both GitHub Container Registry and Docker Hub.

🔗 GitHub Container Registry: clnstrt/harbor-registry

🔗 Docker Hub: docker pull: cleanstart/harbor-registry:latest

---
**Docker Hub Repository**

This image is available on Docker Hub: [cleanstart/harbor-registry](https://hub.docker.com/repository/docker/cleanstart/harbor-registry)

