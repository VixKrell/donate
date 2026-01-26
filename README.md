If you enjoy my tools and want to support me, you can donate below.

<br>

**Bitcoin (BTC):** <code id="btc">bc1qzthdgzhdjmqgan5n9c3dp5g3m24sqv30unzxjn</code> 
<button onclick="copy('btc', this)" style="cursor:pointer; vertical-align:middle;" title="Copy Address">
  <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="9" y="9" width="13" height="13" rx="2" ry="2"></rect><path d="M5 15H4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2h9a2 2 0 0 1 2 2v1"></path></svg>
</button>

<details>
  <summary>Show Bitcoin QR Code</summary>
  <br>
  <img src="btc.png" width="250" alt="Bitcoin QR">
</details>

<br>

**Ethereum (ETH):** <code id="eth">0xda1c45125c3148bef77922225da5936d7777ca0e</code> 
<button onclick="copy('eth', this)" style="cursor:pointer; vertical-align:middle;" title="Copy Address">
  <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="9" y="9" width="13" height="13" rx="2" ry="2"></rect><path d="M5 15H4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2h9a2 2 0 0 1 2 2v1"></path></svg>
</button>

<details>
  <summary>Show Ethereum QR Code</summary>
  <br>
  <img src="eth.png" width="250" alt="Ethereum QR">
</details>

<br>

**XRP:** (Tag not required. If forced, use 0)  
<code id="xrp">rN3KXnyiZvNFTUkY1Yry5xrx3nyNTMjPPo</code> 
<button onclick="copy('xrp', this)" style="cursor:pointer; vertical-align:middle;" title="Copy Address">
  <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="9" y="9" width="13" height="13" rx="2" ry="2"></rect><path d="M5 15H4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2h9a2 2 0 0 1 2 2v1"></path></svg>
</button>

<details>
  <summary>Show XRP QR Code</summary>
  <br>
  <img src="xrp.png" width="250" alt="XRP QR">
</details>

<br>

**Monero (XMR):** <code id="xmr">85WaFLhsc6QFR747nCLtmMes7Qhfwd1gkauBxdep3jpGS2KXj7res17LV5myFNR9XNLGeBEeWmmBpibDEVWG3zpWA1xiQzK</code> 
<button onclick="copy('xmr', this)" style="cursor:pointer; vertical-align:middle;" title="Copy Address">
  <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="9" y="9" width="13" height="13" rx="2" ry="2"></rect><path d="M5 15H4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2h9a2 2 0 0 1 2 2v1"></path></svg>
</button>

<details>
  <summary>Show Monero QR Code</summary>
  <br>
  <img src="xmr.png" width="250" alt="Monero QR">
</details>

<br>

**Litecoin (LTC):** <code id="ltc">ltc1qv2etczlwqklcvkh9axt5uruh0r2qjj45s978pp</code> 
<button onclick="copy('ltc', this)" style="cursor:pointer; vertical-align:middle;" title="Copy Address">
  <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="9" y="9" width="13" height="13" rx="2" ry="2"></rect><path d="M5 15H4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2h9a2 2 0 0 1 2 2v1"></path></svg>
</button>

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
    
    // Save the icon HTML so we can restore it later
    var originalContent = btn.innerHTML;
    
    // Change button text to "Copied!"
    btn.innerText = "Copied!";
    
    // Revert back to the icon after 2 seconds
    setTimeout(function() {
      btn.innerHTML = originalContent;
    }, 2000);
  }, function(err) {
    console.error('Could not copy text: ', err);
  });
}
</script>
