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
      linksDc: [
        {
          text: "Characters",
          url: "#",
        },
        {
          text: "Comics",
          url: "#",
        },
        {
          text: "Movies",
          url: "#",
        },
        {
          text: "TV",
          url: "#",
        },
        {
          text: "Games",
          url: "#",
        },
        {
          text: "Videos",
          url: "#",
        },
        {
          text: "News",
          url: "#",
        },
      ],
      shopsDc: [
        {
          text: "Shop DC",
          url: "#",
        },
        {
          text: "Shop DC collectibles",
          url: "#",
        },
      ],
      dc: [
        {
          text: "Terms Of Use",
          url: "#",
        },
        {
          text: "Privacy policy (New)",
          url: "#",
        },
        {
          text: "Ad Choices",
          url: "#",
        },
        {
          text: "Advertising",
          url: "#",
        },
        {
          text: "Jobs",
          url: "#",
        },
        {
          text: "Subscriptions",
          url: "#",
        },
        {
          text: "Talent Workshops",
          url: "#",
        },
        {
          text: "CPSC Certificates",
          url: "#",
        },
        {
          text: "Ratings",
          url: "#",
        },
        {
          text: "Shop Help",
          url: "#",
        },
        {
          text: "Contact Us",
          url: "#",
        },
      ],
      sites: [
        {
          text: "DC",
          url: "#",
        },
        {
          text: "MAD Magazine",
          url: "#",
        },
        {
          text: "DC Kids",
          url: "#",
        },
        {
          text: "DC Universe",
          url: "#",
        },
        {
          text: "DC Power Visa",
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
  <div class="container_center_footer">
    <div class="container_center">
      <div class="container_left">
        <div>
          <h3>DC COMICS</h3>
          <ul>
            <li v-for="linkDc in linksDc">
              <a :href="linkDc.url">{{ linkDc.text }} </a>
            </li>
          </ul>
          <h3>SHOP</h3>
          <ul>
            <li v-for="shop in shopsDc">
              <a :href="shop.url">{{ shop.text }} </a>
            </li>
          </ul>
        </div>
        <div>
          <h3>DC</h3>
          <ul>
            <li v-for="Element in dc">
              <a :href="Element.url">{{ Element.text }} </a>
            </li>
          </ul>
        </div>
        <div>
          <h3>Sites</h3>
          <ul>
            <li v-for="site in sites">
              <a :href="site.url">{{ site.text }} </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.container_top_footer {
  padding: 50px 0;
  background-color: #0c7cec;
}

.container_top {
  height: 100%;
  margin: 0 15%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.container_top ul {
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

.container_top a {
  display: flex;
  align-items: center;
  text-decoration: none;
  color: white;
}

.container_center_footer {
  background-image: url("/footer-bg.jpg");
}

.container_center {
  padding-bottom: 40px;
  margin: 0 15%;
  display: flex;
}

h3 {
  color: white;
  padding-top: 40px;
  margin-bottom: 10px;
}
.container_center li {
  margin-bottom: 8px;
  font-size: 0.8rem;
  list-style: none;
}
.container_center a {
  text-decoration: none;
  color: gray;
}

.container_left {
  display: flex;
  gap: 4rem;
}
</style>
