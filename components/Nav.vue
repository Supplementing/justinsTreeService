<template>
  <div>
    <div class="outer-container">
      <div class="navigation" :class="{ 'navbar-colored': scrolled }">
        <a class="navbar-brand" href="/">[logo here]</a>

        <span class="navbar-toggler-icon"></span>

        <ul class="asdf">
          <li class="nav-item">
            <a class="nav-link" href="#">
              Home
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">About</a>
          </li>
          <li>
            <a class="nav-link" href="#">Services</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      scrolled: false,
      lastScrollPosition: 0
    };
  },
  mounted() {
    window.addEventListener("scroll", this.onScroll);
  },
  methods: {
    onScroll() {
      const currentScrollPosition =
        window.pageYOffset || document.documentElement.scrollTop;

      if (currentScrollPosition < 0) {
        return;
      }
      this.scrolled = currentScrollPosition > 0;
    }
  }
};
</script>

<style>
.asdf {
  display: flex;
  list-style: none;
}
.navbar-brand {
  color: white;
  text-align: left;
}
.navbar-colored {
  background-color: #4c5b61;

  box-shadow: 0px 0px 0px 3px black;
  z-index: 1;
  width: auto;
  text-align: right;
  align-items: right;
}

.navigation {
  padding-bottom: 5px;
  position: fixed;
  width: 100%;
  display: flex;
  flex: right;
  height: 40px;
  top: 0;
  z-index: 1;

  /* background-color: transparent; */
}

.nav-link {
  color: white;
}
.nav-link:hover {
  color: rgb(152, 159, 134);
}
.navbar-brand {
  text-align: left;
}
.navbar-brand:hover {
  color: rgb(152, 159, 134);
}
</style>
