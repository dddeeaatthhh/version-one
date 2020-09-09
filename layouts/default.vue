<template>
  <div>
    <Nuxt />
  </div>
</template>

<style lang="scss">
html {
  font-family: "Source Serif Pro", serif;
  font-size: 18px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  background-color: #000;
  color: ghostwhite;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
</style>
