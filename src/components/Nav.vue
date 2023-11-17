<script setup>
import { RouterLink } from 'vue-router'
import { useGamesStore } from '@/stores/games'

const store = useGamesStore();
</script>

<template>
    <nav class="navbar bg-dark navbar-expand-lg bg-body-tertiary m-0" data-bs-theme="dark">
        <div class="container-fluid">
            <RouterLink to="/" class="navbar-brand">
                <img src="img/eengameshop.png" alt="Logo Een Game Shop" class="logo-image" />
                Een Game Shop
            </RouterLink>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                        <RouterLink to="/" class="nav-link active" aria-current="page">Home</RouterLink>
                    </li>
                    <li class="nav-item">
                        <RouterLink to="cart" class="nav-link">Winkelwagen</RouterLink>
                    </li>
                </ul>
            </div>
            <span class="badge text-bg-primary position-relative">
                <i class="las la-shopping-cart icon-size text-white"></i>
                <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-danger">
                    <span id="cart-amount">
                        {{  store.countItemsInCart }}
                    </span>
                    <span class="visually-hidden">Items in cart</span>
                </span>
            </span>
        </div>
    </nav>
</template>
