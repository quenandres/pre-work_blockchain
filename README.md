

- Lenguajes y herramientas para el desarrollo de blockchain
5/14

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

1. truffle console --network development
2. web3.eth.getBlock(0) (Nos despliega el estado del bloque 0)
3. Se compilan los contratos (compile)
4. Se despliegan (migrate)
5. const instance = await HelloBlockchain.deployed() (Se instancia la funcion)
6. instance.sayHi() || instance.sayHi.call() (Se ejecuta la función)