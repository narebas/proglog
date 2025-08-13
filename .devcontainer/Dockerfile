FROM mcr.microsoft.com/devcontainers/go:1-1.24-bookworm

USER vscode

RUN sudo apt-get update \
  && sudo apt-get upgrade -y \
  && sudo apt-get install -y protobuf-compiler \
  && go install google.golang.org/protobuf/cmd/protoc-gen-go@latest \
  && go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@latest

RUN go install github.com/go-task/task/v3/cmd/task@latest
