<center>
    <h1>
        CapSolver Modded Wrapper . Vedal Copyrigt(c)
    </h1>

</center>

<center>A wrapper around the <a href="https://capsolver.com/">CapSolver</a> API</center>
<br>
<br>

If there's problems with this service, you can contact me in Discord : vedal.

## Features


Currently Supports:
- Google Recaptcha (v2/v3/enterprise),
- hcaptcha,
- FunCaptcha,
- base64 image captchas
- will be add soon Cloudflare Turnstile,AWS WAF,MT Captcha , DataDome SLider, CyberSiara captcha,GEETEST v3/v4,Image To Text OCR.


## Install

```sh
npm install vedal-modded-capsolver
```


## Usage


Recaptcha Example ,
```js
const CapSolver = require('vedal-modded-capsolver')
//to creat instance 
const solver = new CapSolver.Solver("your capsolver api key.")

/* Example ReCaptcha Website */

solver.recaptchaV2("here-website-key", "here website link")

.then((res) => {
    console.log(res)
})
.catch((err) => {
    console.error("Could not solve this captcha.")
})
```
