FROM node:10

EXPOSE 9545

WORKDIR /app

COPY . .

#RUN npm install

RUN npm uninstall -g truffle

RUN npm install -g truffle@5.0.2

RUN cd app
# install packages
RUN cd app && npm install --save  openzeppelin-solidity@2.3
RUN cd app && npm install --save  truffle-hdwallet-provider@1.0.17
RUN cd app && npm install webpack-dev-server -g
RUN cd app && npm install web3


# Remove the node_modules  
# remove packages
RUN cd app && rm -rf node_modules

# clean cache
#RUN npm cache clean
RUN cd app && npm install --cache /tmp/empty-cache
RUN cd app && rm package-lock.json
# initialize npm (you can accept defaults)
RUN cd app && npm init -y
# install all modules listed as dependencies in package.json
RUN cd app && npm install


#CMD ["node", "index.js"]