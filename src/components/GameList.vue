<template>
    <div class="col" v-for="game in store.getGames" :key="game.id">
        <div class="card shadow-sm">
            <img :src="game.image" alt="" class="game-image" />
            <div class="card-body">
                <p class="card-text">
                    {{ game.description }}
                </p>
                <div class="d-flex justify-content-between align-items-center">
                    <div class="btn-group">
                        <button type="button" class="btn btn-sm btn-outline-secondary">
                            <i class="las la-info-circle icon-size"></i>&nbsp;Info
                        </button>
                        <button type="button" class="btn btn-sm btn-danger" @click="addToCart(game.id)">
                            <i class="las la-cart-plus icon-size text-white"></i>&nbsp;Buy
                        </button>
                    </div>
                    <small class="fs-3 fw-bold text-info">&euro; {{ game.price }}</small>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { useGamesStore } from '@/stores/games'

const store = useGamesStore();

function addToCart(id)
{
    store.addToCart(id);
}
</script>

<style scoped>

</style>