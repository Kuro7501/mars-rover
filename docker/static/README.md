docker build -t static-server .
docker run -p 8080:80 static-server