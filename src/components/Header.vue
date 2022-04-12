<template>
  <header class="header">
    <div class="logo-box">
      <img src="@/assets/logo-white.png" alt="logo" class="logo" />
    </div>

    <div class="text-box">
      <h1 class="heading-primary">
        <span class="heading-primary-main">Outdoors</span>
        <span class="heading-primary-sub">is where life happens</span>
      </h1>
      <a href="#" class="btn btn-white btn-animated"> Discovery our tours </a>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style>
.header {
  height: 95vh;
  background-image: linear-gradient(
      to right bottom,
      rgba(126, 213, 111, 0.7),
      rgba(40, 180, 133, 0.7)
    ),
    url(../assets/hero.jpg);
  background-size: cover;
  background-position: top;

  clip-path: polygon(0 0, 100% 0, 100% 75vh, 0 100%);
  position: relative;
}
.logo-box {
  position: absolute;
  top: 40px;
  left: 40px;
}

.logo {
  height: 35px;
}

.text-box {
  position: absolute;
  top: 40%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
}

.heading-primary {
  color: #fff;
  text-transform: uppercase;

  backface-visibility: hidden;
  margin-bottom: 60px;
}
.heading-primary-main {
  display: block;
  font-size: 60px;
  font-weight: 400;
  letter-spacing: 35px;

  animation-name: moveInLeft;
  animation-duration: 1s;
  animation-timing-function: ease-in;

  /* animation-iteration-count: 3; */
  /* animation-delay: 3s; */
}
.heading-primary-sub {
  display: block;
  font-size: 20px;
  font-weight: 700;
  letter-spacing: 17.4px;

  animation: moveInRight 1s ease-in;
}

@keyframes moveInLeft {
  0% {
    opacity: 0;
    transform: translateX(-100px);
  }

  80% {
    transform: translateX(20px);
  }

  100% {
    opacity: 1;
    transform: translate(0);
  }
}

@keyframes moveInRight {
  0% {
    opacity: 0;
    transform: translateX(100px);
  }

  80% {
    transform: translateX(-20px);
  }

  100% {
    opacity: 1;
    transform: translate(0);
  }
}

.btn:link,
.btn:visited {
  text-transform: uppercase;
  text-decoration: none;
  padding: 15px 40px;
  display: inline-block;
  border-radius: 100px;
  transition: all 0.2s;
  position: relative;
}

.btn:hover {
  transform: translateY(-3px);
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
}

.btn:active {
  transform: translateY(-1px);
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
}

.btn-white {
  background-color: #fff;
  color: #777;
}
.btn::after {
  content: "";
  display: inline-block;
  height: 100%;
  width: 100%;
  border-radius: 100px;
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
  transition: all 0.4s;
}

.btn-white::after {
  background-color: #fff;
}
.btn:hover::after {
  transform: scaleX(1.4) scaleY(1.6);
  opacity: 0;
}

.btn-animated {
  animation: moveInTBottom 0.5s ease-out 0.75s;
  animation-fill-mode: backwards;
}

@keyframes moveInTBottom {
  0% {
    opacity: 0;
    transform: translateY(30px);
  }

  100% {
    opacity: 1;
    transform: translate(0);
  }
}
</style>
