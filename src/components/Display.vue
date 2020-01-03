<template>
    <div class="display">
        <h1>Display</h1>
        <pre>{{ weatherData }}</pre>
    </div>
</template>

<script>
const axios = require('axios');

export default {
    name: 'Display',

    data() {
        return {
            weatherData: {}
        }
    },
    
    mounted() {
        this.load();
    },

    methods: {
        async load() {
            const response = await axios.get('http://localhost:3000/weather');
            this.weatherData = response;
        }
    }
}
</script>

<style lang="scss" scoped>
    .display {
		width: 50%;
        height: 100%;
        padding: 60px 40px;
        float: left;
	}
</style>