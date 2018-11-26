<template>
  <tr class="active">
    <td>{{ title }}</td>
    <td>{{ subtitle }}</td>
    <td>{{ body }}</td>
    <td><img v-bind:src="imgSrc" /></td>
  </tr>
</template>

<script>
export default {
  name: "my-row",
  props: ["title", "subtitle", "body", "imgSrc"]
};
</script>
