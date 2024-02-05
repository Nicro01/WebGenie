<template>
    <div
        :class="{ dark: isDarkMode }"
        class="dark:bg-black bg-white min-h-screen p-2 dark:text-white text-black select-none uppercase"
    >
        <div
            class="w-16 h-8 z-50 fixed bottom-2 left-2 md:left-[95%] md:top-3 md:right-5 flex items-center bg-gray-300 rounded-full p-1 cursor-pointer"
            :class="{
                'bg-slate-600': isDarkMode,
                'bg-yellow-100': !isDarkMode,
            }"
            @click="toggleDarkMode"
        >
            <div
                class="w-6 h-6 rounded-full shadow-md transform duration-300 ease-in-out"
                :class="{
                    'translate-x-8': isDarkMode,
                    'bg-slate-900': isDarkMode,
                    'bg-yellow-300': !isDarkMode,
                }"
            >
                <span class="block text-center" v-if="isDarkMode"></span>
                <!-- Moon Emoji -->
                <span class="block text-center" v-else></span>
                <!-- Sun Emoji -->
            </div>
        </div>

        <!-- FIRST ROW -->

        <div
            class="grid grid-cols-12 border-black dark:border-white dark:bg-black dark:text-white border-solid border-[1px]"
        >
            <div
                class="col-span-12 md:col-span-8 box-decoration-slice flex items-center border-bottom md:border-b-[transparent !important] change-bg justify-center py-4 md:pt-0 md:pb-2 md-border-right"
            >
                <h2 class="text-3xl md:text-8xl tracking-[0.6em] break-words">
                    WebGeni
                </h2>
                <h2 class="text-3xl md:text-8xl md:-ml-2">E</h2>
            </div>
            <div
                class="col-span-12 border-bottom md:border-b-transparent md:col-span-2 md-border-right"
            >
                <div
                    class="flex box-decoration-slice flex-col justify-between h-full"
                >
                    <button
                        class="py-2 change-bg text-center md:text-start pl-2 md-border-bottom border-bottom"
                    >
                        Serviços
                    </button>
                    <button
                        class="py-2 change-bg text-center md:text-start pl-2 md-border-bottom border-bottom"
                    >
                        Tecnologias
                    </button>
                    <button
                        class="py-2 change-bg text-center md:text-start pl-2"
                    >
                        Contato
                    </button>
                </div>
            </div>
            <div class="col-span-12 md:col-span-2 box-decoration-slice">
                <button
                    class="py-10 flex justify-center items-center md:py-2 change-bg h-full md:mx-auto w-full"
                >
                    <p class="text-2xl">
                        Tenha seu <br />
                        próprio site
                    </p>
                </button>
            </div>
        </div>

        <!-- ---------  -->

        <!-- SECOND ROW -->

        <div
            class="grid grid-cols-12 bg-white border-black dark:border-white border-t-transparent dark:bg-black border-solid border-[1px]"
        >
            <div
                class="md:col-span-4 col-span-8 flex flex-col dark:text-white pl-10 justify-center change-bg py-10 md-border-right border-right"
            >
                <h2
                    class="text-xl font-semibold md:text-2xl tracking-[0.28em] break-words"
                >
                    Potencialize Seu Negócio
                </h2>
                <h2 class="text-base md:text-xl tracking-[0.23em]">
                    com Sites e Sistemas Sob Medida
                </h2>
            </div>
            <div
                class="md:col-span-8 col-span-4 flex flex-col items-center justify-center py-2 md:py-10"
            >
                <button
                    class="bg-black dark:bg-white text-white dark:text-black w-[90%] h-full tracking-[0.23em]"
                >
                    <span
                        class="link vertical-text link-underline link-underline-black text-white dark:text-black text-xs my-10 md:my-0 md:text-xl"
                    >
                        VEJA COMO
                    </span>
                </button>
            </div>
        </div>

        <!-- ---------  -->

        <!-- THIRD ROW -->

        <div
            class="grid grid-cols-12 grid-rows-8 border-black dark:border-white bg-white dark:bg-black dark:text-white border-solid border-[1px]"
        >
            <div
                class="col-span-12 md:col-span-6 row-span-8 flex flex-col gap-16 items-center justify-center py-10 md-border-right"
            >
                <div class="flex flex-col md:flex-row mx-5">
                    <div class="md:max-w-[50%] px-5">
                        <h2 class="md:text-2xl font-bold mb-8">Serviços</h2>
                        <p
                            class="break-all text-base normal-case mb-10 md:mb-0"
                        >
                            Desenvolvimento de sites e sistemas personalizados
                            com Laravel, Vue.js e WordPress, focando em soluções
                            responsivas e inovadoras.
                        </p>
                    </div>
                    <div class="mx-auto flex items-center relative">
                        <div
                            class="absolute w-full py-9 bg-transparent isset-0 z-0"
                        ></div>
                        <button
                            class="border-solid z-10 relative border-white dark:border-black border-[1px] change-bg px-20 py-5 hover:shadow-outline"
                        >
                            Saiba Mais
                        </button>
                    </div>
                </div>

                <hr
                    class="border-solid border-black dark:border-white border-[1px] w-full"
                />
                <div class="flex flex-col md:flex-row mx-5">
                    <div class="md:max-w-[50%] px-5">
                        <h2 class="md:text-2xl font-bold mb-8">
                            Desenvolvimento Web
                        </h2>
                        <p
                            class="break-all text-base normal-case mb-10 md:mb-0"
                        >
                            Elevamos sua presença online com sites responsivos e
                            sistemas personalizados. Utilizando Laravel, Vue.js
                            e WordPress, transformamos suas ideias em realidade
                            digital.
                        </p>
                    </div>
                    <div class="mx-auto flex items-center relative">
                        <div
                            class="absolute w-full py-9 bg-transparent isset-0 z-0"
                        ></div>
                        <button
                            class="border-solid z-10 relative border-black border-[1px] change-bg px-20 py-5 hover:shadow-outline"
                        >
                            Saiba Mais
                        </button>
                    </div>
                </div>
            </div>
            <div
                class="col-span-12 md:col-span-6 row-span-2 py-6 border-bottom md-border-bottom border-top flex change-bg items-center justify-center md:justify-start"
            >
                <h2 class="md:ml-5 md:text-4xl">Explore Nossos Serviços</h2>
            </div>
            <div class="col-span-12 md:col-span-6 relative row-span-6 flex">
                <div class="flex flex-col md:flex-row">
                    <!-- Laravel BOX -->
                    <div
                        class="flex flex-col w-full md:max-w-[50%] justify-center md:mx-5 border-bottom md-border-right"
                    >
                        <div class="py-5 md:py-0 px-5">
                            <h2 class="text-2xl md:text-3xl mb-8">
                                Desenvolvimento Personalizado
                            </h2>
                            <p class="break-all text-base normal-case">
                                Utilizamos Laravel para criar sistemas robustos
                                e personalizados, atendendo às necessidades
                                específicas do seu negócio.
                            </p>
                        </div>
                        <div class="relative mx-auto md:mx-0 mb-10 md:mb-0">
                            <button
                                class="border-solid z-10 mt-14 md:ml-5 change-bg px-5 py-1 md:px-20 md:py-5 hover:shadow-outline"
                            >
                                SAIBA MAIS
                            </button>
                        </div>
                    </div>
                    <!-- Vue.js BOX -->
                    <div
                        class="flex flex-col w-full md:max-w-[50%] justify-center md:mx-5"
                    >
                        <div class="py-5 md:py-0 px-5">
                            <h2 class="text-2xl md:text-3xl mb-8">
                                Interfaces Dinâmicas
                            </h2>
                            <p class="break-all text-base normal-case">
                                Com Vue.js, desenvolvemos interfaces interativas
                                e responsivas, proporcionando uma experiência de
                                usuário sem igual.
                            </p>
                        </div>
                        <div class="relative mx-auto md:mx-0 mb-10 md:mb-0">
                            <button
                                class="border-solid z-10 mt-14 md:ml-5 change-bg px-5 py-1 md:px-20 md:py-5 hover:shadow-outline"
                            >
                                SAIBA MAIS
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- ---------  -->

        <!-- FOURTH ROW -->

        <div
            class="grid grid-cols-6 border-black border-t-transparent border-b-transparent dark:border-white border-solid border-[1px]"
        >
            <div class="col-span-1">
                <ImgComparisonSlider class="h-1/2 flex">
                    <!-- eslint-disable -->
                    <img
                        slot="first"
                        class="h-full"
                        src="../../img/Photo2_B.jpg"
                    />
                    <img
                        slot="second"
                        class="h-full"
                        src="../../img/Photo2_A.jpg"
                    />
                    <!-- eslint-enable -->
                </ImgComparisonSlider>
                <ImgComparisonSlider class="h-1/2 flex">
                    <!-- eslint-disable -->
                    <img
                        slot="first"
                        class="h-full"
                        src="../../img/Photo3_B.jpg"
                    />
                    <img
                        slot="second"
                        class="h-full"
                        src="../../img/Photo3_A.jpg"
                    />
                    <!-- eslint-enable -->
                </ImgComparisonSlider>
            </div>
            <div class="col-span-1">
                <ImgComparisonSlider class="h-1/2 flex">
                    <!-- eslint-disable -->
                    <img
                        slot="first"
                        class="h-full"
                        src="../../img/Photo4_B.jpg"
                    />
                    <img
                        slot="second"
                        class="h-full"
                        src="../../img/Photo4_A.jpg"
                    />
                    <!-- eslint-enable -->
                </ImgComparisonSlider>
                <ImgComparisonSlider class="h-1/2 flex">
                    <!-- eslint-disable -->
                    <img
                        slot="first"
                        class="h-full"
                        src="../../img/Photo5_B.jpg"
                    />
                    <img
                        slot="second"
                        class="h-full"
                        src="../../img/Photo5_A.jpg"
                    />
                    <!-- eslint-enable -->
                </ImgComparisonSlider>
            </div>
            <div class="col-span-2 h-full">
                <!-- <div
                    class="absolute text-white dark:bg-black bg-gray-600 bottom-0 max-w-[60%] m-4 p-2 opacity-60"
                >
                    <h2 class="text-2xl mb-5">Title</h2>
                    <p class="text-sm normal-case">
                        Lorem ipsum dolor, sit amet consectetur adipisicing
                        elit.
                    </p>
                </div> -->
                <ImgComparisonSlider class="h-full flex">
                    <!-- eslint-disable -->
                    <img
                        slot="first"
                        class="h-full"
                        src="../../img/Photo1_B.jpg"
                    />
                    <img
                        slot="second"
                        class="h-full"
                        src="../../img/Photo1_A.jpg"
                    />
                    <!-- eslint-enable -->
                </ImgComparisonSlider>
            </div>
            <div class="col-span-1">
                <ImgComparisonSlider class="h-1/2 flex">
                    <!-- eslint-disable -->
                    <img
                        slot="first"
                        class="h-full"
                        src="../../img/Photo5_B.jpg"
                    />
                    <img
                        slot="second"
                        class="h-full"
                        src="../../img/Photo5_A.jpg"
                    />
                    <!-- eslint-enable -->
                </ImgComparisonSlider>
                <ImgComparisonSlider class="h-1/2 flex">
                    <!-- eslint-disable -->
                    <img
                        slot="first"
                        class="h-full"
                        src="../../img/Photo5_B.jpg"
                    />
                    <img
                        slot="second"
                        class="h-full"
                        src="../../img/Photo5_A.jpg"
                    />
                    <!-- eslint-enable -->
                </ImgComparisonSlider>
            </div>
            <div class="col-span-1">
                <ImgComparisonSlider class="h-1/2 flex">
                    <!-- eslint-disable -->
                    <img
                        slot="first"
                        class="h-full"
                        src="../../img/Photo5_B.jpg"
                    />
                    <img
                        slot="second"
                        class="h-full"
                        src="../../img/Photo5_A.jpg"
                    />
                    <!-- eslint-enable -->
                </ImgComparisonSlider>
                <ImgComparisonSlider class="h-1/2 flex">
                    <!-- eslint-disable -->
                    <img
                        slot="first"
                        class="h-full"
                        src="../../img/Photo5_B.jpg"
                    />
                    <img
                        slot="second"
                        class="h-full"
                        src="../../img/Photo5_A.jpg"
                    />
                    <!-- eslint-enable -->
                </ImgComparisonSlider>
            </div>
        </div>

        <!-- ---------  -->

        <!-- FIFTH ROW -->

        <div
            class="grid grid-cols-6 dark:bg-black dark:text-white border-black dark:border-white border-solid border-[1px]"
        >
            <div class="col-span-6 md:col-span-1 md-border-right">
                <div
                    class="flex w-full justify-between box-decoration-slice md:flex-col md:h-full border-bottom"
                >
                    <button
                        class="change-bg text-center md:text-start md:pl-2 py-3 md:py-0 md-border-bottom border-right w-1/3 md:w-auto md:h-1/3"
                    >
                        NOSSOS PROJETOS
                    </button>
                    <button
                        class="change-bg text-center md:text-start md:pl-2 md-border-bottom border-right w-1/3 md:w-auto md:h-1/3"
                    >
                        CONTATO
                    </button>
                    <button
                        class="change-bg text-center dark:border-white md:text-start md:pl-2 w-1/3 md:w-auto md:h-1/3"
                    >
                        SOBRE NÓS
                    </button>
                </div>
            </div>

            <div
                class="col-span-6 md:col-span-1 border-bottom md-border-right flex flex-col items-center justify-center change-bg"
            >
                <h2 class="md:mx-2 text-center md:text-2xl">
                    Formulario de <br />
                    Contato
                </h2>
            </div>
            <div class="col-span-6 md:col-span-4 h-full pt-4 px-4">
                <form action="">
                    <div class="flex gap-10">
                        <input
                            type="text"
                            class="bg-transparent border-black dark:border-white border-solid border-[1px] w-[50%]"
                            placeholder=" Name"
                        />
                        <input
                            type="text"
                            class="bg-transparent border-black dark:border-white border-solid border-[1px] w-[50%] py-2"
                            placeholder=" E-mail"
                        />
                    </div>

                    <textarea
                        name=""
                        id=""
                        rows="5"
                        class="bg-transparent mt-10 border-black dark:border-white border-solid border-[1px] w-full"
                        placeholder=" Message"
                    ></textarea>

                    <div class="flex w-full justify-end">
                        <button
                            class="change-bg px-5 py-2 border-solid border-black dark:border-white border-[1px] self-end mt-5 mb-4"
                        >
                            ENVIAR
                        </button>
                    </div>
                </form>
            </div>
        </div>

        <!-- ---------  -->

        <!-- SIXTH ROW -->
        <div
            class="w-full flex items-center justify-center py-5 bg-black text-white change-bg select-none"
        >
            <p class="text-center">
                Direitos Autorais © 2024 SkySet por Nicro01
            </p>
        </div>
    </div>
