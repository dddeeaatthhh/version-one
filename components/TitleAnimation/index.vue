<template>
  <div>
    <div class="titleContainer fadeIn">
      <div class="flip">D</div>
      <div class="flip">E</div>
      <div class="flipA">V</div>
      <div class="flip">T</div>
      <div class="flip">H</div>
    </div>

    <div class="subtext">omnibus et singulis perit</div>
  </div>
</template>

<style lang="scss" scoped>
$dur: 2;
$del: 2;
$fontSize: 25;

.titleContainer {
  font-family: "Source Serif Pro", serif;
  font-weight: 600;
  display: flex;
  justify-content: center;
  align-items: center;
  // display: none;
  // transform: translateX(-6px)
}

.titleContainer div {
  margin-left: 20px;
  margin-right: 20px;
}

.subtext {
  font-family: "Source Serif Pro", serif;
  font-weight: 400;
  font-size: 0.9rem;
  letter-spacing: 8px;
  margin-top: 10px;
  opacity: 0;
  animation: fadeIn 4s linear 10s forwards;
}

.flip {
  animation: fadeIn $dur + 1 + s ease-in-out,
    flip $dur + s ease-in-out $dur + s both;
  transform: rotateX(180deg);
}

.flipA {
  margin-top: 3px;
  animation: fadeIn $dur + 1 + s ease-in-out,
    flipA $dur * 2 + s ease-in-out $dur + s forwards;
  transform: rotateX(180deg);
}

@keyframes flip {
  0% {
    transform: rotateX(180deg);
  }
  100% {
    transform: rotateX(0);
  }
}

@keyframes flipA {
  0% {
    transform: rotateX(180deg) rotateY(0deg);
  }
  50% {
    transform: rotateX(0) rotateY(0deg);
  }
  100% {
    transform: rotateX(180deg) rotateY(180deg);
    // translate(-.2rem, .05rem)
  }
}
</style>