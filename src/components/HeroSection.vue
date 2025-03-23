<script>
export default {
    name: 'HeroSection',
    data() {
        return {
            hellos: ['வணக்கம்', 'Hello', 'नमस्ते', 'こんにちは', 'Hola', 'Bonjour', 'Hallo', 'Ciao', '안녕하세요', '你好'],
            currentHello: 'வணக்கம்',
            intervalId: null
        };
    },
    mounted() {
        this.startHelloAnimation();
    },
    beforeUnmount() {
        clearInterval(this.intervalId);
    },
    methods: {
        startHelloAnimation() {
            let index = 0;
            this.intervalId = setInterval(() => {
                index = (index + 1) % this.hellos.length;
                this.currentHello = this.hellos[index];
            }, 1000);
        }
    }
};
</script>

<template>
    <div class="relative hero-container w-full min-h-screen flex items-center justify-center ">
        <div class="max-w-7xl mx-auto px-6 pt-16 pb-6">
            <div class="text-center">
                <!-- Animated Hello Text with Bounce Effect -->
                <h1 class="text-3xl tracking-tight font-bold sm:text-4xl md:text-5xl  animate-bounce ">
                    <span class="block text-[#a0ff70]">{{ currentHello }}, I'm Kabilan</span>
                </h1>

                <!-- Main Title with Gradient and Subtle Animation -->
                <h1 class="text-5xl tracking-tight font-extrabold sm:text-6xl md:text-7xl leading-tight">
                    <span
                        class="block text-transparent bg-clip-text bg-gradient-to-r from-[#a0ff70] to-[#70e1ff] animate-fade-in">Full
                        Stack Developer</span>
                    <span class="block text-[#a0ff70] animate-slide-up">& Web Designer</span>
                </h1>

                <!-- Description Section -->
                <p class="mt-6 text-lg text-gray-300 max-w-2xl mx-auto leading-relaxed">
                    Crafting intuitive, responsive, and high-performance web applications using cutting-edge
                    technologies. Transforming ideas into digital experiences that leave a lasting impact.
                </p>

                <!-- CTA Buttons with Enhanced Hover Effects -->
                <div class="mt-8 flex justify-center space-x-6">
                    <a href="#projects"
                        class="px-8 py-3 border border-transparent text-lg font-semibold rounded-lg text-gray-700 bg-[#a0ff70] hover:bg-[#8ce460] transition duration-300 ease-in-out transform hover:scale-110 shadow-lg">
                        View Projects
                    </a>
                    <a href="https://wa.me/918667620030" target="_blank"
                        class="px-8 py-3 border border-transparent text-lg font-semibold rounded-lg text-[#a0ff70] bg-[#000000] hover:bg-[#101010] transform transition duration-300 ease-in-out hover:scale-110 shadow-lg">
                        Let's Connect
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
@keyframes fadeIn {
    from {
        opacity: 0;
    }

    to {
        opacity: 1;
    }
}

@keyframes slideUp {
    from {
        transform: translateY(20px);
        opacity: 0;
    }

    to {
        transform: translateY(0);
        opacity: 1;
    }
}

.animate-fade-in {
    animation: fadeIn 1.5s ease-in-out;
}

.animate-slide-up {
    animation: slideUp 1.5s ease-out;
}

.animate-bounce {
    animation: bounce 1.5s infinite ease-in-out;
}

@keyframes bounce {

    0%,
    100% {
        transform: translateY(0);
    }

    50% {
        transform: translateY(-10px);
    }
}
</style>
