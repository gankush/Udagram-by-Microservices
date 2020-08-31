FROM node:12
# Create app directory
WORKDIR /usr/src/app
# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./

# ENV POSTGRES_USERNAME=udagramgoyaldev
# ENV POSTGRES_PASSWORD=udagramgoyaldev
# ENV POSTGRES_HOST=udagramgoyaldev.cpko0pkznkht.us-east-2.rds.amazonaws.com
# ENV POSTGRES_DB=postgres
# ENV AWS_BUCKET=udagram-goyal-dev
# ENV AWS_REGION=us-east-2
# ENV AWS_PROFILE=default
# ENV JWT_SECRET=hello
# ENV URL=http://localhost:8100


RUN npm ci 
# Bundle app source
COPY . .
EXPOSE 8080
CMD [ "npm", "run", "prod" ]