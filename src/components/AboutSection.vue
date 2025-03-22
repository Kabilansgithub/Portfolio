<script>
export default {
    name: "AboutSection"
}
</script>

<template>
    <div id="about" class="relative py-12 bg-transparent text-white">
        <div class="max-w-6xl mx-auto px-4">
            <div class="text-center mb-12">
                <h1 class="text-4xl font-bold">
                    <span class="text-[#a0ff70]">About Me</span>
                </h1>
                <div class="w-20 h-1 bg-[#a0ff70] mx-auto mt-4"></div>
            </div>

            <div class="grid md:grid-cols-12 gap-8 items-center">
                <!-- Profile Image -->
                <div class="md:col-span-4">
                    <img src="/src/assets/images/blackandwhite.jpg" alt="Profile Picture"
                        class="h-[400px] w-full rounded-lg shadow-lg object-cover shadow-gray-700/50">
                </div>

                <!-- About Content -->
                <div class="md:col-span-8">
                    <h2 class="text-2xl font-semibold mb-4 text-gray-400">Hello, I'm Kabilan S</h2>
                    <p class="mb-6 text-gray-400">
                        I'm a passionate Full Stack Developer with 6 months of experience in Web Development. I
                        specialize in Laravel & Vue.js.
                    </p>

                    <!-- Skills Section -->
                    <div class="mb-8">
                        <h3 class="text-xl font-semibold mb-3 text-gray-400">Skills</h3>
                        <div class="flex flex-wrap gap-3">
                            <span class="px-3 py-1 bg-[#a0ff70] rounded-full text-sm text-gray-800">Laravel</span>
                            <span class="px-3 py-1 bg-[#a0ff70] rounded-full text-sm text-gray-800">Vue.js</span>
                            <span class="px-3 py-1 bg-[#a0ff70] rounded-full text-sm text-gray-800">PHP</span>
                            <span class="px-3 py-1 bg-[#a0ff70] rounded-full text-sm text-gray-800">JavaScript</span>
                            <span class="px-3 py-1 bg-[#a0ff70] rounded-full text-sm text-gray-800">MySQL</span>
                        </div>
                    </div>

                    <!-- Experience Section -->
                    <div class="mb-8">
                        <h3 class="text-xl font-semibold mb-3 text-gray-400">Experience</h3>
                        <ul class="list-disc list-inside text-gray-400">
                            <li>Intern at White Crappie Technologies</li>
                        </ul>
                    </div>

                    <!-- Contact Button -->
                    <a href="https://wa.me/918667620030" target="_blank"
                        class="inline-flex items-center px-6 py-3 bg-[#a0ff70] hover:bg-[#8ce460] text-gray-800 font-semibold rounded-lg transition-transform transform hover:scale-105 shadow-md">
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

<style scoped></style>