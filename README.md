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
Veri seti  DataSet_upload rar dosyaları birleştirilerek elde edilebilir.

Bu veri seti için Elipmoc'un sonuçları her bir akıllı sözleşme için elde edilerek veri tabanına yazılmıştır. 

Elipmoc'un iyileştirilmesi için ilk olarak skeleton elde edilmesi için: https://github.com/gsalzer/ethutils/tree/main/doc/skeleton
kaynağı kullanılabilir.

Ardından gereksiz belleğe yazma işlemlerini kaldıran https://github.com/costa-group/EthIR/tree/master işlemi uygulanabilir. 

Veri setinde bu iki işlem uygulanarak elde edilen bayt kodları için Elipmoc tekrar çalıştırılarak sonuçları çıkarılmıştır.
