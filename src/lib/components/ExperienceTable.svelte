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
            company: "Emagia Corporation",
            startDate: "2024-07",
        },
        {
            jobTitle: "Sr. Software Engineer",
            company: "Emagia Corporation",
            startDate: "2018-10",
            endDate: "2024-07"
        },

        {
            jobTitle: "GIS Engineer",
            company: "RMSI Pvt Limited",
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
    <h3 class="headline">Past work <br /> Experience</h3>
</section>