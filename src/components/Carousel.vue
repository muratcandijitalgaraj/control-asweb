<template>
  <div>
    <!-- Slideshow container -->
    <div class="slideshow-container">
      <!-- Full-width images with number and caption text -->
      <div class="mySlides fade">
        <!-- <div class="numbertext">1 / 3</div> -->
        <img
          class="myImg firstImg"
          src="../assets/giris/imageGroup-1.svg"
          style="width: 100%"
        />
        <!-- <div class="text">Caption Text</div> -->
      </div>

      <div class="mySlides fade">
        <!-- <div class="numbertext">2 / 3</div> -->
        <img
          class="myImg"
          src="../assets/giris/imageGroup-2.svg"
          style="width: 100%"
        />
        <!-- <div class="text">Caption Two</div> -->
      </div>

      <div class="mySlides fade">
        <!-- <div class="numbertext">3 / 3</div> -->
        <img
          class="myImg"
          src="../assets/giris/imageGroup-3.svg"
          style="width: 100%"
        />
        <!-- <div class="text">Caption Three</div> -->
      </div>
    </div>
    <br />
  </div>
</template>

<script>
export default {
  data() {
    return {
      slideIndex: 0,
    };
  },
  methods: {
    showSlides() {
      var i;
      var slides = document.getElementsByClassName("mySlides");
      for (i = 0; i < slides.length; i++) {
        slides[i].style.display = "none";
      }
      this.slideIndex++;
      if (this.slideIndex > slides.length) {
        this.slideIndex = 1;
      }
      slides[this.slideIndex - 1].style.display = "block";
      console.log(this.slideIndex);
      // setTimeout(this.slideIndex + 1, 500); // Change image every 2 seconds
    },
  },
  created() {
    this.slideIndex = setInterval(() => this.showSlides(), 3000);
  },
};
</script>
<style>
* {
  box-sizing: border-box;
}
/* Slideshow container */
.slideshow-container {
  width: 500px;
  height: 500px;
  position: relative;
  margin: auto;
  border: 2px solid red;
}
.myImg {
  width: 500px;
  height: 500px;
}
/* Hide the images by default */
.mySlides {
  display: none;
}

/* Position the "next button" to the right */
.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}
/* On hover, add a black background color with a little bit see-through */
.prev:hover,
.next:hover {
  background-color: rgba(0, 0, 0, 0.8);
}

.active,
.dot:hover {
  background-color: #717171;
}
/* Fading animation */
.fade {
  -webkit-animation-name: fade;
  -webkit-animation-duration: 1.5s;
  animation-name: fade;
  animation-duration: 1.5s;
}
@-webkit-keyframes fade {
  from {
    opacity: 0.4;
  }
  to {
    opacity: 1;
  }
}
@keyframes fade {
  from {
    opacity: 0.4;
  }
  to {
    opacity: 1;
  }
}
</style>
