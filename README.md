
Docs: https://docs.binance.org/smart-chain/developer/upgrade/proxy.html

Deployed Contracts :

Logic 1 Contract (Implementation 1):
https://testnet.bscscan.com/address/0xb11ac4c6f508919aec27506b434dc7db55b4a75d

Logic 2 Contract (Implementation 2):
https://testnet.bscscan.com/address/0xc995e67e54a557ba46795440dbd08eb524412a5b

BEP20TokenFactory:
https://testnet.bscscan.com/address/0x42163f785e1d8021bff1b7f70e1790a1fded3fba

BEP20UpgradableProxy:
https://testnet.bscscan.com/address/0x352d3feb3d01292ddd9c45f992d6f7ba557bc6ab


Contracts are flattened and compiled as a single file (imports are included in the same file)
Owner can mint more tokens. Proxy admin can switch between logic contracts.
Avoid keeping same account address as proxy admin and token owner.
Use correct arguments for verification of contract, the one which was used while deploying.
The Logic 2 contract contains allowMinting() function which the Logic 1 contract does not have.



