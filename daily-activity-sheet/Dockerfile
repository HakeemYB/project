FROM node:19.3.0
WORKDIR /daily-activity-sheet
ADD package*.json ./
RUN npm install
ADD app.js ./
CMD [ "node", "app.js"]
