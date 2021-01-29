<template>
  <div>
    <Nav class="navigation" />
    <div class="jumbotron">
      <div class="animated">
        <h1 class="mainTitle">Justin's Tree Service</h1>
        <div class="small-text">
          Tree Removal. Trimming & Pruning. Stump Grinding & Removal.
        </div>
        <button>
          <a class="jumpButton" href="#quote">Get A Quote</a>
        </button>
        <button class="jumpButton">
          <a href="#services" class="jumpButton">Services</a>
        </button>
      </div>
    </div>
    <div id="services" class="services-section">
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
    <div id="about" class="team-section">
      <h1>Meet the team</h1>
      <h6>
        Several years ago, after working for one of the largest tree companies
        in Charlotte, Justin decided to step away and pursue his life-long goal
        of owning his own business. Starting with just a pickup truck and a
        small utility trailer, Justin’s Tree Service has grown into an extremely
        reputable, professional tree company with all the proper tools and
        equipment needed to get the job done. Justin’s brother, Brandon, and his
        father, Greg, are also part of the team along with several other crew
        members. Justin's Tree Service is dedicated to providing you with
        top-of-the line tree services while focusing on the safety, health, and
        beauty of your trees.
      </h6>
      <div class="images-container">
        <div class="round">
          <div class="showDetails">Justin-Owner/Expert Climber</div>
        </div>
        <div class="round">
          <div class="showDetails">Brandon-Ground Crew/Office Manager</div>
        </div>
        <div class="round">
          <div class="showDetails">Greg-Ground Crew/Equipment Manager</div>
        </div>
      </div>
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
    <div id="quote" class="quote-section">
      <h1>Request A Quote</h1>
      <input type="text" placeholder="Enter your name" />
      <input type="text" placeholder="Enter your email" />
      <br />
      <textarea
        name="description"
        id=""
        cols="20"
        rows="5"
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
  width: 100%;
  padding-top: 40px;
  padding-left: 20px;
  padding-right: 20px;
  padding-bottom: 80px;
  text-align: center;
  margin-bottom: 20px;
  background-color: #3a4549;
  color: white;
}
.team-section .card-body {
  background-color: #4c5b61;
}

body {
  font-family: "Carter One", cursive;
  background: #4c5b61;
}
b-card {
  width: 100%;
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
.jumpButton {
  text-decoration: none;
  color: white;
}
.jumpButton:hover {
  text-decoration: none;
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
.images-container {
  width: auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
.jumbotron {
  background-image: linear-gradient(
      to bottom,
      rgba(36, 50, 65, 0.7),
      rgba(36, 50, 65, 0.7)
    ),
    url("../assets/trees.jpg");
  height: 100vh;
  width: 100%;
  background-size: cover;
  text-align: center;
  color: white;
  text-decoration: none;
}
@media screen and (max-width: 800px) {
  .jumbotron {
    height: auto;
  }
}
.round {
  background-image: url("../assets/trees.jpg");
  background-size: cover;
  margin: 10px 10px 10px 10px;
  border-radius: 50%;
  width: 240px;
  height: 240px;
}
.showDetails {
  opacity: 0;
  padding-top: 20%;
  font-size: 17px;
}
.round:hover .showDetails {
  opacity: 1;
  background-color: rgba(152, 159, 134, 0.7);
  width: 240px;
  height: 240px;
  border-radius: 50%;
  color: white;
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
.team-section h1 {
  margin-bottom: 30px;
  color: white;
  width: 100%;
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
  /* animation: 3s slide-right; */
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
