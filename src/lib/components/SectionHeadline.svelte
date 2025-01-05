<script lang="ts">
    import type { Snippet } from "svelte";

    interface SectionHeadlineProps {
        children: Snippet;
        sectionName: string;
    }

    let { children, sectionName}: SectionHeadlineProps = $props();
</script>

<div class="default-margin">
    <h6>
        {@render children()}
    </h6>
    <div class="underscore"></div>
</div>