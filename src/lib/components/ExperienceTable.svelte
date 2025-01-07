<script lang="ts">
    interface WorkExperience {
        jobTitle: string;
        company: string;
        startDate: string;
        endDate?: string;
    }

    const workExperience: WorkExperience[] = [
        {
            jobTitle: "Software Developer",
            company: "Emagia Corporation - Lewisville, TX, USA",
            startDate: "2024-07",
        },
        {
            jobTitle: "Sr. Software Engineer",
            company: "Emagia Corporation - Hyderabad, INDIA",
            startDate: "2018-10",
            endDate: "2024-07"
        },

        {
            jobTitle: "GIS Engineer",
            company: "RMSI Pvt Limited - Hyderabad, INDIA",
            startDate: "2016-12",
            endDate: "2018-06"
        },
    ];
</script>

<section class="work-experience mt-l mb-l">
    <div class="work-experience-div">
    <ul class="work-experience-list">
        {#each workExperience as job}
        <li class="work-item">
            <artcle>
                <h6 class="semi-bold mb-xs">{job.jobTitle}</h6>
                <div class="company-and-date">
                    <p>{job.company}</p>
                    <p class="dark-grey">
                        {job.startDate}
                        {#if job.endDate}
                        / {job.endDate}
                        {:else}
                        / present
                        {/if}
                    </p>
                </div>
            
            </artcle>
        </li>
        {/each}

    </ul>
    <h3 class="headline">Work <br /> Experience</h3>
</div>
</section>

<style>
    .work-experience {
        background-color: #ffffff;
        width: 100%;
        margin: 0px auto;
        padding-top: 30px;
    }

    .work-experience-div {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-evenly;
        width: 80%;
        margin: 30px auto;
        margin-bottom: 60px;
    }

    .work-experience-list {
        width: 50%;
    }

    .headline {
        text-align: right;
        margin-top: 90px;  
    }

    .work-item {
        border-bottom: 1px solid #f0eded;
        padding-bottom: 12px;
        max-width: 500px;

    }

    .work-item:not(:first-of-type) {
        padding-top: 16px;
    }

    .work-item p {
        margin-bottom: 0;
    }

    .company-and-date {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
    }

    @media (max-width: 800px) {
    .work-experience-list {
        width: 80%;
        margin: 0 auto;
    }

    .headline {
        font-size: 30px;
        margin-top: 20px;
    }

}
</style>