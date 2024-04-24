<svelte:head>
	<title>ascii brain</title>
	<meta name="description" content="ascii brain - a fun interactive brain parts diagram for ap psych" />
</svelte:head>

<script lang="ts">
    import { Button } from "$lib/components/ui/button";
    import * as Tabs from "$lib/components/ui/tabs";
</script>

<Tabs.Root value="lobes" class="flex flex-col items-center justify-center">
    <Tabs.List>
        <Tabs.Trigger value="lobes">lobes</Tabs.Trigger>
        <Tabs.Trigger value="parts">parts</Tabs.Trigger>
    </Tabs.List>
    <Tabs.Content value="lobes">
        <div class="relative">
            <img width="1176" height="1176" src="/images/lobes.png" alt="brain" />
            <Button href="/frontal-lobe" variant="ghost" class="absolute left-[25%] top-[25%] bg-zinc-950 bg-opacity-70 hover:bg-opacity-80 size-16 rounded-full"></Button>
            <Button href="/parietal-lobe" variant="ghost" class="absolute left-[65%] top-[25%] bg-zinc-950 bg-opacity-70 hover:bg-opacity-80 size-16 rounded-full"></Button>
            <Button href="/temporal-lobe" variant="ghost" class="absolute left-[40%] top-[55%] bg-zinc-950 bg-opacity-70 hover:bg-opacity-80 size-16 rounded-full"></Button>
            <Button href="/occipital-lobe" variant="ghost" class="absolute left-[85%] top-[45%] bg-zinc-950 bg-opacity-70 hover:bg-opacity-80 size-16 rounded-full"></Button>
        </div>
    </Tabs.Content>
    <Tabs.Content value="parts">
        parts here
    </Tabs.Content>
</Tabs.Root>
