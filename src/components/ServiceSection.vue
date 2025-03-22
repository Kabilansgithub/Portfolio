<script>
export default {
    name: "ServiceSection",
}
</script>

<template>
    <div id="services" class="relative service-container py-8 bg-transparent ">
        <div class="max-w-6xl mx-auto px-4">
            <!-- Section Header -->
            <div class="text-center mb-12">
                <h2 class="text-4xl font-bold text-gray-900">
                    <span class="text-[#a0ff70]"> My Services</span>
                </h2>
                <div class="w-20 h-1 bg-[#a0ff70] mx-auto mt-4"></div>
            </div>

            <!-- Services Grid -->
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Web Development -->
                <div class="service-card p-6 rounded-xl bg-white shadow-lg shadow-gray-200/50 hover:scale-105">
                    <div class="text-[#a0ff70] mb-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-12 w-12" fill="none" viewBox="0 0 24 24"
                            stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4" />
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold mb-2 text-gray-900">Web Development</h3>
                    <p class="text-gray-600">Full-stack web development using Laravel and Vue.js</p>
                </div>

                <!-- UI/UX Design -->
                <div class="service-card p-6 rounded-xl bg-white shadow-lg shadow-gray-200/50 hover:scale-105">
                    <div class="text-[#a0ff70] mb-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-12 w-12" fill="none" viewBox="0 0 24 24"
                            stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M7 21a4 4 0 01-4-4V5a2 2 0 012-2h4a2 2 0 012 2v12a4 4 0 01-4 4zm0 0h12a2 2 0 002-2v-4a2 2 0 00-2-2h-2.343M11 7.343l1.657-1.657a2 2 0 012.828 0l2.829 2.829a2 2 0 010 2.828l-8.486 8.485M7 17h.01" />
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold mb-2 text-gray-900">UI/UX Design</h3>
                    <p class="text-gray-600">Creating intuitive and responsive user interfaces</p>
                </div>

                <!-- API Development -->
                <div class="service-card p-6 rounded-xl bg-white shadow-lg shadow-gray-200/50 hover:scale-105">
                    <div class="text-[#a0ff70] mb-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-12 w-12" fill="none" viewBox="0 0 24 24"
                            stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M8 9l3 3-3 3m5 0h3M5 20h14a2 2 0 002-2V6a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z" />
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold mb-2 text-gray-900">API Development</h3>
                    <p class="text-gray-600">Building robust and scalable RESTful APIs</p>
                </div>

                <!-- Database Design -->
                <div class="service-card p-6 bg-white rounded-xl shadow-lg">
                    <div class="text-[#a0ff70] mb-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-12 w-12" fill="none" viewBox="0 0 24 24"
                            stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M4 7v10c0 2.21 3.582 4 8 4s8-1.79 8-4V7M4 7c0 2.21 3.582 4 8 4s8-1.79 8-4M4 7c0-2.21 3.582-4 8-4s8 1.79 8 4m0 5c0 2.21-3.582 4-8 4s-8-1.79-8-4" />
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold mb-2 text-gray-900">Database Design</h3>
                    <p class="text-gray-600">Efficient database architecture and optimization</p>
                </div>

                <!-- E-commerce Solutions -->
                <div class="service-card p-6 bg-white rounded-xl shadow-lg">
                    <div class="text-[#a0ff70] mb-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-12 w-12" fill="none" viewBox="0 0 24 24"
                            stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M3 10h18M3 14h18M3 18h18M3 6h18" />
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold mb-2 text-gray-900">E-commerce Solutions</h3>
                    <p class="text-gray-600">Custom online store development and integration</p>
                </div>

                <!-- Website Maintenance -->
                <div class="service-card p-6 bg-white rounded-xl shadow-lg">
                    <div class="text-[#a0ff70] mb-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-12 w-12" fill="none" viewBox="0 0 24 24"
                            stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M8 16h8M8 12h8M8 8h8M4 4h16v16H4V4z" />
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold mb-2 text-gray-900">Website Maintenance</h3>
                    <p class="text-gray-600">Regular updates, security, and performance optimization</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.service-card {
    transition: all 0.3s ease-in-out;
}

.service-card:hover {
    box-shadow: 0 0 30px rgba(160, 255, 112, 0.6);
    border-color: #a0ff70;
    transform: translateY(-2px);
}
</style>