</template>

<script>
import { ImgComparisonSlider } from "@img-comparison-slider/vue";

export default {
    data() {
        return {
            isDarkMode: false,
        };
    },
    components: {
        ImgComparisonSlider,
    },
    methods: {
        toggleDarkMode() {
            this.isDarkMode = !this.isDarkMode;
            document.querySelector("html").classList.toggle("dark");
        },
    },
};
</script>

<style scoped>
@media (min-width: 768px) {
    .md-border-right {
        border-right: 1px solid black;
    }

    .md-border-bottom {
        border-bottom: 1px solid black;
    }

    .md-border-left {
        border-left: 1px solid black;
    }

    .md-border-top {
        border-top: 1px solid black;
    }
}

@media (max-width: 768px) {
    .vertical-text {
        writing-mode: vertical-rl;
        text-orientation: upright;
    }
    .border-right {
        border-right: 1px solid black !important;
    }

    .border-bottom {
        border-bottom: 1px solid black;
    }

    .border-left {
        border-left: 1px solid black;
    }

    .border-top {
        border-top: 1px solid black;
    }
}

.dark .md-border-right {
    border-right: 1px solid white;
}

.dark .md-border-bottom {
    border-bottom: 1px solid white;
}

.dark .md-border-left {
    border-left: 1px solid white;
}

