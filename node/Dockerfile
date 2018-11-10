FROM ubuntu:latest

RUN apt-get update
RUN apt-get install software-properties-common -y
RUN add-apt-repository -y ppa:ethereum/ethereum
RUN apt-get update
RUN apt-get install ethereum -y

CMD geth --port 30303 --rpc --rpcport 8544 --rpcaddr 0.0.0.0 --rpccorsdomain "*" --rpcvhosts "*" --rpcapi "eth,web3,net" --syncmode "full" --gcmode "archive"
