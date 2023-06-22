<template>
  <div  data-aos="zoom-in" data-aos-offset="500" data-aos-easing="ease-in-out" class="video-section max-w-7xl mx-auto mt-12 shadow-white">
    <div class="video-container" ref="videoContainer" :class="{ 'video-playing': isVideoPlaying }">
      <video class="video rounded-3xl" ref="video" @play="handleVideoPlay" @pause="handleVideoPause">
        <source :src="Video" type="video/mp4">
      </video>
    </div>
  </div>
</template>

<script setup>
import { ref, watch } from 'vue';
import Video from '../assets/videobyfiver.mp4';

const videoContainer = ref(null);
const video = ref(null);
const isVideoPlaying = ref(false);

const handleVideoPlay = () => {
  isVideoPlaying.value = true;
};

const handleVideoPause = () => {
  isVideoPlaying.value = false;
};

const options = {
  threshold: 0.5 // Adjust the threshold as needed
};

const intersectionCallback = (entries, observer) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      video.value.play();
    } else {
      video.value.pause();
    }
  });
};

const observer = new IntersectionObserver(intersectionCallback, options);

watch(videoContainer, () => {
  observer.observe(videoContainer.value);
});

</script>

<style>
/* Add your custom styles here */
</style>

<!--  -->
