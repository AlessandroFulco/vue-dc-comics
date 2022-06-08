<template>
    <div>
      <ul>
        <li v-for="(item, index) in otherItems" :key="index">
          <a :href="item.link">
            <img :src="item.path" :alt="item.text">
            {{item.text}}
          </a>
        </li>
      </ul>
    </div>
</template>

<script>
export default {
  name: 'OtherContent',
  data(){
    return {
      otherItems: [
        {
          link: "#",
          path: require("../assets/img/buy-comics-digital-comics.png"),
          text: "digital comics"
        },
        {
          link: "#",
          path: require("../assets/img/buy-comics-merchandise.png"),
          text: "dc merchandise"
        },
        {
          link: "#",
          path: require("../assets/img/buy-comics-shop-locator.png"),
          text: "subscription"
        },
        {
          link: "#",
          path: require("../assets/img/buy-comics-subscriptions.png"),
          text: "comic shop locator"
        },
        {
          link: "#",
          path: require("../assets/img/buy-dc-power-visa.svg"),
          text: "dc power visa"
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
div {
  padding: 20px;
background-color: #0282f9;
  ul {
    list-style-type: none;
    li {
      display: inline-block;
      a {
        display: inline-block;
        text-decoration: none;
        color: #fff;
        padding: 10px 15px;
        text-transform: uppercase;
        font-size: 12px;
        img {
          height: 50px;
          vertical-align: middle;
        }
      }
    }

  }

}

</style>
