<script lang="ts">
    import { SectionHeadline } from "$components";
</script>

<section class="contact-section mt-l">
    <div class="contact-div">
    <SectionHeadline sectionName={"contact-me"}>Contact Me</SectionHeadline>

    <div class="default-margin mt-m contact-details dark-grey">
    <p> vinaykumar.namadi@gmail.com </p>
    <p>+1 945 267 7514</p>
    <p>Plano, Texas, 75024 </p>
</div>
</div>
</section>

<style>
    .contact-section {
        background-color: #fbfbfb;
        padding: 30px 0px;
        display: flex;
        justify-content: center;
        width: 100%;
        margin: 0 auto;
    }

    .contact-div {
        width: 100%;

    }

     .contact-details {
        padding-top: 30px;
        display: block;
        text-align: center;
        
    }
    .contact-details p{
        padding: 0;
        margin: 0;
        font-size: 18px;
    }

    .contact-details p:last-of-type{
        margin-bottom: 100px;
    } 
    
</style>