<template>
    <header>
        <h1>{{ mode }} Mode</h1>
        <Toggle :mode="mode" @toggle="$emit('toggle')" />
        <nav>
            <div class="nav-links">Home</div>
            <div class="nav-links">About</div>
            <div class="nav-links">Portfolio</div>
            <div class="nav-links">Contact</div>
        </nav>
    </header>

</template>

<script>
import Toggle from "@/components/Toggle";

export default {
    props: [ "mode" ],
    components: {
        Toggle
    }
}
</script>

<style>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 25px;
    height: 60px;
    background: #d3d3d3;
    transition: background 0.3s ease-in-out;
}
.dark header {
    background: #15202b;
}
header h1 {
    font-size: 32px;
    text-transform: uppercase;
    font-weight: 900;
}
header nav {
    display: flex;
    height: 60px;
}
header nav .nav-links {
    display: flex;
    align-items: center;
    padding: 0 15px;
}
header nav .nav-links:hover {
    background: #b0b0b0;
}
.dark header nav .nav-links:hover {
    background: #101520;
}

</style>