# 🐬 MySQL Workbench Docker Setup 🐳

This project provides a quick and easy way to set up MySQL and MySQL Workbench in Docker containers. Perfect for development environments or quick database management tasks! 🚀

## 🎯 Purpose

The purpose of this setup is to:

- Quickly spin up a MySQL database 📊
- Provide a web-based MySQL Workbench interface 🖥️
- Ensure data persistence across container restarts 💾

## 🏁 Quickstart

1. **Create a New Directory**: For a clean setup, create a new directory in a convenient location on your system.
    ```bash
    mkdir my-mysql-setup
    cd my-mysql-setup
    ```

2. **Download the Docker Compose File**: You can clone the entire repository or simply download the `docker-compose.yml` file into this new directory.
    ```bash
    curl -O https://raw.githubusercontent.com/sojohnnysaid/mysql-workbench-docker-setup/main/docker-compose.yml
    ```

3. **Prepare the Mount Points**: Before starting your containers, create the directories that will be used for bind mounts.
    ```bash
    mkdir config workbench_files db_data
    ```

4. **Start the Containers**: Navigate to the directory where your `docker-compose.yml` file is located and start your Docker environment.
    ```bash
    docker-compose up -d
    ```

5. **Access MySQL Workbench**:
    - 🌐 Open your web browser.
    - 🔗 Go to http://localhost:3000 (HTTP) or https://localhost:3001 (HTTPS).

6. **Connect to your MySQL database**:
    - 🏠 Hostname: db
    - 🚪 Port: 3306
    - 👤 Username: root
    - 🔑 Password: rootpassword

## 🔄 Using Bind Mounts

Bind mounts are utilized in this Docker setup to link directories on your host machine to directories in your Docker container. This setup uses bind mounts for dynamic file sharing, ensuring that your configurations and data persist between container restarts.

- **Dynamic:** Changes to files in the host directory are immediately reflected in the container, and vice versa.
- **Persistent:** Custom configurations and data are preserved across container restarts and updates.

## 🛠️ Configuration

Modify the `docker-compose.yml` file to change database credentials, port mappings, or volume locations. Remember to rebuild your containers after making changes!

## 🛑 Stopping the Containers

To stop and remove the containers, run:
```bash
docker-compose down
```

🎉 Happy Coding!
