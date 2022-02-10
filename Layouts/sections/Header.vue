<template>
  <div>
<Header1/>
  </div>
</template>

<script>
export default {
  name: "Header",

  components: {
    Header1: () => import("@/components/custom/header/Header1"),
    Logo: () => import("@/layouts/sections/Logo")
  },
  data() {
    return {
      isActive: false
    };
  },
  methods: {
    toggleClass: function(event) {
      this.isActive = !this.isActive;
    }
  }
};
</script>
