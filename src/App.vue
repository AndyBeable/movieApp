<template>
  <header>
    <router-link to="/">
  <Navigation />
    </router-link>
  </header>
  <main>
  <router-view/>
  </main>
</template>

<script>
import Navigation from "@/components/ui/Navigation";
export default {
  components: {
    Navigation
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Fira Sans', sans-serif;

  &::selection {
    background: transparentize(#42b883, 0.5);
  }
}
body {
  background-color: #141414;
}

a {
  text-decoration: none;
}

header {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 10px 16px;
  background-color: #141414;
  box-shadow: 0px 0px 6px rgba(0,0,0, 0.1);

  h1 {
    color: #e5e5e5;
    font-size: 28px;

    span {
      color: #681818;
    }
  }
}
</style>
