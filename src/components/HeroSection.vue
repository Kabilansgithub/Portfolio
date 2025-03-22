<script>
export default {
    name: 'HeroSection',
    data() {
        return {
            hellos: ['Hello', 'Hola', 'Bonjour', 'Hallo', 'Ciao', 'नमस्ते', 'こんにちは', '안녕하세요', '你好', 'வணக்கம்'],
            currentHello: 'Hello'
        };
    },
    mounted() {
        this.startHelloAnimation();
    },
    methods: {
        startHelloAnimation() {
            let index = 0;
            setInterval(() => {
                index = (index + 1) % this.hellos.length;
                this.currentHello = this.hellos[index];
            }, 1000);
        }
    }
}
</script>

<template>
    <div class="hero-container w-full min-h-screen flex items-center justify-center bg-gray-50">
        <div class="max-w-7xl mx-auto px-6 py-8">
            <div class="text-center">
                <h1 class="text-2xl tracking-tight font-bold sm:text-2xl md:text-2xl">
                    <span class="block text-[#a0ff70]">{{ currentHello }}, I'm Kabilan</span>
                </h1>

                <h1 class="text-4xl tracking-tight font-extrabold sm:text-5xl md:text-6xl">
                    <span class="block text-gray-700">Full Stack Developer</span>
                    <span class="block text-[#a0ff70]">& Web Designer</span>
                </h1>

                <p class="mt-4 text-lg text-gray-500 max-w-2xl mx-auto">
                    I craft elegant, user-centric web solutions using modern technologies. From responsive designs to
                    scalable backend architectures, I bring ideas to life with clean code and creative solutions.
                </p>

                <div class="mt-8 flex justify-center space-x-4">
                    <a href="#projects"
                        class="px-8 py-3 border border-transparent text-base font-medium rounded-md text-gray-700 bg-[#a0ff70] hover:bg-[#8ce460] transition duration-300 ease-in-out transform hover:scale-105 cursor-pointer">
                        View Projects
                    </a>
                    <a href="https://wa.me/918667620030" target="_blank"
                        class="px-8 py-3 border border-transparent text-base font-medium rounded-md text-[#a0ff70] bg-gray-100 hover:bg-gray-200 cursor-pointer">
                        Let's Connect
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>