<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="About Karen's Home Cooking"
      subtitle="Learn more about Karen!"
      image="/uploads/home-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>Welcome to my Cookbook!</h3>
          <p>
            <strong>
              This online cookbook contains family favorite recipes!
            </strong>
          </p>
          <p>
            Over the years I have saved up a lot of recipes and needed a place
            to store them, hence the creation of this online cookbook!
          </p>
        </div>
      </template>

      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Latest Posts
        </h3>
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  }
}
</script>
