If you enjoy my tools and want to support me, you can donate below.

<br>

**Bitcoin (BTC):**
<div style="display:flex; align-items:center; gap:2px; margin-top:-12px; margin-bottom:7px;">
  <button onclick="copy('btc', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0;" title="Copy Address">📋</button>
  <code id="btc" style="word-break: break-all;">bc1qzthdgzhdjmqgan5n9c3dp5g3m24sqv30unzxjn</code>
</div>

<details>
  <summary>Show Bitcoin QR Code</summary>
  <br>
  <img src="btc.png" width="250" alt="Bitcoin QR">
</details>

<div style="height:1px; background-color:#cccccc; margin:20px 0;"></div>

**Ethereum (ETH):**
<div style="display:flex; align-items:center; gap:2px; margin-top:-12px; margin-bottom:7px;">
  <button onclick="copy('eth', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0;" title="Copy Address">📋</button>
  <code id="eth" style="word-break: break-all;">0xda1c45125c3148bef77922225da5936d7777ca0e</code>
</div>

<details>
  <summary>Show Ethereum QR Code</summary>
  <br>
  <img src="eth.png" width="250" alt="Ethereum QR">
</details>

<div style="height:1px; background-color:#cccccc; margin:20px 0;"></div>

**XRP:** (Tag not required. If forced, use 0)
<div style="display:flex; align-items:center; gap:2px; margin-top:-12px; margin-bottom:7px;">
  <button onclick="copy('xrp', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0;" title="Copy Address">📋</button>
  <code id="xrp" style="word-break: break-all;">rN3KXnyiZvNFTUkY1Yry5xrx3nyNTMjPPo</code>
</div>

<details>
  <summary>Show XRP QR Code</summary>
  <br>
  <img src="xrp.png" width="250" alt="XRP QR">
</details>

<div style="height:1px; background-color:#cccccc; margin:20px 0;"></div>

**Monero (XMR):**
<div style="display:flex; align-items:center; gap:2px; margin-top:-12px; margin-bottom:7px;">
  <button onclick="copy('xmr', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0;" title="Copy Address">📋</button>
  <code id="xmr" style="word-break: break-all;">85WaFLhsc6QFR747nCLtmMes7Qhfwd1gkauBxdep3jpGS2KXj7res17LV5myFNR9XNLGeBEeWmmBpibDEVWG3zpWA1xiQzK</code>
</div>

<details>
  <summary>Show Monero QR Code</summary>
  <br>
  <img src="xmr.png" width="250" alt="Monero QR">
</details>

<div style="height:1px; background-color:#cccccc; margin:20px 0;"></div>

**Litecoin (LTC):**
<div style="display:flex; align-items:center; gap:2px; margin-top:-12px; margin-bottom:7px;">
  <button onclick="copy('ltc', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0;" title="Copy Address">📋</button>
  <code id="ltc" style="word-break: break-all;">ltc1qv2etczlwqklcvkh9axt5uruh0r2qjj45s978pp</code>
</div>

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
