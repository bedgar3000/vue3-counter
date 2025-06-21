<script>
export default {
    name: 'App',
    data() {
        return {
            contador: 0
        };
    },
    methods: {
        increment() {
            this.contador++;
        },
        decrement() {
            this.contador--;
        },
        reset() {
            this.contador = 0;
        }
    }
};
</script>

<template>
    <div class="container">

        <img src="./assets/logo.svg" alt="Logo" width="125" height="125" />
        <h1>Hola mundo</h1>
        <hr>
        
        <h2>Contador: {{ contador }}</h2>
        <button @click="increment()">+1</button>
        <button @click="decrement()">-1</button>
        <button @click="reset()">Reset</button>
    </div>
</template>

<style scoped>
.container {
    text-align: center;
}
h1 {
    font-weight: bolder;;
}
small {
    color: #666666;
}
</style>