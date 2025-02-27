

### [Git](#Git)
### [Docker](#Docker)

# **Git**  
*A distributed version control system for tracking code changes.*  
- [核心概念](#git-core-concepts)  

## **Git-Core-Concepts**  

### **1. 工作区（Working Directory）**  
- **未跟踪文件（Untracked Files）**：新文件默认未被 Git 追踪，需 `git add <file>` 加入暂存区。  
- **已修改文件（Modified Files）**：可以使用 `git status` 查看修改状态，`git diff` 比较未暂存的变更。  
- **撤销修改**：使用 `git checkout -- <file>` 丢弃本地修改，或 `git reset HEAD <file>` 移出暂存区。  

### **2. 暂存区（Staging Area）**  
- `git add <file>`：将修改的文件添加到暂存区。  
- `git rm --cached <file>`：从暂存区移除文件，但不删除本地文件。  

### **3. 版本库（Repository）**  
- `git commit -m "commit message"`：提交暂存区的更改到本地仓库。  
- `git log`：查看提交历史。  
- `git reset --soft HEAD~1`：撤回最近一次提交，但保留更改。  

### **4. 远程仓库（Remote Repository）**  
- `git push origin main`：将本地 `main` 分支推送到远程仓库。  
- `git pull origin main`：拉取远程 `main` 分支的最新更改。  
- `git clone <repo_url>`：克隆远程仓库。  

[返回顶部](#git)  

---

# **Docker**  
*A platform to develop, ship, and run applications in containers.*  
- [核心概念](#docker-core-concepts)  

## **Docker-Core-Concepts**  

### **1. 镜像（Images）**  
- `docker pull <image>`：从 Docker Hub 拉取镜像。  
- `docker images`：列出本地镜像。  
- `docker rmi <image>`：删除指定镜像。  

### **2. 容器（Containers）**  
- `docker run -d --name <container_name> <image>`：后台运行容器。  
- `docker ps -a`：查看所有容器（包括已停止的）。  
- `docker stop <container>`：停止容器。  
- `docker rm <container>`：删除容器。  

### **3. Dockerfile & 构建（Build）**  
- `docker build -t <image_name> .`：基于 `Dockerfile` 构建镜像。  
- `docker run -p 8080:80 <image_name>`：运行容器，并映射端口 `8080` 到 `80`。  

### **4. Docker Compose**  
- `docker-compose up -d`：根据 `docker-compose.yml` 运行多个容器。  
- `docker-compose down`：停止并删除所有容器。  

[返回顶部](#docker)  




