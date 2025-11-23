# Docker Commands 

## Build Image
```bash
docker build -t welcome-app .
```

## Show Images
docker images

## Run Container
docker run -p 5000:5000 welcome-app

## Running Containers
docker ps

------------------------------------------------------------

# Deployment to Docker Hub

## Login
docker login

## Remove Image by ID
docker image rm -f 878909e6d1a2

## Build Image for Docker Hub
docker build -t vignay/welcome-app .

## OR Tag Image
docker tag vignay/welcome-app vignay/welcome-app1

## Push to Docker Hub
docker push vignay/welcome-app

------------------------------------------------------------

# Pull & Remove From Docker Hub

## Remove Local Image
docker image rm -f vignay/welcome-app:latest

## Pull Image
docker pull vignay/welcome-app:latest

## Run Pulled Image
docker run -d -p 5000:5000 vignay/welcome-app:latest

Example Container ID:
a27db429131d2b226aa937979475d6466615726a355297305dbef42e0ca56f25

------------------------------------------------------------

# Application Access
http://127.0.0.1:5000/
http://localhost:5000/git

# Port Mapping
5000:5000  → host:container
