FROM python:3.12

RUN pip install setuptools==58.0.0
RUN pip install django==3.2

WORKDIR /home/ubuntu/Jenkins-Zero-To-Hero/python-jenkins-argocd-k8s

COPY . .

RUN python manage.py migrate
EXPOSE 8000
CMD ["python","manage.py","runserver","0.0.0.0:8000"]


