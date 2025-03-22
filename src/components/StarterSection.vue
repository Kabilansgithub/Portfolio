<template>
    <div v-if="showWelcome" class="welcome">Welcome to My Portfolio!</div>
</template>

<script>
export default {
    data() {
        return {
            showWelcome: true
        };
    },
    mounted() {
        this.showWelcome = true;
        // Display welcome message for 5 seconds and then hide it
        setTimeout(() => {
            this.showWelcome = false;
            this.$router.push('/home');
        }, 5000);
    }
};
</script>

<style scoped>
.welcome {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #282c34;
    color: white;
    font-size: 2.5rem;
    font-family: Arial, sans-serif;
    animation: fadeOut 5s forwards;
}

@keyframes fadeOut {
    0% {
        opacity: 1;
    }

    100% {
        opacity: 0;
    }
}

.content {
    padding: 20px;
}
</style>