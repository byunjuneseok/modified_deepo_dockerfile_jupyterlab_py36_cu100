# modified_deepo_dockerfile_jupyterlab_py36_cu100
I edited some lines to use deepo(https://github.com/ufoym/deepo) container with jupyter lab. With this container, you can use deep learning frameworks based on python 3.6 and cuda 10.0 with juypter lab.

## How to use
Build the image from dockerfile and just run this command.
```
docker run --runtime=nvidia -it -p 8888:8888 --ipc=host <IMAGE> jupyter lab --no-browser --ip=0.0.0.0 --allow-root --NotebookApp.token= --notebook-dir='/root'
```
