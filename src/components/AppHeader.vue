<script>
export default {
  data() {
    return {
      links: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Video",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<template>
  <div class="container_header">
    <img class="logo" src="/dc-logo.png" alt="logo" />
    <ul>
      <li v-for="link in links">
        <a :href="link.url" :class="link.current ? 'active' : ''">
          {{ link.text }}
        </a>
      </li>
    </ul>
  </div>
</template>

<style lang="scss" scoped>
.container_header {
  margin: 20px 0;
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
}

.logo {
  width: 70px;
  cursor: pointer;
}

ul {
  display: flex;
  align-items: center;
  list-style: none;
  gap: 1.2rem;
  font-size: 0.95rem;
  font-weight: 700;
  line-height: 70px;
}

a {
  text-decoration: none;
  color: black;
}

.active {
  color: #0c7cec;
  border-bottom: 2px solid #0c7cec;
}
</style>
