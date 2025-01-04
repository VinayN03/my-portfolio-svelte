<script>
	import { goto } from "$app/navigation";


	import Button from "$components/Button.svelte";

    function onclick() {
        goto("/#contact-form");
    }

</script>
<section class="hero-section default-margin">
    <h3>Hello! I'm Vinay</h3>
    <div class="underscore mb-m"></div>
    <h2>I'm a Python developer with expertise in Artificial Intelligence, Machine Learning, 
        Deep Learning and 
    </h2>
    <h2 class="dark-grey">Natural Language Processing</h2>
    <Button {onclick}>Let's Talk</Button>
</section>

<style>
    .hero-section {
        padding-top: 60px;
    }
</style>