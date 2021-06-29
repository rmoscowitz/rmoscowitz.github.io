---
layout: post
title: Multi Colored Text
---

I saw [this tweet](https://twitter.com/bramusblog/status/1409484007511838723) with a cute example of using CSS to color text with a background gradient. Check it out!

<div class="multi-color">
  <div class="wrapper">
    <div class="container">
      <h1>Robyn Moscowitz Narro</h1>
    </div>
  </div>
</div>

The html:

```html
<div class="wrapper">
  <div class="container">
    <h1>Robyn Moscowitz Narro</h1>
  </div>
</div>
```
The key is the background gradient and transparent text! Neat, huh?

```css
* {
  box-sizing: border-box
}

:root {
  --color-1: #FFB2E6;
  --color-2: #D972FF;
  --color-3: #8447FF;
  --color-4: #8CFFDA;
  --color-5: #FFFFE8;
}

.wrapper {
  background: #000;
  line-height: 1;
  min-height: 100%;
  display: grid;
  place-items: center;
}

h1 {
  font-family: "Exo", sans-serif;
  font-size: 15vw;
  font-weight: 900;
  width: -webkit-min-content;
  width: -moz-min-content;
  width: min-content;
  margin: auto;
  text-transform: uppercase;
  background: linear-gradient(219deg, 
    var(--color-1) 19%, 
    transparent 19%,transparent 20%, 
    var(--color-2) 20%, var(--color-2)  39%,
    transparent 39%,transparent 40%, 
    var(--color-3) 40%,var(--color-3) 59% ,
    transparent 59%,transparent 60%, 
    var(--color-4) 60%, var(--color-4) 79%,
    transparent 79%, transparent 80%, 
    var(--color-5) 80%);
  background-clip: text;
  -webkit-background-clip: text;
  color: transparent;
}

.container {
  padding: 1.5rem;   
  text-align: center;
}

@media screen and (min-width: 768px) {
  h1 {
    font-size: 6.5rem;
  }
}
```
