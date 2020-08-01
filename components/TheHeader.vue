<template>
  <header>
    <div class="title">
      <h1>Ricardo H. H. Kojo</h1>
      <p>To be updated soon...</p>
      <Brush class="background" />
    </div>
    <div class="social">
      <a href="https://codepen.io/ricardokojo/">
        <img src="https://simpleicons.org/icons/codepen.svg" />
      </a>
      <a href="https://github.com/ricardokojo">
        <img src="https://simpleicons.org/icons/github.svg" />
      </a>
      <a href="https://gitlab.com/ricardokojo">
        <img src="https://simpleicons.org/icons/gitlab.svg" />
      </a>
      <a href="https://www.linkedin.com/in/ricardokojo/">
        <img src="https://simpleicons.org/icons/linkedin.svg" />
      </a>
    </div>
  </header>
</template>

<script>
import Brush from '@/components/Brush.vue'

export default {
  components: {
    Brush,
  },
}
</script>

<style>
header {
  @apply flex flex-col items-center justify-center h-screen w-screen overflow-hidden;
}

h1 {
  @apply text-gray-900 text-4xl uppercase font-black;
}

p {
  @apply text-gray-900 text-2xl;
}

.title {
  @apply flex flex-col text-center relative;
}

.social {
  @apply flex flex-row mt-12;

  a {
    @apply bg-gray-100 mr-4 rounded-sm transition-colors duration-200;

    &:last-child {
      @apply mr-0;
    }

    &:hover {
      background-color: #ef3f56;
    }

    img {
      @apply w-10 p-1;
    }
  }
}

.background {
  @apply absolute;
  width: 350%;
  height: 350%;
  top: 60%;
  left: 50%;
  transform: translate(-50%, -50%) rotateZ(15deg);
  z-index: -1;
}

@screen sm {
  h1 {
    @apply text-5xl;
  }

  .social {
    a {
      @apply mr-2;

      img {
        @apply w-8;
      }
    }
  }
}
</style>
