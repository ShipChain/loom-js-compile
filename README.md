## Compilation errors with loom-js

Run `yarn` to install typescript and loom-js.

Run `yarn compile` to see compilation errors:

```
➜  loom-js-compile git:(master) ✗ yarn compile
yarn run v1.17.3
$ rm -rf ./dist && tsc
node_modules/loom-js/dist/dpos-user.d.ts:7:64 - error TS2307: Cannot find module './mainnet-contracts/EthereumGatewayV2'.

7 import { EthereumGatewayV2 as EthereumGatewayV2Contract } from './mainnet-contracts/EthereumGatewayV2';
                                                                 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

node_modules/loom-js/dist/dpos-user.d.ts:8:23 - error TS2307: Cannot find module './mainnet-contracts/ERC20'.

8 import { ERC20 } from './mainnet-contracts/ERC20';
                        ~~~~~~~~~~~~~~~~~~~~~~~~~~~

node_modules/loom-js/dist/dpos-user.d.ts:9:66 - error TS2307: Cannot find module './mainnet-contracts/ValidatorManagerV2'.

9 import { ValidatorManagerV2 as ValidatorManagerV2Contract } from './mainnet-contracts/ValidatorManagerV2';
                                                                   ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

node_modules/loom-js/dist/ethereum-gateways.d.ts:4:38 - error TS2307: Cannot find module './mainnet-contracts'.

4 import { TransactionOverrides } from './mainnet-contracts';
                                       ~~~~~~~~~~~~~~~~~~~~~

node_modules/loom-js/dist/ethereum-gateways.d.ts:5:66 - error TS2307: Cannot find module './mainnet-contracts/ValidatorManagerV2'.

5 import { ValidatorManagerV2 as ValidatorManagerContractV2 } from './mainnet-contracts/ValidatorManagerV2';
                                                                   ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

node_modules/loom-js/dist/ethereum-gateways.d.ts:6:64 - error TS2307: Cannot find module './mainnet-contracts/EthereumGatewayV1'.

6 import { EthereumGatewayV1 as EthereumGatewayV1Contract } from './mainnet-contracts/EthereumGatewayV1';
                                                                 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

node_modules/loom-js/dist/ethereum-gateways.d.ts:7:64 - error TS2307: Cannot find module './mainnet-contracts/EthereumGatewayV2'.

7 import { EthereumGatewayV2 as EthereumGatewayV2Contract } from './mainnet-contracts/EthereumGatewayV2';
                                                                 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

node_modules/loom-js/dist/ethereum-gateways.d.ts:38:14 - error TS2416: Property 'version' in type 'EthereumGatewayV1' is not assignable to the same property in base type 'IEthereumGateway'.
  Type 'number' is not assignable to type 'GatewayVersion'.

38     readonly version: number;
                ~~~~~~~

node_modules/loom-js/dist/ethereum-gateways.d.ts:47:14 - error TS2416: Property 'version' in type 'EthereumGatewayV2' is not assignable to the same property in base type 'IEthereumGateway'.
  Type 'number' is not assignable to type 'GatewayVersion'.

47     readonly version: number;
                ~~~~~~~

node_modules/loom-js/dist/gateway-user.d.ts:6:23 - error TS2307: Cannot find module './mainnet-contracts/ERC20'.

6 import { ERC20 } from './mainnet-contracts/ERC20';
                        ~~~~~~~~~~~~~~~~~~~~~~~~~~~

node_modules/loom-js/dist/gateway-user.d.ts:7:64 - error TS2307: Cannot find module './mainnet-contracts/EthereumGatewayV2'.

7 import { EthereumGatewayV2 as EthereumGatewayV2Contract } from './mainnet-contracts/EthereumGatewayV2';
                                                                 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

node_modules/loom-js/dist/gateway-user.d.ts:8:66 - error TS2307: Cannot find module './mainnet-contracts/ValidatorManagerV2'.

8 import { ValidatorManagerV2 as ValidatorManagerContractV2 } from './mainnet-contracts/ValidatorManagerV2';
                                                                   ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Found 12 errors.

error Command failed with exit code 2.
info Visit https://yarnpkg.com/en/docs/cli/run for documentation about this command.
```
