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
            startDate: "2018-10",
            endDate: "2024-07"
        },
    ];
</script>

<section class="default-margin work-experience mt-m">
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
                        {job.endDate}
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
</section>

<style>
    .work-experience {
        display: flex;
        justify-content: space-between;
        width: 100%;
    }

    .work-experience-list {
        width: 50%;
    }

    .headline {
        text-align: right;
        margin-top: 90px;
        margin-right: 120px;
        
    }

    .work-item {
        border-bottom: 1px solid #f0eded;
        padding-bottom: 12px;
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
    }
</style>