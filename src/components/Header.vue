<template>
    <header class="header">
        <div class="header__logo-box">
            <img src="@/assets/logo-white.png" alt="logo" class="header__logo" />
        </div>

        <div class="header__text-box">
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
    name: 'Header'
};
</script>

<style src="./styles/Header.scss" lang="scss" />
