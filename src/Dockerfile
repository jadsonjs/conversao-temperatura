#
# docker build . -t jadsonjs/conversor:v1
#

# download node image
FROM node:19.4.0
# create a directory for build the application
WORKDIR /app
# copy and install dependences
COPY package*.json ./
RUN npm install

# copy another files
COPY . .

# expose the port
EXPOSE 8080

#
# docker container run -d -p 8080:8080 --name conversor jadsonjs/conversor:v1
#

# execute the node application
CMD ["node", "server.js"]

