<script setup>
    const testimonials = [
        {
            picture: "alex",
            name: "Alex",
            company: "ApolloNet",
            review: "Sed ut perspiciatis unde omnis iste natus sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quaeab illo inventore veritatis et quasi architectobeatae vitae dicta sunt explicabo.",
        },
        {
            picture: "benjamin",
            name: "Benjamin",
            company: "SINGULART",
            review: "Sed ut perspiciatis unde, totam rem aperiam, eaque ipsa quaeab illo inventore veritatis et quasi architectobeatae vitae dicta sunt explicabo.",
        },
        {
            picture: "sandrine",
            name: "Sandrine",
            company: "gîte La Souris des Champs",
            review: "Sed ut perspiciatis unde omnis iste natus sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quaeab illo inventore veritatis et quasi architectobeatae vitae dicta sunt explicabo.",
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
                src="https://picsum.photos/id/127/1920/1080"
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
