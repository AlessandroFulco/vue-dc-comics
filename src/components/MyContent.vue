<template>
    <div class="card-prod">
        <img :src="details.thumb" :alt="details.series">
        <h4>{{details.series}}</h4>   
    </div>
</template>

<script>
export default {
    name: 'MyContent',
    props: {
        details: Object
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
    div.card-prod {
        flex-basis: calc(100% / 6);
        img {
            height: 150px;
            width: 150px;
            object-fit: cover;
            object-position: top;
        }
        h4 {
            width: 150px;
            color: #fff;
            font-size: 14px;
        }

    }

</style>
