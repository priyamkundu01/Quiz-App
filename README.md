# How to setup Quiz App

## Pre-requisites
* [Download Git](https://git-scm.com/downloads)

### Clone the repository
```bash
git clone https://github.com/priyamkundu01/Quiz-App.git
```

### Change the directory
```bash
cd Quiz-App
```

## 1. Run with Docker Compose

### Install Docker (if you haven't in your system)
* [Download Docker](https://www.docker.com/get-started/)

### Run this below command
```bash
docker compose up
```

## 2. Run through Dockerfile

### Build the docker image
```bash
docker build -t quiz-app .
```

### Run the quiz app container
```bash
docker run -d -p 5173:5173 quiz-app
```

### Go to the address in your web browser
```bash
http://localhost:5173/
```

## 2. Run without Docker

### Install node (if you haven't in your system)
* [Download Node Js](https://nodejs.org/en/download/)

### Install node modules
```bash
npm install
```

### Run the quiz app
```bash
npm run dev -- --host
```