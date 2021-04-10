# fc2-graphql\

docker rmi $(docker images -q) -f\
docker rm $(docker ps -a -q) -f\

==================================================================\

docker build -t jjnatanx/go-graphql .\
docker run -it -v /home/jonathan/GO-GRAPHQL:/go/src/app -p 8081:8080 --rm --name go-graphql jjnatanx/go-graphql\

==================================================================

github.com/jdoliveirasa/fc2-graphql\

https://gqlgen.com/getting-started/\

go mod init github.com/jdoliveirasa/fc2-graphql\

go get github.com/99designs/gqlgen\
 
go run github.com/99designs/gqlgen init\

go run github.com/99designs/gqlgen generate\

go run ./server.go\