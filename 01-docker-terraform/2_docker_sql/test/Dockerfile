FROM python:3.9

RUN pip install pandas
#RUN pip install pandas sqlalchemy psycopg2

WORKDIR /app
COPY pipeline.py pipeline.py 

ENTRYPOINT [ "python", "pipeline.py" ]


   #docker needs full path
# sudo docker run -it \
#     -e POSTGRES_USER="root" \
#     -e POSTGRES_PASSWORD="root" \
#     -e POSTGRES_DB="ny_taxi" \
#     -v ${pwd}/ny_taxi_postgres_data:/var/lib/postgresql/data \                            
#     -p 5432:5432 \
#     postgres:13

#docker run -t -e POSTGRES_USER="root"        -e POSTGRES_PASSWORD="root"      -e POSTGRES_DB="ny_taxi"     -v ./ny_taxi_postgres_data:/var/lib/postgresql/data -p 5432:5432  postgres:13