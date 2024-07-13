<script setup>
import AppLayout from "@/Layouts/AppLayout.vue";
import { Link } from "@inertiajs/vue3";

defineProps({
    canLogin: {
        type: Boolean,
    },
    canRegister: {
        type: Boolean,
    },
    laravelVersion: {
        type: String,
        required: true,
    },
    phpVersion: {
        type: String,
        required: true,
    },
});
</script>

<template>
    <AppLayout title="Strona Domowa">
        <div class="max-w-7xl mx-auto sm:px-6 lg:px-8">
            <!--  Hero Section -->
            <section
                class="bg-primary-50 bg-dotted-pattern bg-contain py-5 md:py-10"
            >
                <div
                    class="wrapper grid grid-cols-1 gap-5 md:grid-cols-2 2xl:gap-0"
                >
                    <div class="flex flex-col justify-center gap-8">
                        <h1 class="h1-bold">
                            Znajdź Przyjaciela w
                            <span style="color: #1493e2">Animal Shelter</span>
                            na Całe Życie!
                        </h1>
                        <p>
                            Otwórz swoje serce i dom dla wyjątkowych zwierząt z
                            naszego schroniska Animal Shelter. Nasz zespół
                            specjalistów pomoże Ci znaleźć idealnego towarzysza,
                            który wprowadzi radość i miłość do Twojego życia.
                            Kliknij poniżej, aby rozpocząć proces adopcji i
                            zmienić życie jednego z naszych podopiecznych na
                            lepsze.
                        </p>
                        <button
                            class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded-full"
                        >
                            <Link href="#">Adoptuj</Link>
                        </button>
                    </div>
                    <img
                        width="1000"
                        height="1000"
                        src="../assets/hero-section.svg"
                        alt="Hero Logo"
                        className="max-h-[70vh] object-contain object-center 2xsl:max-h-[50vh]"
                    />
                </div>
            </section>
        </div>
    </AppLayout>
</template>
