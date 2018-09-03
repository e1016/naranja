


<h1 align="center">🍊 Naranja</h1>

<h3 align="center">Notifications with a great look</h3>

<h6 align="center">Script</h6>
<p align="center">
<code>&lt;script&gt; src="https://unpkg.com/naranja@1.0.0/lib/naranja.min.js">&lt;/script&gt;</code>
</p>
<h6 align="center">Styles</h6>
<p align="center">
<code>&lt;link rel="stylesheet" href="https://unpkg.com/naranja@1.0.0/lib/naranja.min.css"&gt;</code>
</p>
<p align="center">npm soon...</p>



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
  timeout: 2000 or 'keep', // <- unrequired, default 3000 miliseconds
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
