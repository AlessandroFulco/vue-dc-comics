<template>
    <div>
        <h2> &rArr;contenuto principale &lArr; </h2>
    </div>
</template>

<script>
export default {
  name: 'MainContent',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
div {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 150px;
    background-color: #000;

    h2 {
    color: #fff;
}
}

</style>
