<script>
export default {
    name: 'ContactSection',
}
</script>

<template>
    <div id="contact" class="relative contact-container py-8 bg-transparent">
        <div class="max-w-4xl mx-auto px-4 pb-12">
            <!-- Section Header -->
            <div class="text-center mb-12">
                <h2 class="text-4xl font-bold text-gray-900">
                    <span class="text-[#a0ff70]">Contact Me</span>
                </h2>
                <div class="w-20 h-1 bg-[#a0ff70] mx-auto mt-4"></div>
                <p class="mt-4 text-gray-300">
                    Let's work together on your next project
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Email -->
                <div
                    class="contact-card p-6 rounded-xl bg-gradient-to-br from-gray-900 via-gray-800 to-gray-700  text-center">
                    <span class="inline-block p-3 text-[#a0ff70] rounded-full bg-gray-800 mx-auto">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor" class="w-6 h-6 text-[#a0ff70]">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M21.75 6.75v10.5a2.25 2.25 0 01-2.25 2.25h-15a2.25 2.25 0 01-2.25-2.25V6.75m19.5 0A2.25 2.25 0 0019.5 4.5h-15a2.25 2.25 0 00-2.25 2.25m19.5 0v.243a2.25 2.25 0 01-1.07 1.916l-7.5 4.615a2.25 2.25 0 01-2.36 0L3.32 8.91a2.25 2.25 0 01-1.07-1.916V6.75" />
                        </svg>
                    </span>

                    <h3 class="mt-4 text-lg font-medium text-gray-800">Email</h3>
                    <p class="mt-2 text-gray-300">Get in touch anytime!</p>
                    <a href="mailto:kabilansdev@gmail.com"
                        class="mt-2 text-[#a0ff70] hover:text-[#90ef60] inline-block">kabilansdev@gmail.com</a>
                </div>

                <!-- Location -->
                <div
                    class="contact-card p-6 rounded-xl bg-gradient-to-br from-gray-900 via-gray-800 to-gray-700  text-center">
                    <span class="inline-block p-3 text-[#a0ff70] rounded-full bg-gray-800 mx-auto">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor" class="w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M15 10.5a3 3 0 11-6 0 3 3 0 016 0z" />
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1115 0z" />
                        </svg>
                    </span>

                    <h3 class="mt-4 text-lg font-medium text-gray-800">Location</h3>
                    <p class="mt-2 text-gray-300">Based in <span class="text-[#a0ff70]">Chennai</span> </p>
                    <p class="mt-2 text-gray-300">Available for remote work</p>
                </div>

                <!-- Phone -->
                <div
                    class="contact-card p-6 rounded-xl bg-gradient-to-br from-gray-900 via-gray-800 to-gray-700  text-center">
                    <span class="inline-block p-3 text-[#a0ff70] rounded-full bg-gray-800 mx-auto">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor" class="w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M2.25 6.75c0 8.284 6.716 15 15 15h2.25a2.25 2.25 0 002.25-2.25v-1.372c0-.516-.351-.966-.852-1.091l-4.423-1.106c-.44-.11-.902.055-1.173.417l-.97 1.293c-.282.376-.769.542-1.21.38a12.035 12.035 0 01-7.143-7.143c-.162-.441.004-.928.38-1.21l1.293-.97c.363-.271.527-.734.417-1.173L6.963 3.102a1.125 1.125 0 00-1.091-.852H4.5A2.25 2.25 0 002.25 4.5v2.25z" />
                        </svg>
                    </span>

                    <h3 class="mt-4 text-lg font-medium text-gray-800">Phone</h3>
                    <p class="mt-2 text-gray-300">Mon-Fri 9am-5pm</p>
                    <a href="tel:+918667620030" class="mt-2 text-[#a0ff70] hover:text-[#90ef60] inline-block">+91
                        8667620030</a>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.contact-card {
    transition: all 0.3s ease-in-out;
}

.contact-card:hover {
    box-shadow: 0 0 30px rgba(160, 255, 112, 0.6);
    border-color: #a0ff70;
    transform: translateY(-2px);
}
</style>