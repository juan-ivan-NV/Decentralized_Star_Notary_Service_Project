# Decentralized Star Notary Service Project

Projec to register, sale and buy stars on a blockchain app


# How to use it?

## Run the app in docker

Download the repo and type ...

Build the image <code>docker build -t testnetdapp . </code>

<center>
<img src='images/image.png'/>
<figcaption>Docker image</figcaption></center>
<br/>

Run the image and app <code>docker run -t -d -p 9545:9545 -p 8080:8080 testnetdapp </code>

<center>
<img src='images/container.png'/>
<figcaption>Container</figcaption></center>
<br/>

List the running containers <code>docker ps </code>

Enter the container terminal <code>docker exec -it [container id] bash </code>

<center>
<img src='images/terminal.png'/>
<figcaption>Container terminal</figcaption></center>
<br/>

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
docker run -t -d -p 9545:9545 -p 8080:8080 testnetdapp bash
docker run -i -t -d -p 9545:9545 -p 8080:8080 testnetdapp bash
docker run -i -t testnetdapp bash

docker exec -it [container id] bash

docker inspect [containername]

http://localhost:8080/


<code>// name: Is a short name to your token </code><br/>
<code>string public name = "Alfa Tauri Token"; </code><br/>
<code>// symbol: Is a short string like 'USD' -> 'American Dollar' </code><br/>
<code>string public symbol = "a Tau"; </code>


Transaction example
https://goerli.etherscan.io/tx/0x33379cc3a9632ee63c4929aca9ef25b5b384455903a8033a0bbeb72c961af096