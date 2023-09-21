# tkdnn-container

#Dockerfile2 : r32.4.4
sudo docker build -t tkdnn:build -f Dockerfile2 .

#Dockerfile6 : R32.3.1
sudo docker build -t tkdnn:build -f Dockerfile6 .

#run the container
sudo docker run --rm -it --runtime=nvidia -v $HOME/test/tkDNN:/home/$(id -un)/tkDNN  tkdnn:build
