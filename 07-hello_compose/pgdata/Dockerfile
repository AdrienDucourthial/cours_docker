FROM postgres
ENV POSTGRES_USER doc
ENV POSTGRES_PASSWORD doc
ENV POSTGRES_DB doc
COPY db.sql /docker-entrypoint-initdb.d/
