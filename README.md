# 🚀 EC2 Streamlit Application

## 📖 Overview
Welcome to **My App**! This project is a Dockerized application that serves a web interface for **[brief description of your app, e.g., "an interactive data visualization tool for analyzing mushroom species"]**. It is built using **Python** and **Streamlit**, providing an engaging and user-friendly experience for users to explore and interact with data.

## 🌟 Features
- **Interactive UI**: Users can easily navigate through the application and visualize data.
- **Data Analysis**: Perform various analyses on the provided datasets.
- **Responsive Design**: The application is designed to work seamlessly on different devices.

---

## 🛠️ Prerequisites
Before you begin, ensure you have met the following requirements:

- An **Amazon Linux 2** instance running on AWS EC2.
- **Docker** installed on your instance.
- Access to your **AWS EC2 instance** via SSH.
- Basic knowledge of using the command line.

## 📋 Required Software
- **Docker**: A platform for developing, shipping, and running applications in containers.
- **SSH Client**: To connect to your EC2 instance.

---

## 📦 Setup Instructions

### 1️⃣ Update the System and Install Docker
First, update your system packages to ensure you have the latest versions:

```sh
sudo yum update -y
sudo yum install docker -y
```

Start and enable Docker:

```sh
sudo systemctl start docker
sudo systemctl enable docker
```

### 2️⃣ Clone the Repository
Clone this repository onto your EC2 instance:

```sh
git clone https://github.com/your-repository-url.git
cd your-repository-folder
```

### 3️⃣ Build and Run the Docker Container
Build the Docker image:

```sh
docker build -t my-streamlit-app .
```

Run the Docker container:

```sh
docker run -d -p 8501:8501 my-streamlit-app
```

### 4️⃣ Access the Application
Once the container is running, you can access your Streamlit application via:

```
http://your-ec2-public-ip:8501
```

Use the following command to check running containers:

```sh
docker ps
```

---

## 🔧 Stopping and Managing the Application
To stop the running container:

```sh
docker stop <container_id>
```

To remove the container:

```sh
docker rm <container_id>
```

To remove the Docker image:

```sh
docker rmi my-streamlit-app
```

---

## 📜 License
This project is licensed under the [MIT License](LICENSE).

## 🤝 Contributing
Contributions are welcome! If you'd like to improve this project, please fork the repository and submit a pull request.

## 📞 Support
For any issues or questions, feel free to reach out by creating an issue in this repository.

---

🌟 Happy Coding! 🚀

