# openfaas-workshop
Đồ án Chuyên ngành

- Tên tiếng Việt: Nghiên cứu thực nghiệm về triển khai và đánh giá nền tảng Serverless mã nguồn mở OpenFaaS trên Kubernetes

- Tên tiếng Anh: An empirical study on deployment and evaluation of OpenFaaS Serverless open source platform on Kubernetes

## Phần mềm/Phần cứng sử dụng

OS: Ubuntu Desktop 20.04 LTS
- CPU: 2 cores
- Memory: 4GB
- Hard disk: 20 GB

Application:
- Docker
- Kubernetes
- k3d, arkade (install OpenFaaS)

## Tổng quan bài Lab

### [Lab 1 - Prepare for OpenFaaS](/Lab1)
- Install pre-requisites
- Set up a single-node cluster with Docker Swarm or Kubernetes
- Docker Hub account
- OpenFaaS CLI
- Deploy OpenFaaS

### [Lab 2 - Test things out](/Lab2)
- Use the UI Portal
- Deploy via the Function Store
- Learn about the CLI
- Find metrics with Prometheus

### [Lab 3 - Introduction to Functions](/Lab3)
- Scaffold or generate a new function
- Build the astronaut-finder function
- Add dependencies with pip
- Troubleshooting: find the container's logs
- Troubleshooting: verbose output with write_debug
- Use custom and third-party language templates
- Discover community templates using the Template Store

### [Lab 4 - Go deeper with functions](/Lab4)
- Inject configuration through environmental variables
- At deployment using yaml
- Dynamically using HTTP context - querystring / headers etc
- Security: read-only filesystems
- Making use of logging
- Create Workflows
- Chaining functions on the client-side
- Call one function from another

### [Lab 5 - Create a GitHub bot](/Lab5)
- Build issue-bot - an auto-responder for GitHub Issues
- Get a GitHub account
- Set up a tunnel with ngrok
- Create an webhook receiver issue-bot
- Receive webhooks from GitHub
- Deploy SentimentAnalysis function
- Apply labels via the GitHub API
- Complete the function

### [Lab 6 - HTML for your functions](/Lab6)
- Generate and return basic HTML from a function
- Read and return a static HTML file from disk
- Collaborate with other functions

### [Lab 7 - Asynchronous Functions](/Lab7)
- Call a function synchronously vs asynchronously
- View the queue-worker's logs
- Use an X-Callback-Url with requestbin and ngrok

### [Lab 8 - Advanced Feature - Timeouts](/Lab8)
- Adjust timeouts with read_timeout
- Accommodate longer running functions

### [Lab 9 - Advanced Feature - Auto-scaling](/Lab9)
- See auto-scaling in action
- Some insights on min and max replicas
- Discover and visit local Prometheus
- Execute and Prometheus query
- Invoke a function using curl
- Observe auto-scaling kicking in

### [Lab 10 - Advanced Feature - Secrets](/Lab10)
- Adapt issue-bot to use a secret
- Create a Swarm secret
- Access the secret within the function

### [Lab 11 - Advanced feature - Trust with HMAC](/Lab11)
- Apply trust to functions using HMAC

## Các công cụ sử dụng để đánh giá hiệu năng

- Pigo: https://github.com/tri105/faas-pigo
- Client: https://github.com/tri105/mec-client
- Hey: https://github.com/rakyll/hey

## Nguồn tham khảo

- https://github.com/openfaas/workshop

