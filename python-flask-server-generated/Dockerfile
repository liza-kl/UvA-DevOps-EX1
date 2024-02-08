FROM python:3.11.7

RUN mkdir -p /usr/src/app

WORKDIR /usr/src/app

COPY requirements.txt /usr/src/app/
COPY setup.py /usr/src/app/

RUN pip3 install --no-cache-dir -r requirements.txt
RUN python3 setup.py install

COPY . /usr/src/app

EXPOSE 8080

ENTRYPOINT ["python3"]

CMD ["-m", "swagger_server"]

# To access it: 
# docker run -p 8080:8080 <name-of-image>
# access via http://localhost:8080/LKLETSKO0202/tutorial/1.0.0/swagger.json
# http://localhost:8080/LKLETSKO0202/tutorial/1.0.0/ui/
