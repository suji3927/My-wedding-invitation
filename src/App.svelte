<script>
  import Welcome from "@/components/Welcome.svelte";
  import Invitation from "@/components/Invitation.svelte";
  import Calendar from "@/components/Calendar.svelte";
  import Gallery from "@/components/Gallery.svelte";
  import Place from "@/components/Place.svelte";
  import Contect from "@/components/Contect.svelte";
  import Notifications from "svelte-notifications";
  import Footer from "@/components/Footer.svelte";

  let flowerSrc = "images/flower.png";
</script>

<style>
  @import url("https://fonts.googleapis.com/css2?family=Gowun+Dodum&display=swap");

  .body-margin {
    margin: 0 auto;
  }

  * {
    font-family: "Gowun Dodum";
  }

  /* @font-face {
    font-family: "SunBatang-Light";
    src: url(../fonts/SunBatang-Light.ttf);
  } */
</style>

<Notifications>
  <main class="w-10/12 body-margin">
    <Welcome />
    <Invitation flowerSrc="{flowerSrc}" />
    <Calendar flowerSrc="{flowerSrc}" />
    <Gallery flowerSrc="{flowerSrc}" />
    <Place flowerSrc="{flowerSrc}" />
    <Contect flowerSrc="{flowerSrc}" />
    <Footer />
  </main>
</Notifications>
