<template>
  <section>
   <div class="container">
      <Header />
    <Nuxt />
    <Footer />
   </div>
  </section>
</template>
<style scoped>
section {

  background: rgb(42, 83, 42);
  background: radial-gradient(
    circle,
    rgb(53, 105, 53) 0%,
    rgba(77, 147, 76, 1) 100%
  );

}
.container{
display: block;
overflow: hidden;
  margin: 0 auto;
}
</style>
