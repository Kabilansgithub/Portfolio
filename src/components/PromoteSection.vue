<template>
    <div
        class="relative promote-section py-12 bg-gradient-to-br from-gray-900 via-gray-800 to-gray-700 transition-colors duration-200">
        <div class="lg:flex lg:items-center lg:justify-between w-full mx-auto px-6 sm:px-8 lg:px-12 max-w-7xl">
            <!-- Headline Section -->
            <h2 class="text-4xl font-extrabold text-white sm:text-5xl mb-8 lg:mb-0 leading-tight animate-fade-in">
                <span class="block">Ready to bring your ideas to life?</span>
                <span
                    class="block text-transparent bg-clip-text bg-gradient-to-r from-[#a0ff70] to-[#70e1ff] animate-slide-up">
                    Let's build something amazing together.
                </span>
            </h2>

            <!-- CTA Button with Animation -->
            <div class="lg:mt-0 lg:flex-shrink-0">
                <a href="https://forms.gle/wNJJb6tPNshD1ePG9" target="_blank"
                    class="inline-flex items-center justify-center px-8 py-4 bg-[#70e1ff] hover:bg-[#58d4f0] text-gray-900 font-bold text-lg rounded-lg transition-transform transform hover:scale-110 shadow-xl animate-pulse">
                    Start a Project
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 ml-2" viewBox="0 0 20 20"
                        fill="currentColor">
                        <path fill-rule="evenodd"
                            d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
                            clip-rule="evenodd" />
                    </svg>
                </a>
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

.animate-pulse {
    animation: pulse 1.5s infinite;
}

@keyframes pulse {

    0%,
    100% {
        transform: scale(1);
    }

    50% {
        transform: scale(1.05);
    }
}
</style>