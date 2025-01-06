<script>
	import { goto } from "$app/navigation";


	import Button from "$components/Button.svelte";

    function onclick() {
        goto("/#contact-form");
    }

</script>
<section class="hero-section">
    <h5 class="ml-l">Hello!</h5><h5 class="ml-s mr-s">I'm</h5><h6>VINAY</h6>
    <div class="underscore mb-m ml-l"></div>
    <div class="summary mb-m">
        <!-- I am a Python developer with specialized expertise in Machine Learning (ML), Deep Learning (DL), Generative AI, and Natural Language Processing (NLP). -->
    <h4 class="ml-xs">I'm a</h4><h2> Python Developer </h2><h4>with specialized expertise in</h4><h2 class="dark-grey">Machine Learning</h2><h4 class="ml-xs">,</h4>
        <h2>Deep Learning</h2><h4 class="ml-xs">,</h4><h2 class="dark-grey">Generative AI</h2><h4>and</h4>
    <h2>Natural Language Processing</h2>
</div>
<div class='contact-me-button'>
    <Button {onclick}>Contact Me</Button>
</div>
</section>

<style>
    .hero-section {
        width: 100%;
        padding-top: 40px;
        margin-left: 20px;
        margin-right: 20px;
    }

    .summary {
        width: 100%;
        text-align: center;
    }

    .contact-me-button {
        display: flex;
        justify-content: center;
    }


</style>