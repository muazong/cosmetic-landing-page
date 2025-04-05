<script setup lang="ts">
import ProductAwards from './components/ProductAwards.vue'
import ProductBanner from './components/ProductBanner.vue'
import ProductDetails from './components/ProductDetails.vue'
import ProductFeature from './components/ProductFeature.vue'
import ProductIngredients from './components/ProductIngredients.vue'
import ProductRatings from './components/ProductRatings.vue'
import ProductUsageGuide from './components/ProductUsageGuide.vue'
import SkinCareFeatures from './components/SkinCareFeatures.vue'
import SkinCareResults from './components/SkinCareResults.vue'
</script>

<template>
  <section id="detail" class="detail-container component-container">
    <SkinCareFeatures />
    <ProductFeature />
    <ProductDetails />
    <ProductIngredients />
    <ProductBanner />
    <ProductUsageGuide />
    <SkinCareResults />
    <ProductAwards />
    <ProductRatings />
  </section>
</template>

<style scoped>
.detail-component {
  padding-top: var(--nav-height);
  padding: var(--nav-height) 0 30px 0;
  min-height: 500px;
  height: auto;
  margin-bottom: var(--nav-height);
}
</style>
