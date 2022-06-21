K8s ingress的http、https测试访问
使用到的镜像为tomcat:8.5.34-jre8-alpine

create ssl.crt <Command>
openssl genrsa -out tls.key 2048
openssl req -new -x509 -key tls.key -out tls.crt -subj /C=CN/ST=Beijing/L=Beijing/O=DevOps/CN=tomcat.kris.com
