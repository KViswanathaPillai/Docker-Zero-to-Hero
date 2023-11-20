from centos

workdir /app

copy requirements.txt /app
copy devops /app

run yum-get update && \
    yum-get install -y python3 python3-pip && \
    pip install -r requirements.txt && \
    cd devops

entrypoint ["python3"]
cmd ["manage.py", "runserver", "0.0.0.0:8000"]




