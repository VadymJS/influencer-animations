<template>
    <header class="header wrapper">
        <div class="header-main">
            <button
                class="btn btn-rounded btn-header-burger"
                :class="{'is-active': isActiveBurger}"
                @click="toggleBurger"/>
            <a href="#" class="header-logo">
                <img src="../assets/img/logo.svg" alt="Logo" width="175" height="34">
            </a>
            <ul
                class="list"
                :class="{'is-active': isActiveBurger}">
                <li class="list-item">
                    <a href="#">How it works</a>
                </li>
                <li class="list-item">
                    <a href="#">Creators</a>
                </li>
                <li class="list-item">
                    <a href="#">Holders</a>
                </li>
                <li class="list-item">
                    <a href="#">About us</a>
                </li>
                <li class="list-item list-item-btn">
                    <button class="btn btn-header-mobile">Launch platform</button>
                </li>
            </ul>
        </div>
        <button class="btn btn-header-desktop">Launch platform</button>
    </header>
</template>

<script setup>
import { ref } from 'vue';

const isActiveBurger = ref(false);

function toggleBurger() {
    isActiveBurger.value = !isActiveBurger.value;
}

</script>
