<template>
  <div>
    <div class="outer-container">
      <nav
        class="navbar navbar-expand-lg"
        :class="{ 'navbar-colored': scrolled }"
      >
        <a class="navbar-brand" href="/">[logo here]</a>
        <button
          class="navbar-toggler"
          type="button"
          data-toggle="collapse"
          data-target="#navbarText"
          aria-controls="navbarText"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarText">
          <ul class="navbar-nav ml-auto">
            <li class="nav-item active">
              <a class="nav-link" href="#">
                Home
                <span class="sr-only">(current)</span>
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
      </nav>
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
.navbar-brand {
  color: white;
  text-align: left;
}
.navbar-colored {
  background-color: #4c5b61;
  box-shadow: 0px 0px 0px 3px black;
  z-index: 1;
}

.navbar {
  position: fixed;
  right: 0;
  width: 100%;
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
.navbar-brand:hover {
  color: rgb(152, 159, 134);
}
</style>
