<template>
    <div v-if="showSplash" class="splash-screen">
        <transition name="fade" mode="out-in">
            <p :key="currentMessage" :class="currentFont">{{ currentMessage }}</p>
        </transition>
    </div>
</template>

<script>
export default {
    data() {
        return {
            messages: [
                "Loading... Just kidding, I'm fast.",
                "You’ve entered the world of Kabilan S — Watch what happens next.",
                "Sit back, relax, and let the code take you places."
            ],
            fonts: [
                "font-bungee",
                "font-unica",
                "font-major"
            ],
            currentMessageIndex: 0,
            showSplash: true,
        };
    },
    computed: {
        currentMessage() {
            return this.messages[this.currentMessageIndex];
        },
        currentFont() {
            return this.fonts[this.currentMessageIndex];
        }
    },
    mounted() {
        this.startMessageSequence();
    },
    methods: {
        startMessageSequence() {
            const interval = setInterval(() => {
                if (this.currentMessageIndex < this.messages.length - 1) {
                    this.currentMessageIndex++;
                } else {
                    clearInterval(interval);
                    setTimeout(() => {
                        this.showSplash = false;
                    }, 1700);
                }
            }, 1700);
        }
    }
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Bungee+Inline&family=Unica+One&family=Major+Mono+Display&display=swap');

.splash-screen {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background: linear-gradient(135deg, #000428, #004e92);
    color: #fff;
    text-align: center;
}

.font-bungee {
    font-family: 'Bungee Inline', cursive;
    font-size: 4rem;
    font-weight: 900;
}

.font-unica {
    font-family: 'Unica One', sans-serif;
    font-size: 4rem;
    font-weight: 700;
}

.font-major {
    font-family: 'Major Mono Display', monospace;
    font-size: 4rem;
    font-weight: 600;
}

.fade-enter-active,
.fade-leave-active {
    transition: opacity 0.8s;
}

.fade-enter,
.fade-leave-to {
    opacity: 0;
}
</style>
