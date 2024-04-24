<script lang="ts">
    import { Button } from "$lib/components/ui/button";
    import Arrow from "lucide-svelte/icons/corner-down-left";
    import Terminal from "lucide-svelte/icons/terminal";

    export let name: string;
    export let tagline: string;
    export let definition: string;
    export let example: string;
</script>

<div class="flex justify-center">
<div class="flex flex-col items-center justify-center gap-8 mx-8 p-8 border rounded-lg w-fit">

    <h1 class="text-2xl text-center">{name}</h1>

    <div class="flex flex-row items-center gap-4">
        <Terminal class="h-4 w-4" />
        <p class="text-center">{tagline.toLowerCase()}</p>
    </div>

    <p class="text-center">{definition.toLowerCase()}</p>

    <p class="text-center">{example.toLowerCase()}</p>

    <Button variant="outline" href="/">
        go back
        <Arrow class="ml-4 h-4 w-4" />
    </Button>

</div>
</div>
