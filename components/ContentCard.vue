<template>
  <v-card class="pa-3 my-2">
    <div class="headline">
      <span class="ubunto">
        <slot name="title"></slot>
      </span>
    </div>
    <v-divider class="my-2"></v-divider>
    <div class="body-2 pa-3">
      <slot name="body"></slot>
    </div>
  </v-card>
</template>

<script>
export default {};
</script>
