# docker run -d -p 8888:8888 -v ~/talks:/home/jovyan jupyter/datascience-notebook start-notebook.sh --NotebookApp.token=''
FROM jupyter/datascience-notebook
MAINTAINER Brendan Ryan

# copy all notebooks to the directory that the base image points to
COPY notebooks/  /home/jovyan/

# remove this jank directory which the base image points to
RUN rm -rf /home/jovyan/work

CMD ["start-notebook.sh", "--NotebookApp.token=''"]
