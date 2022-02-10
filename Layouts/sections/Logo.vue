<template>
  <div class="logo">
    <NLink to="/">
      <v-img
        :src="require('@/assets/images/logos/apuka-logo.png')"
        alt="logo"
      />
    </NLink>
  </div>
</template>

<script>
export default {
  name: "Logo",

  data() {
    return {};
  },
};
</script>

<style lang="scss">
.logo{
  max-width: 100px;
}
.logo a {
  display: flex;
}
</style>