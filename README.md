# modified_deepo_dockerfile_jupyterlab_py36_cu100
I edited some lines to use deepo(https://github.com/ufoym/deepo) container with jupyter lab.

## How to use
```
docker run --runtime=nvidia -it -p 8888:8888 --ipc=host 152f05546aa4 jupyter lab --no-browser --ip=0.0.0.0 --allow-root --NotebookApp.token= --notebook-dir='/root'
```
> Just run this command.
