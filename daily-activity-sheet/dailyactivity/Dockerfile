# pull official base image
FROM node:19.3.0

# set working directory
WORKDIR /dailyactivity

# add `/dailyactivity/node_modules/.bin` to $PATH
ENV PATH /dailyactivity/node_modules/.bin:$PATH

# install app dependencies
COPY package.json ./
COPY package-lock.json ./
RUN npm install --silent
RUN npm install react-scripts@5.0.1 -g

# add app
COPY . ./

# start app
CMD ["npm", "start"]