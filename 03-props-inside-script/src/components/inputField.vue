
<script setup>
defineEmits(['onClick'])</script>

<template>
    <input type="text" placeholder="Enter your name" @click="$emit('onClick')"
</template>