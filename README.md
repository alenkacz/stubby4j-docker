# stubby4j-docker
Dockerfile for stubby4j https://github.com/azagniotov/stubby4j

In order to use it in your application you need to create your own image based on this image. Example of such dockerfile is here:

FROM alenkacz/stubby4j-docker

ADD config.txt /home/your_application/

CMD ["--data", "/home/your_application/config.txt", "--location", "0.0.0.0"]