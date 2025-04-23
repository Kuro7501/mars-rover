docker build -t python-server .
docker run -d -p 8080:80 python-server