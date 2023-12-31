<script>
export default {
  name: "AppHeader",
  data() {
    return {
      links: [
        {
          text: "CHARACTERS",
          url: "#",
          current: false
        },
        {
          text: "COMICS",
          url: "#",
          current: true
        },
        {
          text: "MOVIES",
          url: "#",
          current: false
        },
        {
          text: "TV",
          url: "#",
          current: false
        },
        {
          text: "GAMES",
          url: "#",
          current: false
        },
        {
          text: "COLLECTIBLES",
          url: "#",
          current: false
        },
        {
          text: "VIDEOS",
          url: "#",
          current: false
        },
        {
          text: "FANS",
          url: "#",
          current: false
        },
        {
          text: "NEWS",
          url: "#",
          current: false
        },
        {
          text: "SHOP",
          url: "#",
          current: false
        }
      ]
    }
  }
}
</script>

<template>
    <header>
      <div class="container">
        <div class="logo">
          <img src="../../public/img/dc-logo.png" alt="logo dc">
        </div>
        <nav>
          <ul>
            <li v-for="(link, i) in links" :key="i" :class="link.current ? 'active' : ''">  
            <a :class="link.current ? 'active' : ''" href="#"> {{ link.text }} </a>
            </li>
          </ul>
        </nav>
      </div>
      
    </header>
  
</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;
@use '../styles/general.scss' as *;

header {
  width: 100%;
  height: 100px;
  .container {
    @include flex-between;
    height: 100%;
  }

  .logo {
    width: 70px;

    img {
      width: 100%
    }
  }

  nav {
    height: 100%;

    ul {
    @include flex-between;
    height: 100%;

    li {
      padding: 10px;
      font-size: 13px;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100%;

      &.active {
        border-bottom: 3px solid $primary;
        }

      a {
        color: #787878;

        &.active {
        color: $primary;
        }

        
      }
    }
  }
  }

}




</style>
