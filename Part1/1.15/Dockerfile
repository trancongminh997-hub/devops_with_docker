FROM  python:3
WORKDIR /app
RUN apt-get update -y
RUN apt-get install -y git
RUN apt-get install -y curl
RUN git clone https://github.com/trancongminh997-hub/de_homeworks.git .
RUN pip install -r requirements.txt
CMD python flask_sorting_service.py
EXPOSE 5000
