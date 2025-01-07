<script lang="ts">

    let certifications = [
        {
            title: "Foundations of Artificial Intelligence and Machine Learning",
            from: "International Institute of Information Technology (IIIT), Hyderabad"
        },

        {
            title: "Deep Learning Specialization",
            from: "Coursera"
        },

        {
            title: "Generative AI with Large Language Models",
            from: "Coursera"
        },

        {
            title: "Generative AI LLMs",
            from: "Nvidia"
        },

        {
            title: "Master Svelte 5 & SvelteKit – Build & Deploy Real-World Apps",
            from: "Udemy"
        }
    ]
</script>

<section class="certification mt-m">
    <h3 class="cert-headline">Certifications</h3>
    <ul class="certification-list">
        {#each certifications as cert}
        <li class="cert-item">
            <artcle>
                <h6 class="semi-bold mb-xs">{cert.title}</h6>
                <div class="cert-from">
                    <p class="dark-grey">
                        {cert.from}
                    </p>
                </div>
            </artcle>
        </li>
        {/each}

    </ul>
</section>

<style>
    .certification {
        width: 80%;
        margin: 60px auto;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-evenly;
        align-items: center;
        border: 1px solid #f0eded;
        border-radius: 10px;
        padding: 30px 15px;
    }

    .certification-list {
        width: 50%;
    }

    .cert-headline {
        text-align: center;
        /* margin-left: 80px;  */
        /* margin-right: 0;   */
    }

    .cert-item:not(:last-of-type) {
        border-bottom: 1px solid #f0eded;
        padding-bottom: 8px;
    }

    .cert-item:not(:first-of-type) {
        padding-top: 12px;
    }

    .cert-item p {
        margin-bottom: 0;
    }

    .cert-from {
        display: flex;
        justify-content: left;
    }

    @media (max-width: 800px) {
    .certification-list {
        width: 90%;
    }

    .cert-headline {
        width: 100%;
        margin: 0 auto;
        padding-bottom: 30px;
    }
}
</style>