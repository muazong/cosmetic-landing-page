<script setup lang="ts">
import ProductBanner from './components/ProductBanner.vue'
import ProductDetails from './components/ProductDetails.vue'
import ProductFeature from './components/ProductFeature.vue'
import ProductIngredients from './components/ProductIngredients.vue'
import ProductUsageGuide from './components/ProductUsageGuide.vue'
import SkinCareFeatures from './components/SkinCareFeatures.vue'
</script>

<template>
  <section id="detail">
    <SkinCareFeatures />
    <ProductFeature />
    <ProductDetails />
    <ProductIngredients />
    <ProductBanner />
    <ProductUsageGuide />
  </section>
</template>

<style scoped>
#detail {
  width: 100%;
}
</style>
