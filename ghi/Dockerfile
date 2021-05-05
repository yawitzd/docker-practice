FROM rackspacedot/python37

# Create app directory
WORKDIR /usr/src/ghi

# Bundle app source
COPY . .

EXPOSE 8080
CMD [ "python3", "server.py" ]

# To run container:
# docker build . -t ghi
# docker run -e APP_URL=http://localhost:8081/api/items -e AUTH_URL=http://localhost:8082/api/login  -p 8080:80  -d ghi