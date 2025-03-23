<script>
export default {
    name: "AboutSection"
};
</script>

<template>
    <div id="about" class="relative py-16 bg-gradient-to-br from-gray-900 via-gray-800 to-gray-700 text-white">
        <div class="max-w-7xl mx-auto px-6">
            <div class="grid md:grid-cols-12 gap-12 items-center">
                <!-- Profile Image Section with Glow Effect -->
                <div class="md:col-span-4">
                    <img src="/src/assets/images/blackandwhite.jpg" alt="Profile Picture"
                        class="h-[400px] w-full rounded-xl shadow-lg object-cover hover:shadow-[#a0ff70]/50 transition-transform transform hover:scale-105">
                </div>

                <!-- About Content Section -->
                <div class="md:col-span-8">
                    <h2
                        class="text-4xl font-extrabold mb-6 bg-clip-text text-transparent bg-gradient-to-r from-[#a0ff70] to-[#70e1ff]">
                        Hey, I'm Kabilan S
                    </h2>
                    <p class="mb-8 text-lg text-gray-300 leading-relaxed">
                        A dedicated Full Stack Developer with a strong passion for building dynamic web applications.
                        Experienced in crafting elegant, user-centric solutions using Laravel and Vue.js.
                    </p>

                    <!-- Skills Section with Animation -->
                    <div class="mb-10">
                        <h3 class="text-2xl font-semibold mb-4 text-[#a0ff70]">Skills</h3>
                        <div class="flex flex-wrap gap-4">
                            <span
                                class="px-4 py-2 bg-[#a0ff70] rounded-full text-gray-800 text-sm font-semibold transform hover:scale-110 transition-transform">Laravel</span>
                            <span
                                class="px-4 py-2 bg-[#a0ff70] rounded-full text-gray-800 text-sm font-semibold transform hover:scale-110 transition-transform">Vue.js</span>
                            <span
                                class="px-4 py-2 bg-[#a0ff70] rounded-full text-gray-800 text-sm font-semibold transform hover:scale-110 transition-transform">PHP</span>
                            <span
                                class="px-4 py-2 bg-[#a0ff70] rounded-full text-gray-800 text-sm font-semibold transform hover:scale-110 transition-transform">JavaScript</span>
                            <span
                                class="px-4 py-2 bg-[#a0ff70] rounded-full text-gray-800 text-sm font-semibold transform hover:scale-110 transition-transform">MySQL</span>
                        </div>
                    </div>

                    <!-- Experience Section -->
                    <div class="mb-8">
                        <h3 class="text-2xl font-semibold mb-4 text-[#a0ff70]">Experience</h3>
                        <ul class="list-disc list-inside text-gray-300">
                            <li>Intern at White Crappie Technologies</li>
                        </ul>
                    </div>

                    <!-- Contact Me Button with Hover Animation -->
                    <a href="https://wa.me/918667620030" target="_blank"
                        class="inline-flex items-center px-8 py-3 bg-[#70e1ff] hover:bg-[#a0ff70] text-gray-900 font-semibold rounded-lg transition-transform transform hover:scale-110 shadow-md">
                        Contact Me
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 ml-2" viewBox="0 0 20 20"
                            fill="currentColor">
                            <path fill-rule="evenodd"
                                d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
                                clip-rule="evenodd" />
                        </svg>
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
img {
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}
</style>
