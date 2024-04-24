<script lang="ts">
    import { Button } from "$lib/components/ui/button";
    import Arrow from "lucide-svelte/icons/corner-down-left"

    export let name: string;
    export let definition: string;
    export let example: string;
</script>

<div class="flex flex-col items-center justify-center gap-16 px-4">

    <h1 class="text-2xl text-center">{name}</h1>

    <p class="text-center">{definition}</p>

    <Button variant="outline" href="/">
        go back
        <Arrow class="ml-4 h-4 w-4" />
    </Button>

</div>
