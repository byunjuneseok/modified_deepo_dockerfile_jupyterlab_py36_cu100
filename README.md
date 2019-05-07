# modified_deepo_dockerfile_jupyterlab_py36_cu100
I edited some lines to use deepo(https://github.com/ufoym/deepo) container with jupyter lab.

## How to use
Build the image from dockerfile and just run this command.
```
docker run --runtime=nvidia -it -p 8888:8888 --ipc=host <CONTAINER ID> jupyter lab --no-browser --ip=0.0.0.0 --allow-root --NotebookApp.token= --notebook-dir='/root'
```