.dark .md-border-top {
    border-top: 1px solid white;
}

.dark .border-right {
    border-right: 1px solid white;
}

.dark .border-bottom {
    border-bottom: 1px solid white;
}

.dark .border-left {
    border-left: 1px solid white;
}

.dark .border-top {
    border-top: 1px solid white;
}

.change-bg:hover {
    background-color: black;
    color: white;
}

.dark .change-bg:hover {
    background-color: white;
    color: black;
}

.grid div {
    box-sizing: border-box;
}
.link-underline {
    border-bottom-width: 0;
    background-image: linear-gradient(transparent, transparent),
        linear-gradient(#000, #000);
    background-size: 100% 1px;
    background-position: 0 100%;
    background-repeat: no-repeat;
    transition: background-size 0.3s ease-in-out;
}

.dark .link-underline {
    background-image: linear-gradient(transparent, transparent),
        linear-gradient(#fff, #fff);
}

.link-underline-black {
    background-image: linear-gradient(transparent, transparent),
        linear-gradient(#fff, #fff);
}

.dark .link-underline-black {
    background-image: linear-gradient(transparent, transparent),
        linear-gradient(#000, #000);
}

.link-underline:hover {
    background-size: 0 1px;
    background-position: 10 0%;
}

.hover\:shadow-outline:hover {
    box-shadow: 0 0 0 1px #000, 0 0 0 8px #fff, 0 0 0 9px #000, 0 0 0 16px #fff,
        0 0 0 17px #000;
}

.hover\:shadow-outline:not(:hover) {
    box-shadow: 0 0 0 1px #fff, 0 0 0 8px #fff, 0 0 0 9px #fff, 0 0 0 16px #fff,
        0 0 0 17px #fff;
    animation: shadow-reverse 0.2s ease-in-out forwards;
}

.hover\:shadow-outline {
    border: 1px solid black !important;
    box-shadow: 0 0 0 1px #fff, 0 0 0 8px #fff, 0 0 0 9px #fff, 0 0 0 16px #fff,
        0 0 0 17px #fff;
    animation: shadow 0.2s ease-in-out forwards;
}

@keyframes shadow {
    0% {
        box-shadow: 0 0 0 1px #fff, 0 0 0 8px #fff, 0 0 0 9px #fff,
            0 0 0 16px #fff, 0 0 0 17px #fff;
    }
    50% {
        box-shadow: 0 0 0 1px #000, 0 0 0 8px #fff, 0 0 0 9px #fff,
            0 0 0 16px #000, 0 0 0 17px #fff;
    }
    100% {
        box-shadow: 0 0 0 1px #000, 0 0 0 8px #fff, 0 0 0 9px #000,
            0 0 0 16px #fff, 0 0 0 17px #000;
    }
}

@keyframes shadow-reverse {
    0% {
        box-shadow: 0 0 0 1px #000, 0 0 0 8px #fff, 0 0 0 9px #000;
    }
    50% {
        box-shadow: 0 0 0 1px #000, 0 0 0 8px #fff, 0 0 0 9px #fff;
    }
    100% {
        box-shadow: 0 0 0 1px #fff, 0 0 0 8px #fff, 0 0 0 9px #fff;
    }
}

.dark .hover\:shadow-outline:hover {
    box-shadow: 0 0 0 1px #fff, 0 0 0 8px #000, 0 0 0 9px #fff, 0 0 0 16px #000,
        0 0 0 17px #fff;
}

.dark .hover\:shadow-outline:not(:hover) {
    box-shadow: 0 0 0 1px #000, 0 0 0 8px #000, 0 0 0 9px #000, 0 0 0 16px #000,
        0 0 0 17px #000;
    animation: dark_shadow-reverse 0.2s ease-in-out forwards;
}

.dark .hover\:shadow-outline {
    border: 1px solid white !important;
    box-shadow: 0 0 0 1px #000, 0 0 0 8px #000, 0 0 0 9px #000, 0 0 0 16px #000,
        0 0 0 17px #000;
    animation: dark_shadow 0.2s ease-in-out forwards;
}

@keyframes dark_shadow {
    0% {
        box-shadow: 0 0 0 1px #000, 0 0 0 8px #000, 0 0 0 9px #000,
            0 0 0 16px #000, 0 0 0 17px #000;
    }
    50% {
        box-shadow: 0 0 0 1px #fff, 0 0 0 8px #000, 0 0 0 9px #000,
            0 0 0 16px #fff, 0 0 0 17px #000;
    }
    100% {
        box-shadow: 0 0 0 1px #fff, 0 0 0 8px #000, 0 0 0 9px #fff,
            0 0 0 16px #000, 0 0 0 17px #fff;
    }
}

@keyframes dark_shadow-reverse {
    0% {
        box-shadow: 0 0 0 1px #fff, 0 0 0 8px #000, 0 0 0 9px #fff;
    }
    50% {
        box-shadow: 0 0 0 1px #fff, 0 0 0 8px #000, 0 0 0 9px #000;
    }
    100% {
        box-shadow: 0 0 0 1px #000, 0 0 0 8px #000, 0 0 0 9px #000;
    }
}
</style>
