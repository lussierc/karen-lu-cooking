<template>
  <div id="categories-page" class="page-wrapper categories-page">
    <site-hero title="Recipe Categories" image="/uploads/home-hero.jpg" />
    <main-section theme="one-column">
      <categories-grid />
    </main-section>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: `Recipe Categories | ${this.$siteConfig.siteName}`
    }
  }
}
</script>
