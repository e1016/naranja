


<h1 align="center">🍊 Naranja</h1>

<h3 align="center">Pure JS, HTML, and CSS Notifications with a great look – <a href="https://e1016.github.io/naranja-demo/">Live demo</a></h3>


`npm install --save naranja`


<h6 align="center">Script</h6>
<p align="center">
<code>&lt;script src="https://unpkg.com/naranja@1.0.1/lib/naranja.min.js">&lt;/script&gt;</code>
</p>
<h6 align="center">Styles</h6>
<p align="center">
<code>&lt;link rel="stylesheet" href="https://unpkg.com/naranja@1.0.1/lib/naranja.min.css"&gt;</code>
</p>
<p align="center">npm i -s naranja</p>


```js
// script
import naranja from 'naranja'
// styles
import '~/naranja/lib/naranja.min.css'
```
<p align="center">
  <img src="https://i.imgur.com/8vWYkFd.gif" />
<p>

---

_For first, why naranja? ... because all cool names in npm are taken, yes, and is easy to remember (it's orange in English)._

```js
naranja().log({
  title: 'Notification Title', // <- required
  text: 'Here goes a description for notifiaction', // <- required
  icon: true or false, // <- unrequired, default true,
  timeout: 2000 or 'keep', // <- unrequired, default 5000 miliseconds
  buttons: [
    {
      text: 'OK',
      click: function (e) {
        // click event close notifiaction
        // unless you use preventClose method
        e.preventClose()
        // if you want close notifiaction
        // manually, use closeNotification
        e.closeNotification()
      }
    },
    {
      text: 'Cancel',
      click: function () {
        // make something here...

        // you can (but you should not)
        // add infinity buttons
      }
    }
  ]
})
```

more notifiactions

```js

naranja().log({ ...

naranja().success({ ...

naranja().warn({ ...

naranja().error({ ...

```

All methods need the same arguments
