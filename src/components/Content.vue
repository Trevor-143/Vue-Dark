<template>
    <div class="content">
        <h3>This is {{ mode }} mode</h3>
        <div class="image-grid">
            <div class="col">
                <img src="https://cdn.pixabay.com/photo/2016/02/28/12/55/boy-1226964__340.jpg" alt="">
            </div>
            <div class="col">
                <img src="https://cdn.pixabay.com/photo/2012/12/27/19/40/chain-link-72864__340.jpg" alt="">
            </div>
            <div class="col">
                <img src="https://cdn.pixabay.com/photo/2017/09/25/11/55/cyberspace-2784907__340.jpg" alt="">
            </div>
        </div>
        <p class="para">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore quae cum natus quia odio, accusantium adipisci, suscipit quibusdam cupiditate nostrum, neque voluptatum ea id. Laudantium consectetur repudiandae velit officiis. Amet esse iure omnis nesciunt corporis. Exercitationem voluptate enim numquam quaerat ducimus at dignissimos quasi, quo sunt nemo nisi similique est?
        </p>
    </div>

</template>

<script>
export default {
    props: ['mode']
}
</script>

<style>
.content {
    padding: 25px;
}
.content h3 {
    font-size: 28px;
    text-transform: uppercase;
    font-weight: 300;
    margin-bottom: 25px;
}
.image-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-gap: 15px;
}
.image-grid .col img {
    width: 100%;
}
.para {
    width: 100%;
    max-width: 600px;
    margin: 25px auto 0px;
}
</style>