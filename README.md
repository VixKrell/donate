If you enjoy my tools and want to support me, you can donate below.

<br>

**Bitcoin (BTC):** <br>
<button onclick="copy('btc', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0; margin-right:-5px;" title="Copy Address">📋</button><code id="btc">bc1qzthdgzhdjmqgan5n9c3dp5g3m24sqv30unzxjn</code> 

<details>
  <summary>Show Bitcoin QR Code</summary>
  <br>
  <img src="btc.png" width="250" alt="Bitcoin QR">
</details>

<br>

**Ethereum (ETH):** <br>
<button onclick="copy('eth', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0; margin-right:-5px;" title="Copy Address">📋</button><code id="eth">0xda1c45125c3148bef77922225da5936d7777ca0e</code> 

<details>
  <summary>Show Ethereum QR Code</summary>
  <br>
  <img src="eth.png" width="250" alt="Ethereum QR">
</details>

<br>

**XRP:** (Tag not required. If forced, use 0) <br>
<button onclick="copy('xrp', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0; margin-right:-5px;" title="Copy Address">📋</button><code id="xrp">rN3KXnyiZvNFTUkY1Yry5xrx3nyNTMjPPo</code> 

<details>
  <summary>Show XRP QR Code</summary>
  <br>
  <img src="xrp.png" width="250" alt="XRP QR">
</details>

<br>

**Monero (XMR):** <br>
<button onclick="copy('xmr', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0; margin-right:-5px;" title="Copy Address">📋</button><code id="xmr">85WaFLhsc6QFR747nCLtmMes7Qhfwd1gkauBxdep3jpGS2KXj7res17LV5myFNR9XNLGeBEeWmmBpibDEVWG3zpWA1xiQzK</code> 

<details>
  <summary>Show Monero QR Code</summary>
  <br>
  <img src="xmr.png" width="250" alt="Monero QR">
</details>

<br>

**Litecoin (LTC):** <br>
<button onclick="copy('ltc', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0; margin-right:-5px;" title="Copy Address">📋</button><code id="ltc">ltc1qv2etczlwqklcvkh9axt5uruh0r2qjj45s978pp</code> 

<details>
  <summary>Show Litecoin QR Code</summary>
  <br>
  <img src="ltc.png" width="250" alt="Litecoin QR">
</details>

<br>

*Thanks for your support!* [vixkrell@gmail.com](mailto:vixkrell@gmail.com)

<script>
function copy(id, btn) {
  var txt = document.getElementById(id).innerText;
  
  navigator.clipboard.writeText(txt).then(function() {
    
    // Change icon to checkmark
    btn.innerText = "✅";
    
    // Revert back after 2 seconds
    setTimeout(function() {
      btn.innerText = "📋";
    }, 2000);
  }, function(err) {
    console.error('Could not copy text: ', err);
  });
}
</script>
