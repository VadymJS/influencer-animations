<template>
    <div class="card" :style="`background-image: url(${props.card.imgUrl});`">
        <h5 class="card-title">{{ props.card.title }}</h5>
        <p class="card-subs">{{ props.card.subs }}</p>
        <div class="card-main">
            <div class="card-main-item">
                <p>Market price</p>
                <p>{{ props.card.marketPrice }}</p>
            </div>
            <div class="card-main-item">
                <p>Remaining time</p>
                <p>{{ props.card.time }}</p>
            </div>
        </div>
    </div>
</template>

<script setup>

const props = defineProps({
    card: Object
})

</script>
