<template>
    <div
        :class="{ dark: isDarkMode }"
        class="dark:bg-black bg-white min-h-screen p-2 dark:text-white text-black select-none uppercase"
    >
        <div
            class="w-16 h-8 z-50 fixed right-5 flex items-center bg-gray-300 rounded-full p-1 cursor-pointer"
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
                class="col-span-8 box-decoration-slice flex items-center change-bg justify-center pb-2 border-right"
            >
                <h2 class="text-8xl tracking-[0.6em] break-words">webgeni</h2>
                <h2 class="text-8xl -ml-2">e</h2>
            </div>
            <div class="col-span-2 border-right">
                <div
                    class="flex box-decoration-slice flex-col justify-between h-full"
                >
                    <button
                        class="py-2 change-bg text-start pl-2 border-bottom"
                    >
                        FEATURES
                    </button>
                    <button
                        class="py-2 change-bg text-start pl-2 border-bottom"
                    >
                        SERVICES
                    </button>
                    <button class="py-2 change-bg text-start pl-2">
                        PRICES
                    </button>
                </div>
            </div>
            <div class="col-span-2 box-decoration-slice">
                <button class="py-2 change-bg h-full mx-auto w-full">
                    CONTACT
                </button>
            </div>
        </div>

        <!-- ---------  -->

        <!-- SECOND ROW -->

        <div
            class="grid grid-cols-12 bg-white border-black dark:border-white border-t-transparent dark:bg-black border-solid border-[1px]"
        >
            <div
                class="col-span-4 flex flex-col dark:text-white items-center justify-center change-bg py-10 border-right"
            >
                <h2 class="text-5xl tracking-[0.28em] break-words">
                    A Brutalist
                </h2>
                <h2 class="text-4xl tracking-[0.23em]">HTML 5 Template</h2>
            </div>
            <div
                class="col-span-8 flex flex-col items-center justify-center py-10"
            >
                <button
                    class="bg-black dark:bg-white text-white dark:text-black w-[90%] h-full tracking-[0.23em]"
                >
                    <span
                        class="link link-underline link-underline-black text-white dark:text-black text-xl"
                    >
                        SEE PROJECTS</span
                    >
                </button>
            </div>
        </div>

        <!-- ---------  -->

        <!-- THIRD ROW -->

        <div
            class="grid grid-cols-12 grid-rows-8 border-black dark:border-white bg-white dark:bg-black dark:text-white border-solid border-[1px]"
        >
            <div
                class="col-span-6 row-span-8 flex flex-col gap-16 items-center justify-center py-10 border-right"
            >
                <div class="flex mx-5">
                    <div class="max-w-[50%] px-5">
                        <h2 class="text-4xl mb-8">Responsive</h2>
                        <p class="break-all text-base normal-case">
                            Websites and web applications that are not only
                            fully responsive and mobile-friendly but also
                            tailored to your unique needs.
                        </p>
                    </div>
                    <div class="mx-auto flex items-center relative">
                        <div
                            class="absolute w-full py-9 bg-transparent isset-0 z-0"
                        ></div>
                        <button
                            class="border-solid z-10 relative border-white dark:border-black border-[1px] change-bg px-20 py-5 hover:shadow-outline"
                        >
                            READ MORE
                        </button>
                    </div>
                </div>
                <hr
                    class="border-solid border-black dark:border-white border-[1px] w-full"
                />
                <div class="flex mx-5">
                    <div class="max-w-[50%] px-5">
                        <h2 class="text-4xl mb-8">RESPONSIVE</h2>
                        <p class="break-all text-base normal-case">
                            Lorem ipsum dolor sit amet, consectetur adipiscing
                            elit, sed do eiusmod tempor. Incididunt ut labore et
                            dolore magna aliqua.
                        </p>
                    </div>
                    <div class="mx-auto flex items-center relative">
                        <div
                            class="absolute w-full py-9 bg-transparent isset-0 z-0"
                        ></div>
                        <button
                            class="border-solid z-10 relative border-black border-[1px] change-bg px-20 py-5 hover:shadow-outline"
                        >
                            READ MORE
                        </button>
                    </div>
                </div>
            </div>
            <div
                class="col-span-6 row-span-2 py-6 border-bottom flex change-bg items-center"
            >
                <h2 class="ml-5 text-5xl">There are features</h2>
            </div>
            <div class="col-span-6 relative row-span-6 border-bottom flex">
                <div class="flex">
                    <!-- HTML 5 BOX -->

                    <div
                        class="flex flex-col max-w-[50%] justify-center mx-5 border-right"
                    >
                        <div class="px-5">
                            <h2 class="text-4xl mb-8">HTML 5</h2>
                            <p class="break-all text-base normal-case">
                                Lorem ipsum dolor sit amet, consectetur
                                adipiscing elit, sed do eiusmod tempor.
                                Incididunt ut labore et dolore magna aliqua.
                            </p>
                        </div>
                        <div class="relative">
                            <button
                                class="border-solid z-10 mt-14 ml-5 change-bg px-20 py-5 hover:shadow-outline"
                            >
                                READ MORE
                            </button>
                        </div>
                    </div>

                    <!-- -------- -->

                    <!-- CSS 3 BOX -->

                    <div class="flex flex-col max-w-[50%] justify-center mx-5">
                        <div class="px-5">
                            <h2 class="text-4xl mb-8">CSS 3</h2>
                            <p class="break-all text-base normal-case">
                                Lorem ipsum dolor sit amet, consectetur
                                adipiscing elit, sed do eiusmod tempor.
                                Incididunt ut labore et dolore magna aliqua.
                            </p>
                        </div>
                        <div class="relative">
                            <button
                                class="border-solid z-10 mt-14 ml-5 change-bg px-20 py-5 hover:shadow-outline"
                            >
                                READ MORE
                            </button>
                        </div>
                    </div>

                    <!-- --------- -->
                </div>
            </div>
        </div>

        <!-- ---------  -->

        <!-- FOURTH ROW -->

        <div class="grid grid-cols-6 border-white border-solid border-[1px]">
            <div class="col-span-1">
                <img
                    draggable="false"
                    src="https://placehold.co/300x300"
                    width="300"
                    height="300"
                    alt=""
                />
                <img
                    draggable="false"
                    src="https://placehold.co/300x300"
                    width="300"
                    height="300"
                    alt=""
                />
            </div>
            <div class="col-span-1">
                <img
                    draggable="false"
                    src="https://placehold.co/300x300"
                    width="300"
                    height="300"
                    alt=""
                />
                <img
                    draggable="false"
                    src="https://placehold.co/300x300"
                    width="300"
                    height="300"
                    alt=""
                />
            </div>
            <div class="col-span-2 h-full relative">
                <div
                    class="absolute text-white dark:bg-black bg-gray-600 bottom-0 max-w-[60%] m-4 p-2 opacity-60"
                >
                    <h2 class="text-2xl mb-5">Title</h2>
                    <p class="text-sm normal-case">
                        Lorem ipsum dolor, sit amet consectetur adipisicing
                        elit.
                    </p>
                </div>
                <img
                    draggable="false"
                    src="https://placehold.co/600x600"
                    width="600"
                    height="600"
                    alt=""
                />
            </div>
            <div class="col-span-1">
                <img
                    draggable="false"
                    src="https://placehold.co/300x300"
                    width="300"
                    height="300"
                    alt=""
                />
                <img
                    draggable="false"
                    src="https://placehold.co/300x300"
                    width="300"
                    height="300"
                    alt=""
                />
            </div>
            <div class="col-span-1">
                <img
                    draggable="false"
                    src="https://placehold.co/300x300"
                    width="300"
                    height="300"
                    alt=""
                />
                <img
                    draggable="false"
                    src="https://placehold.co/300x300"
                    width="300"
                    height="300"
                    alt=""
                />
            </div>
        </div>

        <!-- ---------  -->

        <!-- FIFTH ROW -->

        <div
            class="grid grid-cols-6 dark:bg-black dark:text-white border-black dark:border-white border-solid border-[1px]"
        >
            <div class="col-span-1 border-right">
                <div class="flex box-decoration-slice flex-col h-full">
                    <button
                        class="change-bg text-start pl-2 border-bottom h-1/3"
                    >
                        GITHUB
                    </button>
                    <button
                        class="change-bg text-start pl-2 border-bottom h-1/3"
                    >
                        INSTAGRAM
                    </button>
                    <button class="change-bg text-start pl-2 h-1/3">
                        WHATSAPP
                    </button>
                </div>
            </div>
            <div
                class="col-span-1 border-right flex flex-col items-center justify-center change-bg"
            >
                <h2 class="text-start text-3xl">CONTACT</h2>
            </div>
            <div class="col-span-4 h-full p-10">
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
                            class="change-bg px-5 py-2 border-solid border-black dark:border-white border-[1px] self-end mt-10"
                        >
                            SEND
                        </button>
                    </div>
                </form>
            </div>
        </div>

        <!-- ---------  -->

        <!-- SIXTH ROW -->
    </div>
    <div
        class="w-full flex items-center justify-center py-5 bg-black text-white change-bg select-none"
    >
        <p class="text-center">
            Copyright © 2024 Brutalism Portfolio by Nicro01
        </p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            isDarkMode: false,
        };
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
.border-right {
    border-right: 1px solid black;
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
