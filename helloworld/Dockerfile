# cd directory
# docker build -t my-server .
# docker run my-server .
# export PROJECT_ID="$(gcloud config get-value project -q)"
# docker build -t gcr.io/${PROJECT_ID}/hello-app:v1 .
# docker images
# gcloud auth configure-docker
# docker push gcr.io/${PROJECT_ID}/hello-app:v1
# docker run --rm -p 8080:8080 gcr.io/${PROJECT_ID}/hello-app:v1


FROM python:3
ADD server.py /
RUN pip3 install six
ENV PORT 8000
CMD [ "python3", "./server.py" ]
