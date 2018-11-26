<template>
  <div class="card">
    <div class="card-image">
      <img v-bind:src="imgSrc" class="img-responsive" />
    </div>
    <div class="card-header">
      <div class="card-title h5">{{ title }}</div>
      <div class="card-subtitle text-gray">{{ subtitle }}</div>
    </div>
    <div class="card-body">{{ body }}</div>
    <div class="card-footer"></div>
  </div>
</template>

<script>
export default {
  name: "my-card",
  props: ["title", "subtitle", "body", "imgSrc"]
};
</script>
