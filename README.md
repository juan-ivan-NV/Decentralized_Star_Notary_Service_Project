# How to use it?

## Run the app in docker

Download the repo and type ...

Build the image <code>docker build -t testnetdapp . </code>

Run the image and app <code>docker run -p 9545:9545 testnetdapp </code>

List the running containers <code>docker ps </code>

Stop the container <code>docker stop **(first 2 container name characters) </code>

Once the app is running ...

## Start Truffle by running

#### For starting the development console

<code>truffle develop</code>

#### truffle console
#### For compiling the contract, inside the development console, run:
<code>compile</code>

#### For migrating the contract to the locally running Ethereum network, inside the development console
<code>migrate --reset</code>

#### For running unit tests the contract, inside the development console, run:
<code>test</code>


## Frontend - Once you are ready to start your frontend, run the following from the app folder:

<code>cd app</code>

<code>npm run dev</code>


docker build -t testnetdapp .
docker run -p 9545:9545 testnetdapp
docker run -i -t testnetdapp bash