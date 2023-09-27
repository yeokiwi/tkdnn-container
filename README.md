# tkdnn-container

#Dockerfile2 : r32.4.4
sudo docker build -t tkdnn:build -f Dockerfile2 .

#Dockerfile6 : R32.3.1
sudo docker build -t tkdnn:build -f Dockerfile6 .

#create package directory to put files into /usr
/packages/usr/lib/aarch64-linux-gnu/tegra/ 
and
/packages/usr/lib/aarch64-linux-gnu/libcuda.so

#run the container
sudo docker run --rm -it --runtime=nvidia -v $HOME/test/tkDNN:/home/$(id -un)/tkDNN  tkdnn:build
