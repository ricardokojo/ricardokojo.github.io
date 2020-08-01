<template>
  <main>
    <TheHeader />
  </main>
</template>

<script>
import TheHeader from '@/components/TheHeader.vue'

export default {
  components: {
    TheHeader,
  },
  head() {
    return {
      title: "Kojo's - personal page, portolio, glorified CV",
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        {
          hid: 'description',
          name: 'description',
          content:
            "Ricardo H. H. Kojo's personal page. Built as a portfolio, glorified CV and WebDev sandbox. UNDER CONSTRUCTION.",
        },
      ],
    }
  },
}
</script>

<style></style>
