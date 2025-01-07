<script lang="ts">

	import { SectionHeadline, ExperienceTable } from "$components";
    import image from "$assets/about-me.jpg";

</script>


<section class="about-me mt-l mb-l">
    <SectionHeadline sectionName={"about-me"}>About Me</SectionHeadline>
    <div class="content-container default-margin mt-m mb-m">
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
    .about-me {
        width: 100%;
        background-color: #fbfbfb;
        margin: 0 auto;
        margin-top: 60px;
        padding-top: 40px;
    }

    .content-container {
        width: 80%;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-evenly;
        align-items: stretch;
        padding-bottom: 60px;


    }

    .image {
        max-width: 400px;
        border-radius: 20px;
        object-fit: cover;
        margin: 20 auto;
    }

    .text {
        max-width: 550px;
        margin: 20px auto;
    }

    .text p {
        font-size: 18px;
        text-align: left;
    }

    @media (max-width: 800px) {
    .image {
        width: 90%;
        margin: 0 auto;
    }

    .text p {
        width: 100%;
        margin: 20px auto;
        text-align: center;
    }
}
</style>
