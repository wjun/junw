# Steps to generate a http server and build a container image and run image as a container
- export GOOS=linux
- go build helloserver.go
- docker build .
- docker images
- docker tag image_id your_docker_hub_account_name/your_docker_hub_repository_name
- docker push image_id your_docker_hub_account_name/your_docker_hub_repository_name
- docker run -id image_id your_docker_hub_account_name/your_docker_hub_repository_name
