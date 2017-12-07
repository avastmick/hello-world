FROM fsharp

# Example Docker file to compile assets in a container
# To build: docker build -t myapp .
# To run: docker run --rm myapp

ADD HelloWorld.fs src/
RUN cd src && fsharpc HelloWorld.fs
ENTRYPOINT ["mono", "/root/src/HelloWorld.exe"]