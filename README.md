# Liquidity Pool (DEV)




### 1. Smart contracts - `contract/` 
Smart contract are implemented with **Solidity** and require the **version 0.8.0** of the compiler. 
1. `ERC20Token.sol`
Contrato básico de token ERC20 utilizado por los proveedores de liquidez y el comerciante para interactuar con Dex

2. `DEX.sol`
Mercado descentralizado donde se puede crear un nuevo fondo de liquidez.

3. `LiquidityPool.sol`
Archivo principal del proyecto. El contrato de fondo de liquidez representa un fondo de liquidez TokenA/TokenB.
Los proveedores de liquidez pueden proporcionar liquidez al grupo. Luego recibirán tokens de proveedor de liquidez (LPTokens), que representan la parte del fondo de liquidez que poseen.
Cuando retiren la liquidez que proporcionaron, se les reembolsará con la misma cantidad de token que depositaron + las tarifas cobradas con todas las operaciones (0,3% en cada operación).
### 2. Pruebas - `test/`
Pruebas unitarias para los contratos `DEX.sol`, `LiquidityPool.sol` y `ERC20Token.sol`.

## ¿Como correr?
### Stack
* NodeJS (v >= 12.0.0)
* npm 
* Hardhat 
* Solidity (v0.8.0)

### Install dependencies and run tests
1. ` npm install`
2. `npx hardhat compile` (to compile contracts and generate artifacts)
3. `npx hardhat test` (to run existing unit tests)  

