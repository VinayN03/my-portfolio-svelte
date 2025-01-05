<script>
	import { goto } from "$app/navigation";


	import Button from "$components/Button.svelte";

    function onclick() {
        goto("/#contact-form");
    }

</script>
<section class="hero-section default-margin">
    <h5>Hello!</h5><h5 class="ml-s mr-s">I'm</h5><h6>Vinay Kumar Namadi</h6>
    <div class="underscore mb-m"></div>
    <div class="summary mb-m">
        <!-- I am a Python developer with specialized expertise in Machine Learning (ML), Deep Learning (DL), Generative AI, and Natural Language Processing (NLP). -->
    <h4 class="ml-xs">I'm a</h4><h2> Python developer </h2><h4>with specialized expertise in</h4><h2>Machine Learning</h2><h4 class="ml-xs">,</h4>
        <h2>Deep Learning</h2><h4 class="ml-xs">,</h4><h2> Generative AI </h2><h4>and</h4>
    <h2 class="dark-grey">Natural Language Processing</h2>
</div>
    <Button {onclick}>Let's Talk</Button>
</section>

<style>
    .hero-section {
        padding-top: 40px;
    }


</style>