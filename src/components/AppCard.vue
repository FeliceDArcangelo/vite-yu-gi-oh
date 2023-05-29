<script>

export default {
    props: {
        CharacterData: Object,
    }

}
</script>


<template>
  <div class="card">
    <img :src="CharacterData.card_images[0].image_url" :alt="CharacterData.name">
    <h3>{{ CharacterData.name }}</h3>
    <div class="specie">{{ CharacterData.race }} </div>
  </div>
</template>



<style lang="scss" scoped>
@use '../assets/style/partials/variables' as *;
.card{
    width: 200px;
    height: 400px;
    text-align: center;
    background-color: $brand-color;
    border-bottom-left-radius: 18px;
    border-bottom-right-radius: 18px;

    img{
        width: 100%;
    }

    h3{
        margin-top: .8em;
        color: white;
    }

    .specie{
        margin-top: .8em;
    }


}

</style>