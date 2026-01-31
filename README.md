<style>
  /* Hides the main auto-generated title */
  h1, .page-heading, .post-title {
    display: none !important;
  }
  
  /* Make the "Show QR Code" text 12.5% smaller and nudge it right */
  summary {
    font-size: 0.875em;
    cursor: pointer;
    outline: none; /* Removes the blue box when clicking */
    margin-left: 5px; /* Nudges the button to the right */
  }
</style>

If you enjoy my tools and want to support me, you can donate below.

<div style="height:1px; background-color:#dbdbdb; margin:20px 0;"></div>

**Bitcoin (BTC):**
<div style="display:flex; align-items:center; gap:2px; margin-top:-12px; margin-bottom:4px;">
  <button onclick="copy('btc', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0;" title="Copy Address">📋</button>
  <code id="btc" style="word-break: break-all;">bc1qzthdgzhdjmqgan5n9c3dp5g3m24sqv30unzxjn</code>
</div>

<details>
  <summary>Show Bitcoin QR Code</summary>
  <br>
  <img src="btc.png" width="250" alt="Bitcoin QR">
</details>

<div style="height:1px; background-color:#dbdbdb; margin:20px 0;"></div>

**Ethereum (ETH):**
<div style="display:flex; align-items:center; gap:2px; margin-top:-12px; margin-bottom:4px;">
  <button onclick="copy('eth', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0;" title="Copy Address">📋</button>
  <code id="eth" style="word-break: break-all;">0xda1c45125c3148bef77922225da5936d7777ca0e</code>
</div>

<details>
  <summary>Show Ethereum QR Code</summary>
  <br>
  <img src="eth.png" width="250" alt="Ethereum QR">
</details>

<div style="height:1px; background-color:#dbdbdb; margin:20px 0;"></div>

**XRP:** <span style="font-size: 0.875em;">(Tag not required. If forced, use 0)</span>
<div style="display:flex; align-items:center; gap:2px; margin-top:-12px; margin-bottom:4px;">
  <button onclick="copy('xrp', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0;" title="Copy Address">📋</button>
  <code id="xrp" style="word-break: break-all;">rN3KXnyiZvNFTUkY1Yry5xrx3nyNTMjPPo</code>
</div>

<details>
  <summary>Show XRP QR Code</summary>
  <br>
  <img src="xrp.png" width="250" alt="XRP QR">
</details>

<div style="height:1px; background-color:#dbdbdb; margin:20px 0;"></div>

**Solana (SOL):**
<div style="display:flex; align-items:center; gap:2px; margin-top:-12px; margin-bottom:4px;">
  <button onclick="copy('sol', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0;" title="Copy Address">📋</button>
  <code id="sol" style="word-break: break-all;">GxUYy9TrK5sKvr8NEYs8QeC1XZ8ZZ8e2xhevYmf83JPu</code>
</div>

<details>
  <summary>Show Solana QR Code</summary>
  <br>
  <img src="sol.png" width="250" alt="Solana QR">
</details>

<div style="height:1px; background-color:#dbdbdb; margin:20px 0;"></div>

**Dogecoin (DOGE):**
<div style="display:flex; align-items:center; gap:2px; margin-top:-12px; margin-bottom:4px;">
  <button onclick="copy('doge', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0;" title="Copy Address">📋</button>
  <code id="doge" style="word-break: break-all;">DAHdS4S4tuhPy2HMbboYaTf6unPHQPYyAH</code>
</div>

<details>
  <summary>Show Dogecoin QR Code</summary>
  <br>
  <img src="doge.png" width="250" alt="Dogecoin QR">
</details>

<div style="height:1px; background-color:#dbdbdb; margin:20px 0;"></div>

**Monero (XMR):**
<div style="display:flex; align-items:center; gap:2px; margin-top:-12px; margin-bottom:4px;">
  <button onclick="copy('xmr', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0;" title="Copy Address">📋</button>
  <code id="xmr" style="word-break: break-all;">85WaFLhsc6QFR747nCLtmMes7Qhfwd1gkauBxdep3jpGS2KXj7res17LV5myFNR9XNLGeBEeWmmBpibDEVWG3zpWA1xiQzK</code>
</div>

<details>
  <summary>Show Monero QR Code</summary>
  <br>
  <img src="xmr.png" width="250" alt="Monero QR">
</details>

<div style="height:1px; background-color:#dbdbdb; margin:20px 0;"></div>

**Litecoin (LTC):**
<div style="display:flex; align-items:center; gap:2px; margin-top:-12px; margin-bottom:4px;">
  <button onclick="copy('ltc', this)" style="cursor:pointer; font-size: 1.2em; border:none; background:none; padding:0; margin:0;" title="Copy Address">📋</button>
  <code id="ltc" style="word-break: break-all;">ltc1qv2etczlwqklcvkh9axt5uruh0r2qjj45s978pp</code>
</div>

<details>
  <summary>Show Litecoin QR Code</summary>
  <br>
  <img src="ltc.png" width="250" alt="Litecoin QR">
</details>

<div style="height:1px; background-color:#dbdbdb; margin:20px 0;"></div>

*Thanks for your support!* [vixkrell@gmail.com](mailto:vixkrell@gmail.com)

<script>
// Variables to track the currently active button and its timer
var activeBtn = null;
var activeTimer = null;

function copy(id, btn) {
  var txt = document.getElementById(id).innerText;
  
  navigator.clipboard.writeText(txt).then(function() {
    
    // 1. If there is already a green checkmark on a DIFFERENT button, reset it immediately
    if (activeBtn && activeBtn !== btn) {
      activeBtn.innerText = "📋";
      clearTimeout(activeTimer);
    }
    
    // 2. If clicking the SAME button again, reset the timer so it stays green longer
    if (activeBtn === btn) {
      clearTimeout(activeTimer);
    }
    
    // 3. Turn the current button green and save it as "active"
    btn.innerText = "✅";
    activeBtn = btn;
    
    // 4. Start the timer to revert THIS button after 1750ms
    activeTimer = setTimeout(function() {
      btn.innerText = "📋";
      activeBtn = null;
      activeTimer = null;
    }, 1750);
    
  }, function(err) {
    console.error('Could not copy text: ', err);
  });
}
</script>
