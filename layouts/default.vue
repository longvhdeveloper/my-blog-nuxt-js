<template>
  <Nuxt />
</template>
<style>
body {
  font-size: 20px;
  color: #212529;
  font-family: 'Lora', 'Times New Roman', serif;
}

p {
  line-height: 1.5;
  margin: 30px 0;
}

p a {
  text-decoration: underline;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-weight: 800;
  font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
}

a {
  color: #212529;
  transition: all 0.2s;
}

a:focus,
a:hover {
  color: #0085a1;
}

blockquote {
  font-style: italic;
  color: #868e96;
}

.section-heading {
  font-size: 36px;
  font-weight: 700;
  margin-top: 60px;
}

.caption {
  font-size: 14px;
  font-style: italic;
  display: block;
  margin: 0;
  padding: 10px;
  text-align: center;
  border-bottom-right-radius: 5px;
  border-bottom-left-radius: 5px;
}

::-moz-selection {
  color: #fff;
  background: #0085a1;
  text-shadow: none;
}

::selection {
  color: #fff;
  background: #0085a1;
  text-shadow: none;
}

img::-moz-selection {
  color: #fff;
  background: transparent;
}

img::selection {
  color: #fff;
  background: transparent;
}

img::-moz-selection {
  color: #fff;
  background: transparent;
}

.btn {
  font-size: 14px;
  font-weight: 800;
  padding: 15px 25px;
  letter-spacing: 1px;
  text-transform: uppercase;
  border-radius: 0;
  font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
}

.btn-primary {
  background-color: #0085a1;
  border-color: #0085a1;
}

.btn-primary:hover,
.btn-primary:focus,
.btn-primary:active {
  color: #fff;
  background-color: #00657b !important;
  border-color: #00657b !important;
}

.btn-lg {
  font-size: 16px;
  padding: 25px 35px;
}
</style>
