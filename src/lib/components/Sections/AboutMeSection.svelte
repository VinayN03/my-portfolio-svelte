<script lang="ts">

	import { SectionHeadline, ExperienceTable } from "$components";
    import image from "$assets/about-me.jpg";

</script>


<section class="about-me mt-l">
    <SectionHeadline sectionName={"about-me"}>About Me</SectionHeadline>
    <div class="mt-m content-container default-margin">
        <img class="image" src={image} alt="" />
        <div class="text">
            <p>
                I am a results-driven Python developer with over 7.5 years of experience specializing in Machine Learning (ML), Deep Learning (DL), Natural Language Processing (NLP), and Generative AI. Throughout my career, I have developed a strong foundation in designing and implementing innovative AI solutions, focusing on transforming data into actionable insights. My experience spans across various domains, including document data extraction, optical character recognition (OCR), Named Entity Recognition (NER), and cloud-based services using AWS. I have worked with open-source LLMs and advanced deep learning algorithms to automate complex tasks and improve operational efficiency. Additionally, I am well-versed in developing REST APIs, working with databases like MySQL and Oracle, and optimizing cloud infrastructure. I thrive in dynamic environments and excel in leading teams to deliver scalable and high-performance solutions. Passionate about continuous learning, I am always eager to explore emerging technologies and apply them to real-world challenges.
            </p>
        </div>
    </div>
    <ExperienceTable />
</section>

<style>
    .content-container {
        display: flex;
        justify-content: space-between;
        align-items: stretch;
    }

    .image {
        width: 42%;
        border-radius: 20px;
        object-fit: cover;
    }

    .text {
        width: 55%;
        text-align: left;
    }
</style>
