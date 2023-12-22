FROM node:10


#Echo the argument to check passed argument loaded here correctly
RUN echo "Argument port is : 3000"

# Create app directory
WORKDIR /usr/src/app

#COPY . .
COPY package.json /usr/src/app/package.json
#COPY package-lock.json /usr/src/app/package-lock.json

# Install app dependencies
RUN npm install

COPY . /usr/src/app

EXPOSE 3000

CMD npm run dev


