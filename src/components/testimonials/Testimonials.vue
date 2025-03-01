<script setup>
    const testimonials = [
        {
            picture: "mathias",
            name: "Mathias",
            company: "Caféine Web",
            review: "Lucie s'est intégrée au projet avec aisance, faisant preuve d'efficacité, d'aisance technique, de réactivité et d'une grande précision dans le design et l'intégration des projets, ce fut un plaisir de travailler ensemble.",
        },
        {
            picture: "alexandre",
            name: "Alexandre",
            company: "Backmarket",
            review: "Je recommande vivement Lucie comme développeuse front end. Au cours de notre collaboration de deux ans, elle a toujours fait preuve d'une approche proactive, axée sur la recherche de solutions. Lucie sait s'adapter au changement, elle est rigoureuse dans l'exécution.",
        },
        {
            picture: "frederic",
            name: "Frédéric",
            company: "SINGULART",
            review: "Techniquement compétente et extrêmement douée en communication, Lucie a constamment apporté des solutions créatives et des implémentations pertinentes à nos projets. Son enthousiasme et sa volonté d'apprendre sont contagieux, apportant une énergie positive et dynamisante à toute l'équipe.",
        },
    ];
</script>

<template>
    <section class="testimonials">
        <div
            v-for="(testimonial, index) in testimonials"
            :key="index"
            class="testimonial"
        >
            <img
                class="testimonial__image"
                :src="
                    '/public/images/testimonials/' +
                    testimonial.picture +
                    '.jpg'
                "
                alt=""
            />
            <h2 class="testimonial__reviewer discrete">
                {{ testimonial.name }},
                {{ testimonial.company }}
            </h2>
            <p class="heading-3">
                " {{ testimonial.review }} "
            </p>
        </div>
    </section>
</template>
