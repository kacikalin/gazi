# Gazi
In this project, the dataset, the criteria and the evaluation of the results will be used for the comparison of smart contract decompile tools.

To obtain run-time bytecode:

```
urlmainnet=""https://mainnet.infura.io/v3/....";

web3=Web3(Web3.HTTPProvider(urlmainnet));

address="0xab2323..";

byteCode=web3.eth.get_code(web3.toChecksumAddress(address));

print(byteCode);

print(byteCode.hex());
```
The dataset can be obtained by the DataSet_upload rar files.

For this dataset, the results of Elipmoc were obtained for each smart contract and written to the database. 

Elipmoc rar files contains Elipmoc's results.
