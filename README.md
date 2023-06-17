# GOLANG_PROJECTS_Protobuf_Golang-


Linux/MacOS
make all
*all is a Makefile rule - check the other rules

Windows - Chocolatey
choco install make
make all
*all is a Makefile rule - check the other rules

Windows - Without Chocolatey
protoc -Igreet/proto --go_opt=module=github.com/Clement-Jean/grpc-go-course --go_out=. --go-grpc_opt=module=github.com/Clement-Jean/grpc-go-course --go-grpc_out=. greet/proto/*.proto

protoc -Icalculator/proto --go_opt=module=github.com/Clement-Jean/grpc-go-course --go_out=. --go-grpc_opt=module=github.com/Clement-Jean/grpc-go-course --go-grpc_out=. calculator/proto/*.proto

protoc -Iblog/proto --go_opt=module=github.com/Clement-Jean/grpc-go-course --go_out=. --go-grpc_opt=module=github.com/Clement-Jean/grpc-go-course --go-grpc_out=. blog/proto/*.proto

go build -o bin/greet/server.exe ./greet/server
go build -o bin/greet/client.exe ./greet/client

go build -o bin/calculator/server.exe ./calculator/server
go build -o bin/calculator/client.exe ./calculator/client

go build -o bin/blog/server.exe ./blog/server
go build -o bin/blog/client.exe ./blog/client

Makefile
For more information about what are the rules defined in the Makefile, please type:

make help
