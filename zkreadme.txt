cd to root [/imgproxy]
docker build -t imgproxy -f docker/Dockerfile . 

docker run -d --restart=always -e IMGPROXY_USER_AGENT='Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36' -p 8888:8080 --name imageproxy -t imgproxy
