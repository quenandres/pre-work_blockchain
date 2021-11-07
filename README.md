

## Lenguajes y herramientas para el desarrollo de blockchain
    - C++
    - Python
    - JS
    - Solidity (Smart contracts)
    - RemixIDE: Es una aplicacion web donde se pueden hacer simulaciones y compilaciones, tambien se puede comunicar con otras blockchain
    - VSC
    - Truggle Suite: Sistemas mas robustos, smart contracts con mas dependencias.
    - HyperLedger: Entendimiento de blockchain, permite entender como es el funcionamiento de los nodos

# Solidity
Lenguaje de programación mas popular, diseñado para interactuar con la EVM(Ethereum virtual machine). 
* https://ethereum.org/
* https://solidity-by-example.org/
* https://openzeppelin.com/contracts/
* https://cryptozombies.io/es/ (Juego)

# Uso de wallets: Metamask
Se puede descargar en el telefono, pero tambien existen extensiones para el explorador

# Ropsten y Rinkeby
Ambas son testnet de las mas utilizadas, tambien se pueden tener redes locales.
- ropsten ethereum faucet (Para pedir eth gratuitos para moverlos en la red de prueba)

# RemixIDE (Integrated development environment)
Es la opcion ideal para comenzar con solidity

# Truffle Suite
Es un entorno de desarrollo que facilita la creacion de apps basadas en tecnologias blockchain, permite compilar, deplegar y desarrollar frontend

 - Truffle
 - Ganache: Brinda la opcion de tener una blockchain para desplegar los contratos inteligentes.
 - Drizzle: Coleccion de librerias para frontend, que facilita la creacion de aplicaciones, se instala dentro de la carpeta 
 ``` npm install --save @drizzle/store```
 
 ### Crear un nuevo proyecto
 ```truffle init```

 ---
 - Carpetas
    - contracts: Se deben crear los contratos de nuestro proyecto (Solidity)
    - migrations: Se escriben los scripts para desplegar los contratos (JS)
    - test: Para nuestra pruebas al codigo (JS)
    - truffle-config.js : Archivo de configuracion (JS)

---------------------------

| Step | Description | command |
|------|-------------|---------|
| 1    |truffle console --network development| Se conecta a la red de development |
| 2    |web3.eth.getBlock(0) |Nos despliega el estado del bloque 0
| 3    |Se compilan los contratos |compile
| 4    |Se despliegan |migrate
| 5    |const instance = await HelloBlockchain.deployed()| Se instancia la funcion
| 6    |instance.sayHi() O instance.sayHi.call()| Se ejecuta la función


## HARDHAT
>Es una herramienta para desarrollar localmente en solidity, permite hacer test y desplegar, brinda una red de prueba llamada hardhat network, con mejoras para descubrir errores en contratos inteligentes.
Los proyectos de Hardhat, son proyectos de NPM con el paquete Hardhat instalado que se ayuda de otros plugins para incrementar sus funcionalidades.


- Cursos: Dapps aplicaciones decentralizadas y web3

|Command|Description|
|-------|-------|
|npm install --save-dev hardhat|Instala hardhat|
|npx hardhat|comprueba instalacion|
| npm i @nomiclabs/hardhat-waffle | Instalaciones |
  npm install --save-dev "@nomiclabs/hardhat-ethers@^2.0.0" "ethers@^5.0.0" "ethereum-waffle@^3.2.0"| Instalaciones |
| npx hardhat accounts | Muestra todas las cuentas que tenemos en la red de prueba |
| npx hardhat compile | Compila los contratos |
|npx hardhat run script/sample-script.js|Se despliega el contrato en la red local con el archivo ```script/sample-script.js``` Muestra mensaje Hello, Hardhat y muestra la direccion del contrato|

>Algo poderoso es la capacidad de hacer un fork de la main net de ethereum, asi que podra simular como se comportaran los contratos en la main net con la red local, ademas permite interactuar con protocolos ya desplegados. 
*Documentacion* [Hardhat](https://www.hardhat.org)


## Web3.js
>Es una coleccion de librerias que te permite interactuar de manera local o remote con tu nodo de Ethereum utilizando el protocolo HTTP, IPC o WebSocket.
Desde RemixIDE se pueden encontrar los archivos de ejemplos de ejecución de Web3.js
- [web3.js](https://web3js.readthedocs.io/en/v1.5.2/)
- [web3 github](https://github.com/ChainSafe/web3.js)

