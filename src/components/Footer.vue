<template>
    <div>
        <!-- Main Content -->
        <div class="relative bg-black text-white h-screen overflow-hidden">
            <!-- Social Links -->
            <div class="absolute top-8 right-8 text-right">
                <ul class="space-y-2 text-lg">
                    <li><a href="#" class="hover:underline">LinkedIn</a></li>
                    <li><a href="#" class="hover:underline">Instagram</a></li>
                    <li><a href="#" class="hover:underline">Behance</a></li>
                    <li><a href="#" class="hover:underline">Twitter</a></li>
                </ul>
            </div>

            <!-- Floating Circle -->
            <div class="absolute top-16 left-1/3 transform -translate-x-1/2 w-10 h-10 bg-white rounded-full"></div>

            <!-- Large Name -->
            <div class="absolute bottom-16 left-0 right-0 text-center">
                <h1 class="text-9xl font-bold tracking-wide">KABILAN S</h1>
            </div>

            <!-- Footer Section -->
            <footer class="absolute bottom-4 left-8 text-gray-400 text-sm">
                <p>Copyright © KABILAN S</p>
            </footer>

            <footer class="absolute bottom-4 right-8 text-gray-400 text-sm">
                <p>Proudly 🇮🇳</p>
            </footer>

            <!-- Current Time in IST -->
            <div class="absolute bottom-12 left-1/2 transform -translate-x-1/2 text-gray-500" id="current-time">
                IST --:--:--
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            showSplash: true
        };
    },
    mounted() {
        setTimeout(() => {
            this.showSplash = false;
        }, 5000);
        this.updateTime();
        setInterval(this.updateTime, 1000);
    },
    methods: {
        updateTime() {
            const now = new Date();
            const options = { timeZone: 'Asia/Kolkata', hour12: false, hour: '2-digit', minute: '2-digit', second: '2-digit' };
            const timeString = new Intl.DateTimeFormat('en-IN', options).format(now);
            document.getElementById('current-time').innerText = `IST ${timeString}`;
        }
    }
};
</script>

<style scoped>
footer {
    font-family: Arial, sans-serif;
}
</style>