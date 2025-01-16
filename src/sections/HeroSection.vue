<script setup></script>

<template>
    <!-- Hero Section Start -->
    <div class="container mx-auto px-5 overflow-x-hidden lg:overflow-x-visible h-[100vh] flex items-center" id="about">
        <section class="grid grid-cols-none lg:grid-cols-2 pb-16 pt-8 items-center">
            <div class="lg:w-5/6 order-2 lg:order-none flex flex-col justify-center">
                <h1 class="text-4xl xl:text-5xl font-bold font-theme-heading text-left"><span class=" bg-blue-700 px-2">Binary</span> Needle</h1>
                <p class="lg:text-xl mt-10 font-theme-content text-theme-grayish-blue text-left">A clean and simple interface to organize your favourite websites. Open a new browser tab and see your sites load instantly. Try it for free.</p>
                <div class="flex justify-start mt-10">
                    <LinkButton btnType="primary" link="#download-section">Get It On Chrome</LinkButton>
                    <LinkButton btnType="muted" link="#download-section">Get It On Firefox</LinkButton>
                </div>
            </div>
            <div class="relative order-1 lg:order-none mb-20 lg:mt-0 lg:mb-0 lg:-mr-10">
                <div class="-z-10 bg-theme-primary h-52 w-full sm:h-80 sm:w-full rounded-l-full absolute -right-28 md:-right-48 -bottom-8"></div>
            </div>
        </section>
    </div>
    <!-- Hero Section End -->
</template>