FROM node:14.17.3

# In the docker image, make the working directory the frontend directory. (If it doesn't exist it will create a directory called 'frontend')
WORKDIR /frontend

# copy contents of the folder where Dockerfile is to the working directory (frontend) of the docker image
COPY . .

# run command npm install
RUN npm install

# create react app production version
RUN npm run build

# expose on port 3000
EXPOSE 3000

# run the build
CMD [ "npx", "serve", "build" ]