<template>
  <div>
    <!-- -----------------------------------------------
    Banner
    ----------------------------------------------- -->
    <Banner />
    <!-- -----------------------------------------------
    ./ Banner
    ----------------------------------------------- -->
    <!-- -----------------------------------------------
    All Components
    ----------------------------------------------- -->
   <BannerText />
    <Banner1 />
    <Feature1 />
    <Team />
    <Contact />
    <!-- -----------------------------------------------
    ./ All Components
    ----------------------------------------------- -->
    <!-- -----------------------------------------------
    Coming Soon
    ----------------------------------------------- -->
    <ComingSoon />
    <!-- -----------------------------------------------
    ./ Coming Soon
    ----------------------------------------------- -->
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: "Apukasoft",
      meta: [
        {
          hid: "description",
          name: "Apukasoft",
          content: "Empresa de tecnologia",
        },
      ],
    };
  },

  data() {
    return {};
  },
  components: {
    // ------------------------- //
    Banner: () => import("@/components/shared/lp-banner/Banner"),
    ComingSoon: () => import("@/components/shared/coming-soon/ComingSoon"),
      BannerText: () => import("@/components/custom/banner/BannerText"),
    Banner1: () => import("@/components/custom/banner/Banner1"),
    Feature1: () => import("@/components/custom/features/Feature1"),
    Team: () => import("@/components/custom/team/Team"),
    Contact: () => import("@/components/custom/contact/Contact"),
  },
};
</script>
