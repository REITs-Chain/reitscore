# reitscore

This Library is for bitcoin Transaction.

### Instruction 



```
// index.html

<script src="./bitcore-lib.min.js"></script>
<script src="./bitcore-mnemonic.min.js"></script>
<script>
    
var Mnemonic = require('bitcore-mnemonic');


 var utxo = {

     "txid": "c783603c32fba7d8ef6645b468b2e194d8c3c06169f3a33326d5863661ca928f",

     "vout": 11,

     "address": "1Po5H7YTa5hxRydP3SpaxqiTcmremacgZ6",

     "scriptPubKey": "76a914fa0978f06fd761dc30ac71c05cf38767df99552b88ac",

     "amount": 23,

     "assetType": 0

 }

 var T = new Mnemonic.bitcore.Transaction()
     .from(utxo)
     .to("15rtjeTJJ2hL83cGmNQRRNS4Uamq2bKcSo", 5,0)
     .change('1Po5H7YTa5hxRydP3SpaxqiTcmremacgZ6',0)
     .sign("43f0380f66ecbc7ed6bb276ccbf89585e0bfd5d1c11874b5f6b395decb2090c6");

 console.debug(T.toString());


</script>




```

