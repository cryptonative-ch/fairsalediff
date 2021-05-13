

```
# bash README.md
git clone git@github.com:cryptonative-ch/fairsalediff.git
cp README.md fairsalediff/
cd fairsalediff
git add README.md
git commit -a -m ' This README'
wget https://raw.githubusercontent.com/gnosis/ido-contracts/df90c25067fa940d9e92e20e4b0b54164e8dd8a3/contracts/EasyAuction.sol
wget https://raw.githubusercontent.com/gnosis/ido-contracts/df90c25067fa940d9e92e20e4b0b54164e8dd8a3/contracts/EasyAuction.sol -O FairSale.sol
git add EasyAuction.sol FairSale.sol
git commit -a -m ' Audited Version from Gnosis: https://raw.githubusercontent.com/gnosis/ido-contracts/df90c25067fa940d9e92e20e4b0b54164e8dd8a3/contracts/EasyAuction.sol '
wget https://raw.githubusercontent.com/cryptonative-ch/mesa-smartcontracts/d41eac1ec4a80f7decf24b5b88e3169de16210b1/contracts/sales/FairSale.sol -O FairSale.sol
git commit -a  -m ' Latest Mesa Version https://raw.githubusercontent.com/cryptonative-ch/mesa-smartcontracts/d41eac1ec4a80f7decf24b5b88e3169de16210b1/contracts/sales/FairSale.sol'
git push
# git --no-pager diff --no-index --word-diff  --patience EasyAuction.sol FairSale.sol > FairSale.sol.diff
```

Look here: https://github.com/cryptonative-ch/fairsalediff/commit/b9bdf33c3513b80778014d8c8fdb02e1e6ccbd2c