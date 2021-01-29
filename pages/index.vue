<template>
  <div>
    <div class="jumbotron">
      <Nav class="navigation" />
      <div class="animated">
        <h1 class="mainTitle">Justin's Tree Service</h1>
        <div class="small-text">
          Tree Removal. Trimming & Pruning. Stump Grinding & Removal.
        </div>
        <button>Get A Quote</button>
        <button>Services</button>
      </div>
    </div>
    <div class="services-section">
      <h1>Services Offered</h1>
      <b-card-group deck>
        <b-card
          class="card-images"
          img-src="../assets/trees.jpg"
          header="Tree Removal"
          img-alt="Card image"
        >
          <b-card-text>
            Some quick example text to build on the card and make up the bulk of
            the card's content.
          </b-card-text>
        </b-card>
        <b-card
          class="card-images"
          img-src="../assets/trees.jpg"
          header="Trimming & Pruning"
          img-alt="Card image"
        >
          <b-card-text>
            Some quick example text to build on the card and make up the bulk of
            the card's content.
          </b-card-text>
        </b-card>
        <b-card
          class="card-images"
          img-src="../assets/trees.jpg"
          header="Stump Grinding & Removal"
          img-alt="Card image"
        >
          <b-card-text>
            Some quick example text to build on the card and make up the bulk of
            the card's content.
          </b-card-text>
        </b-card>
      </b-card-group>
    </div>
    <div class="team-section">
      <h1>Meet the team</h1>

      <b-card
        img-src="https://placekitten.com/300/300"
        img-alt="Card image"
        img-left
        class="mb-3"
      >
        <b-card-text>
          <h2>Justin-Professional Climber</h2>
          <p>about justin here</p>
        </b-card-text>
      </b-card>

      <b-card
        img-src="https://placekitten.com/300/300"
        img-alt="Card image"
        img-right
      >
        <b-card-text>
          <h2>Greg - Ground Crew, Equipment Manager</h2>
          <p>about greg here</p>
        </b-card-text>
      </b-card>
      <br />
      <b-card
        img-src="https://placekitten.com/300/300"
        img-alt="Card image"
        img-left
        class="mb-3"
      >
        <b-card-text>
          <h2>Brandon - Ground Crew, Office Manager</h2>
          <p>about brandon here</p>
        </b-card-text>
      </b-card>
    </div>
    <div class="gallery-section">
      <h1>Gallery</h1>
      <b-carousel
        id="carousel-fade"
        style="text-shadow: 0px 0px 2px #000"
        fade
        indicators
        img-width="1024"
        img-height="480"
      >
        <b-carousel-slide
          caption="First slide"
          img-src="https://picsum.photos/1024/480/?image=10"
        ></b-carousel-slide>
        <b-carousel-slide
          caption="Second Slide"
          img-src="https://picsum.photos/1024/480/?image=12"
        ></b-carousel-slide>
        <b-carousel-slide
          caption="Third Slide"
          img-src="https://picsum.photos/1024/480/?image=22"
        ></b-carousel-slide>
      </b-carousel>
    </div>
    <div class="quote-section">
      <h1>Request A Quote</h1>
      <input type="text" placeholder="Enter your name" />
      <input type="text" placeholder="Enter your email" />
      <br />
      <textarea
        name="description"
        id=""
        cols="80"
        rows="10"
        placeholder="Enter a description of your needs"
      ></textarea>
      <br />
      <button>Submit</button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Carter+One&display=swap");
.team-section {
  padding-top: 40px;
  padding-left: 20px;
  padding-right: 20px;
  padding-bottom: 80px;
  text-align: center;
  margin-bottom: 20px;
  background-color: #3a4549;
}
.team-section .card-body {
  background-color: #4c5b61;
}

.team-section h1 {
  margin-bottom: 30px;
  color: white;
}

body {
  font-family: "Carter One", cursive;
  background: #4c5b61;
}
button {
  margin-top: 50px;
  margin-right: 30px;
  /* border-radius: 25px; */
  font-size: 30px;
  width: auto;
  height: auto;
  background: transparent;

  border: groove;
  color: white;
}
button:hover {
  color: rgb(152, 159, 134);
}
.card-images img {
  height: 300px;
  width: auto;
}
#carousel-fade {
  z-index: -1;
}
.card-body {
  background-color: rgb(63, 64, 78);
  color: white;
}
.card-header {
  background-color: rgb(152, 159, 134);
  color: white;
}
.gallery-section {
  padding-top: 40px;
  padding-left: 20px;
  padding-right: 20px;
  padding-bottom: 20px;
  text-align: center;
  margin-top: 10px;
  color: white;
  margin-bottom: 20px;
}
.jumbotron {
  background-image: linear-gradient(
      to bottom,
      rgba(36, 50, 65, 0.7),
      rgba(36, 50, 65, 0.7)
    ),
    url("../assets/trees.jpg");
  height: 100vh;
  background-size: cover;
  text-align: center;
  color: white;
  text-decoration: none;
}
.navigation {
  padding-top: 0px;

  font-size: 20px;
  text-align: right;
}
.mainTitle {
  font-size: 120px;
  color: white;
}
.small-text {
  margin-top: 50px;
  font-size: 35px;
  color: rgb(169, 186, 157);
}
.services-section {
  padding-left: 20px;
  padding-right: 20px;
  padding-bottom: 70px;
  text-align: center;
  margin-bottom: 20px;
  color: white;
}
.quote-section {
  padding-top: 40px;
  padding-left: 20px;
  padding-right: 20px;
  padding-bottom: 70px;
  text-align: center;
  margin-top: 10px;
  margin-bottom: 20px;
  color: white;
  background-color: #3a4549;
}
.quote-section input,
textarea {
  font-size: 30px;
  margin-top: 20px;
  margin-right: 20px;
  background-color: transparent;
  border-top-style: hidden;
  border-right-style: hidden;
  border-left-style: hidden;
  border-bottom-style: groove;
}
/* textarea {
  font-size: 30px;
  margin-top: 20px;
  margin-right: 20px;
  background-color: transparent;
} */
.animated {
  top: 30%;
  position: relative;
  animation: 3s slide-right;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}
::placeholder {
  /* Chrome, Firefox, Opera, Safari 10.1+ */
  color: white;
  opacity: 1; /* Firefox */
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
@keyframes slide-right {
  from {
    margin-left: -100%;
    width: 100%;
  }

  to {
    margin-left: 0%;
    width: 100%;
  }
}
</style>
