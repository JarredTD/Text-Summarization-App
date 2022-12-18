Commands to run the container:

1. Build the image (if you are not downloading it)
```
docker build <directory with the dockerfile>
docker build -t clrhoades1/shap-notebook-container:latest .
```

2. Create the container
```
docker run -p 8888:8888 clrhoades1/shap-notebook-container

# Does not work
docker run -it --rm -p 10000:8888 -v "${PWD}/Notebooks":/home/jovyan/notebooks -v "${PWD}/Data":/home/jovyan/data jupyter/datascience-notebook:latest

```#   S H A P - C o n t a i n e r i z a t i o n  
 