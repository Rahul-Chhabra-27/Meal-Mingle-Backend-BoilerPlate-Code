proto-generate:
	protoc -I ./proto \
	--go_out ./proto --go_opt paths=source_relative \
	--go-grpc_out ./proto --go-grpc_opt paths=source_relative \
	--grpc-gateway_out ./proto --grpc-gateway_opt paths=source_relative \
	./proto/order/order.proto

environment-variable:
	export PATH=$PATH:$(go env GOPATH)/bin

.PHONY: install

install:
	go get -u gorm.io/gorm
	go get -u gorm.io/driver/mysql
	go get -u google.golang.org/grpc
	go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@v1.2
	go install google.golang.org/protobuf/cmd/protoc-gen-go@v1.28
	go get -u golang.org/x/crypto/bcrypt 
	go get github.com/grpc-ecosystem/grpc-gateway/v2/protoc-gen-grpc-gateway
	go get github.com/grpc-ecosystem/grpc-gateway/v2/runtime
	go get github.com/joho/godotenv
	go get github.com/dgrijalva/jwt-go
	go get -u go.uber.org/zap
	go get github.com/gorilla/handlers