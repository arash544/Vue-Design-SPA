<template>
  <main>
    <section class="banner-wrapper">
      <Banner />
      <Top />
    </section>
    <section class="toptext-wrapper">
      <OfficeDetails />
      <LawDetails />
    </section>
  </main>
</template>

<script>
import Banner from "@/components/menu-baner/Banner";
import Top from "@/components/cities-info/Top";
import LawDetails from "@/components/law-info/LawDetails";
import OfficeDetails from "@/components/office-part/OfficeDetails";
export default {
  components: {
    Banner,
    LawDetails,
    OfficeDetails,
    Top
  }
};
</script>

<style lang="scss" scoped>
section {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-evenly;
}

main {
  padding-top: 50px;
  padding-left: 15px;
  overflow-y: hidden;
  @media screen and (max-width: 768px) {
    padding-left: 0;
  }
}
.toptext-wrapper {
  margin-top: 50px;
  width: 100%;
}
</style>
