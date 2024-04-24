<script lang="ts">
    import "../app.css";

    import Header from "./Header.svelte";
    import Sidebar from "./Sidebar.svelte";
</script>

<div class="flex flex-col items-center gap-16">

    <Header />

    <div class="flex flex-row justify-center gap-32 w-full">
        <div class="basis-1/6">
            <Sidebar />
        </div>
        <slot />
        <div class="basis-1/6"></div>
    </div>

</div>
