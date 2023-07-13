# Gazi
Bu projede akıllı sözleşme decompile araçlarının karşılaştırılması için kullanılacak veri seti, kriterler ve sonuçların değerlendirilmesi bulunacaktır.

Run-time bytecode'u elde etmek için:

```
urlmainnet=""https://mainnet.infura.io/v3/....";

web3=Web3(Web3.HTTPProvider(urlmainnet));

address="0xab2323..";

byteCode=web3.eth.get_code(web3.toChecksumAddress(address));

print(byteCode);

print(byteCode.hex());
```
Veri seti için DataSet_upload rar dosyaları birleştirilebilir.
