<template>
  <div class="resume">
    <div class="container">
      <resumeInfo />
      <resumeServices />
      <resumeQuantity />
      <resumeReviews />

    </div>
  </div>
</template>

<script>
import resumeInfo from '@/components/page-section/resumeInfo';
import resumeServices from '@/components/page-section/resumeServices';
import resumeQuantity from '@/components/page-section/resumeQuantity';
import resumeReviews from '@/components/page-section/resumeReviews';

export default {
  components:{
    resumeInfo,
    resumeServices,
    resumeQuantity,
    resumeReviews
  }
}
</script>

<style scoped>
.resume {
  max-width: 479px;
  margin: 0 auto;
  background: #fff;
}
.container {
  padding: 0 10px;
}
</style>

