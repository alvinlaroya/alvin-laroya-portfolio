<script>
  import "aos/dist/aos.css";
  // @ts-ignore
  import AOS from "aos";

  import { onMount } from "svelte";

  import "../app.css";

  import Navbar from "../lib/components/Navbar.svelte";

  onMount(() => {
    AOS.init();
  });
</script>

<svelte:head>
  <link href="https://fonts.cdnfonts.com/css/bogart" rel="stylesheet" />
  <!-- Google Tag Manager -->
  <script>
    (function (w, d, s, l, i) {
      w[l] = w[l] || [];
      w[l].push({ "gtm.start": new Date().getTime(), event: "gtm.js" });
      var f = d.getElementsByTagName(s)[0],
        j = d.createElement(s),
        dl = l != "dataLayer" ? "&l=" + l : "";
      j.async = true;
      j.src = "https://www.googletagmanager.com/gtm.js?id=" + i + dl;
      f.parentNode.insertBefore(j, f);
    })(window, document, "script", "dataLayer", "GTM-T4VJJ3MT");
  </script>
  <!-- End Google Tag Manager -->

  <script
    async
    src="https://www.googletagmanager.com/gtag/js?id=G-0ZWP28158E"
  ></script>
  <script>
    window.dataLayer = window.dataLayer || [];
    function gtag() {
      dataLayer.push(arguments);
    }
    gtag("js", new Date());

    gtag("config", "G-0ZWP28158E");
  </script>
</svelte:head>

<Navbar />
<div class="p-5">
  <!-- Google Tag Manager (noscript) -->
  <noscript
    ><iframe
      src="https://www.googletagmanager.com/ns.html?id=GTM-T4VJJ3MT"
      height="0"
      width="0"
      style="display:none;visibility:hidden"
    ></iframe></noscript
  >
  <!-- End Google Tag Manager (noscript) -->
  <slot />
</div>
