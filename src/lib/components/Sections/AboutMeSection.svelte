<script lang="ts">

	import SectionHeadline from "$components/SectionHeadline.svelte";
    import image from "$assets/about-me.jpg";

</script>


<section class="about-me mt-l">
    <SectionHeadline sectionName={"about-me"}>About Me</SectionHeadline>
    <div class="mt-m content-container default-margin">
        <img class="image" src={image} alt="" />
        <div class="text">
            <p>
                I am a Python developer with specialized expertise in Machine Learning (ML), Deep Learning (DL), Generative AI, and Natural Language Processing (NLP). With a strong foundation in designing, implementing, and optimizing complex algorithms, I focus on leveraging cutting-edge AI technologies to build intelligent, data-driven solutions. My experience includes developing custom ML models, training deep neural networks, implementing NLP pipelines, and creating innovative generative AI applications. I am passionate about transforming data into actionable insights and delivering scalable AI solutions.
            </p>
        </div>
    </div>
</section>
