* Docker Nessus

- Build image
docker build --squash -t nessus:v1 -f Dockerfile .

- Run image to container
docker run -it --name nessus1 -p 8834:8834 -d nessus:v1
