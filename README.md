# DAPP DE VOTACIÓN MEDIANTE TOKENS

Esta aplicación consta de un smart contract que emite tokens, y lleva un registro de votos a canditatos de una organización. 

Quienes desean participar debe comprar tokens con ethers y utilizarlos para votar a los candidatos listados mediante una interface web. 

Ofrece información sobre los votos acumulados por cada candidato y permite consultar los votos realizados por cada participante. 


```sh
$ git clone https://github.com/maginkgo/Voting_tokens_dapp.git
$ cd Voting_tokens_dapp
$ npm install -g truffle
$ npm install -g webpack
```

## Editar migrations/2_deploy_contracts.js
Reemplazar valores ('Bob', 'Alice', 'Jose', 'etc')


> var Voting = artifacts.require("./Voting.sol");
> module.exports = function(deployer) {
> 	deployer.deploy(Voting, 10000, web3.toWei('0.01', 'ether'), ['Bob', 'Alice', 'Jose']);
> };


## Ejecutar testrpc

## Compilar y deployar
```sh
$truffle compile
$truffle migrate
```

## Ejecutar interface web
```sh
$npm run dev
```

