<script>

export default {
    name: 'MyName',
}

</script>

<template>
    <button id="btn">
        KABILAN S
    </button>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Agu+Display&family=Open+Sans:ital,wght@0,300..800;1,300..800&family=Orbitron:wght@400..900&family=Press+Start+2P&family=Raleway:ital,wght@0,100..900;1,100..900&display=swap');

#btn,
#btn::after {
    padding: 10px 50px;
    font-family: 'Agu Display';
    font-weight: 300;
    font-size: 25px;
    border: none;
    border-radius: 5px;
    color: rgb(255, 255, 255);
    background-color: transparent;
    position: relative;
}

#btn::after {
    --move1: inset(50% 50% 50% 50%);
    --move2: inset(31% 0 40% 0);
    --move3: inset(39% 0 15% 0);
    --move4: inset(45% 0 40% 0);
    --move5: inset(45% 0 6% 0);
    --move6: inset(14% 0 61% 0);
    clip-path: var(--move1);
    content: 'KABILAN S';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    display: block;
}

#btn:hover::after {
    animation: glitch_4011 1s;
    text-shadow: 10 10px 10px black;
    animation-timing-function: steps(2, end);
    text-shadow: -3px -3px 0px #1df2f0, 3px 3px 0px #E94BE8;
    background-color: transparent;
}

#btn:hover {
    text-shadow: -1px -1px 0px #1df2f0, 1px 1px 0px #E94BE8;
}

#btn:hover {
    background-color: transparent;
}

@keyframes glitch_4011 {
    0% {
        clip-path: var(--move1);
        transform: translate(0px, -10px);
    }

    10% {
        clip-path: var(--move2);
        transform: translate(-10px, 10px);
    }

    20% {
        clip-path: var(--move3);
        transform: translate(10px, 0px);
    }

    30% {
        clip-path: var(--move4);
        transform: translate(-10px, 10px);
    }

    40% {
        clip-path: var(--move5);
        transform: translate(10px, -10px);
    }

    50% {
        clip-path: var(--move6);
        transform: translate(-10px, 10px);
    }

    60% {
        clip-path: var(--move1);
        transform: translate(10px, -10px);
    }

    70% {
        clip-path: var(--move3);
        transform: translate(-10px, 10px);
    }

    80% {
        clip-path: var(--move2);
        transform: translate(10px, -10px);
    }

    90% {
        clip-path: var(--move4);
        transform: translate(-10px, 10px);
    }

    100% {
        clip-path: var(--move1);
        transform: translate(0);
    }
}
</style>