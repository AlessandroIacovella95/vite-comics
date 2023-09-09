<script>
export default {
  data() {
    return {
      cards: [
        {
          text: "DIGITAL COMICS",
          image: "buy-comics-digital-comics.png",
          url: "#",
        },
        {
          text: "DC MERCHANDISE",
          image: "buy-comics-merchandise.png",
          url: "#",
        },
        {
          text: "SUBSCRIPTION",
          image: "buy-comics-subscriptions.png",
          url: "#",
        },
        {
          text: "COMIC SHOP LOCATOR",
          image: "buy-comics-shop-locator.png",
          url: "#",
        },
        {
          text: "DC POWER VISA",
          image: "buy-dc-power-visa.svg",
          url: "#",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="container_top_footer">
    <div class="container_top">
      <ul>
        <li v-for="card in cards">
          <a :href="card.url">
            <img :src="card.image" alt="" />
            <span>{{ card.text }}</span>
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.container_top_footer {
  height: 200px;
  background-color: #0c7cec;
}

.container_top {
  height: 100%;
  margin: 0 15%;
  display: flex;
  justify-content: center;
  align-items: center;
}

ul {
  display: flex;
  align-items: center;
  gap: 3rem;
  list-style-type: none;
}

span {
  font-size: 0.8rem;
  margin-left: 10px;
  white-space: nowrap;
}

li img {
  width: 45px;
}

li:last-child img {
  width: 65px;
}

a {
  display: flex;
  align-items: center;
  text-decoration: none;
  color: white;
}
</style>
