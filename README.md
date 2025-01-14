

https://hub.docker.com/r/leandrobirth/conversao-distancia/tags

# Distance Converter - Python with Docker

A Python-based application for converting distances between different measurement units, packaged with Docker for seamless deployment and usage.

---

## 🐳 **Run with Docker**

This application is containerized to make it easy to set up and run. You can pull the pre-built image from Docker Hub and quickly start a container.

### Docker Hub Repository
[leandrobirth/conversao-distancia](https://hub.docker.com/r/leandrobirth/conversao-distancia/tags)

---

## 🚀 **Quick Start**

### 1. **Pull the Docker Image**
Download the image from Docker Hub:
```bash
docker pull leandrobirth/conversao-distancia:v2
```

### 2. **Run the Docker Container**
Run the container and expose it on port `5000`:
```bash
docker run -d -p 5000:5000 --name conversao-distancia-container leandrobirth/conversao-distancia:v2
```

### 3. **Access the Application**
Open your browser or use `curl` to access the application:
```
http://localhost:5000
```

---

## 🛠️ **Build Locally with Docker**

If you want to build the Docker image locally instead of pulling it from Docker Hub, follow these steps:

### 1. **Clone the Repository**
```bash
git clone https://github.com/LeandroBirth/conversao-distancia.git
cd conversao-distancia
```

### 2. **Build the Docker Image**
```bash
docker build -t conversao-distancia .
```

### 3. **Run the Container**
```bash
docker run -d -p 5000:5000 --name conversao-distancia-container conversao-distancia
```

### 4. **Test the Application**
Access the application at:
```
http://localhost:5000
```

---

## 🩱 **Clean Up**

To stop and remove the container:
```bash
docker stop conversao-distancia-container
docker rm conversao-distancia-container
```

To remove the Docker image:
```bash
docker rmi leandrobirth/conversao-distancia:v2
```

---

## 📄 **Features**

- Converts distances between metric and imperial units.
- Ready-to-run with Docker to simplify deployment.
- Lightweight and easy to integrate.

---

## 🖥️ **Development**

If you'd like to modify or enhance the application:
1. Clone the repository:
   ```bash
   git clone https://github.com/LeandroBirth/conversao-distancia.git
   cd conversao-distancia
   ```

2. Install dependencies locally:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the application:
   ```bash
   python app.py
   ```

---

## 📦 **Docker Image Details**

- **Base Image**: Python 3.12
- **Exposed Port**: `5000`
- **Entry Command**: Uses `gunicorn` to serve the application.

Visit the [Docker Hub repository](https://hub.docker.com/r/leandrobirth/conversao-distancia/tags) for more information about the available tags.

