<template>
  <thead>
    <tr>
      <th>{{ titlehead }}</th>
      <th>{{ subtitlehead }}</th>
      <th>{{ bodyhead }}</th>
      <th>{{ imghead }}</th>
    </tr>
  </thead>
</template>

<script>
export default {
  name: "my-tablehead",
  props: ["titlehead", "subtitlehead", "bodyhead", "imghead"]
};
</script>
