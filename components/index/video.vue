<style scoped>
  

  .background{
    background-image: 'https://ibb.co/qyHfNFD';
  }


</style>

<template>
  <div class="view">

    <!--Video source-->
    <video class="video-intro" id="header-video" autoplay="autoplay" loop="loop">
      <source src="https://media.istockphoto.com/id/618488436/video/milky-way-over-the-kolsay-lake-in-kazakhstan-mountains.mp4?s=mp4-640x640-is&k=20&c=vpXa7izd3uzRoqfAekRyHiU-cYAtmS_l6XTCv54gQHE=" type="video/mp4" />
    </video>

    <!-- Mask & flexbox options-->
    <div class="mask rgba-black-light d-flex justify-content-center align-items-center">

      <!-- Content -->
      <div class="text-center white-text mx-5 wow fadeIn">
        <h1 class="mb-4">
          <strong>Hi Im Winston!</strong>
        </h1>
        <p>Nice to meet you</p>

        <p>
          <strong>Every great developer you know got there by solving problems 
they were unqualified to solve until they actually did it. </strong>
        </p>

        <p class="mb-4 d-none d-md-block">
          <strong>by Patrick McKenzie.</strong>
        </p>

        <!-- <a target="_blank" href="https://mdbootstrap.com/bootstrap-tutorial/" class="btn btn-outline-white btn-lg">Start free tutorial
          <i class="fa fa-graduation-cap ml-2"></i>
        </a> -->
      </div>
      <!-- Content -->

    </div>
    <!-- Mask & flexbox options-->
  </div>
</template>
<script>
export default {
  data(){
      return{
        playBg: false
      }
  },
  mounted(){
      
  },
  methods: {
      userInteract(){
          if(!this.playBg){
              this.playBg = true;
              document.getElementById('header-video').play();
              return true
          }

          return false
      }
  }
}
</script>
