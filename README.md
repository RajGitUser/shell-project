🐚 Shell Project

A collection of Bash/Shell scripts and service definitions to automate setup and deployment tasks for different microservices and infrastructure components. This project aims to provide reusable scripts for managing services such as catalogue, cart, payment, shipping, user, and associated tooling like MongoDB, Redis, MySQL, RabbitMQ, etc. 
GitHub

📌 Table of Contents

About

Repository Structure

Prerequisites

Usage

Scripts & Services

Contributing

License

🤔 About

This repository contains useful shell scripts that help automate and bootstrap various components of a project environment. The scripts are typically used for:

✔ Service installation & configuration
✔ Application setup
✔ Environment initialization
✔ Infrastructure bootstrapping
✔ System automation via shell scripting

All scripts are written in Bash (Shell). 
GitHub

📁 Repository Structure
shell-project/
├── 01-roboshop.sh
├── catalogue.sh
├── cart.sh
├── frontend.sh
├── mongodb.sh
├── mysql.sh
├── payment.sh
├── rabbitmq.sh
├── redis.sh
├── user.sh
├── catalogue.service
├── cart.service
├── payment.service
├── shipping.service
├── user.service
├── mongo.repo
└── rabbitmq.repo
``` :contentReference[oaicite:3]{index=3}

Shell scripts automate service tasks, while `.service` and `.repo` files define systemd service units and repository configurations respectively.

---

## 🧰 Prerequisites

Before using these scripts, ensure:

✔ You’re running on a **Linux environment with Bash installed**  
✔ You have **sudo or root privileges** if executing system operations  
✔ Required command line tools (e.g., `curl`, `yum`/`apt`, `systemctl`) are available  
✔ Your environment matches the expected service dependencies

Feel free to modify/install dependencies as needed.

---

## 🚀 Usage

### 1. Clone the Repository

```bash
git clone https://github.com/RajGitUser/shell-project.git
cd shell-project

2. Make Scripts Executable
chmod +x *.sh

3. Run a Script
./01-roboshop.sh


Or execute any individual script, for example:

./catalogue.sh


Scripts are designed to automate tasks like installation or configuration for targeted components.

📦 Scripts & Service Definitions
⭐ Installation & Setup Scripts
File	Purpose
01-roboshop.sh	Master script that orchestrates setup
catalogue.sh	Setup for catalogue service
cart.sh	Setup for cart service
payment.sh	Setup for payment service
user.sh	Setup for user service
frontend.sh	Setup for frontend
⭐ Dependency & System Scripts
File	Purpose
mongodb.sh	Installs/configures MongoDB
redis.sh	Installs/configures Redis
mysql.sh	Installs/configures MySQL
rabbitmq.sh	Installs/configures RabbitMQ
⭐ Systemd & Repo Files
File	Purpose
*.service	Systemd service definitions for each microservice
*.repo	Repository configuration for package manager

These definitions help manage services via systemctl.

📌 Tips

✔ Read each script before executing it in a production environment
✔ Use version control branches when making changes
✔ Modify service units under /etc/systemd/system/ if needed

🤝 Contributing

Contributions are welcome!

Fork the repository

Create a feature branch

Make improvements (add scripts, refactor, document)

Open a Pull Request
