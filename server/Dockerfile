FROM gcc:4.9
RUN mkdir /usr/src/myapp
COPY . /usr/src/myapp
WORKDIR /usr/src/myapp
RUN gcc -o server server.c
CMD ["./server", "9999"]




