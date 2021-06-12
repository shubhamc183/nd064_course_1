FROM golang:alpine
LABEL maintainer="shubhamc183@gmail.com"
ARG APP_HOME="/go/src/app"
RUN mkdir -p ${APP_HOME}
WORKDIR ${APP_HOME}
COPY main.go ${APP_HOME}
RUN go mod init
RUN go build -o helloworld
EXPOSE 6111
CMD ["./helloworld" ]

# To Build the Docker image
# export TAG=1.0.0
# docker build -t shubhamc183/go-helloworld:$TAG .
# docker push shubhamc183/go-helloworld:$TAG