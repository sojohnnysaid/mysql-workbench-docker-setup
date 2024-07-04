# 🐬 MySQL Workbench Docker Setup 🐳

This project provides a quick and easy way to set up MySQL and MySQL Workbench in Docker containers. Perfect for development environments or quick database management tasks! 🚀

## 🎯 Purpose

The purpose of this setup is to:

- Quickly spin up a MySQL database 📊
- Provide a web-based MySQL Workbench interface 🖥️
- Ensure data persistence across container restarts 💾

## 🏁 Quickstart

1. Clone this repository:
git clone https://github.com/yourusername/mysql-workbench-docker.git
cd mysql-workbench-docker

2. Start the containers:
docker-compose up -d

3. Access MySQL Workbench:
- 🌐 Open your web browser
- 🔗 Go to http://localhost:3000 (HTTP) or https://localhost:3001 (HTTPS)

4. Connect to your MySQL database:
- 🏠 Hostname: db
- 🚪 Port: 3306
- 👤 Username: root
- 🔑 Password: rootpassword

## 🛠️ Configuration

You can modify the `docker-compose.yml` file to change:
- Database credentials
- Port mappings
- Volume locations

Don't forget to rebuild your containers after making changes!

## 🛑 Stopping the Containers

To stop and remove the containers, run:
docker-compose down

🎉 Happy Coding!
