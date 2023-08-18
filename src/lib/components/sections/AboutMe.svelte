<script>
  import AboutMeImages from "./AboutMeImages.svelte";
  import HeaderTitle from "./HeaderTitle.svelte";
</script>

<div id="about-me-section">
  <HeaderTitle title="About Me" subtitle="My Introduction" />
  <div class="grid grid-cols-1 md:grid-cols-2 mt-7 md:px-32">
    <div class="order-2 md:order-1 flex md:px-24 justify-center mt-8 md:mt-0">
      <AboutMeImages />
    </div>
    <div
      class="order-1 md:order-2 grid md:h-[420px] content-center"
      data-aos="fade-up"
    >
      <p class="text-gray-600 text-sm font-thin md:pr-[29rem] text-justify">
        Web developer with extensive knowledge and years of experience working
        in web technologies and UI/UX design delivering quality work.
      </p>
      <div class="grid grid-cols-3 md:pr-[20rem] mt-8">
        <div class="text-center">
          <h1 class="text-xl md:text-2xl">3+</h1>
          <p class="font-thin text-gray-600 text-xs md:text-sm">
            Years experience
          </p>
        </div>
        <div class="text-center">
          <h1 class="text-xl md:text-2xl">15+</h1>
          <p class="font-thin text-gray-600 text-xs md:text-sm">
            Completed projects
          </p>
        </div>
        <div class="text-center">
          <h1 class="text-xl md:text-2xl">5+</h1>
          <p class="font-thin text-gray-600 text-xs md:text-sm">
            Companies worked
          </p>
        </div>
      </div>
      <a href="/files/alvinlaroyaresumeupdated.docx">
        <button
          type="button"
          data-aos="zoom-in"
          class="w-full md:w-48 mt-9 text-white bg-gradient-to-r from-purple-500 via-purple-600 to-purple-700 hover:bg-gradient-to-br focus:ring-4 focus:outline-none focus:ring-purple-300 dark:focus:ring-purple-800 font-normal rounded-lg text-lg px-5 py-4 text-center mr-2 mb-2"
          data-gtm-event="cta_dl_cv_click"
          data-gtm-category="cta"
          data-gtm-action="click"
          data-gtm-label="Download CV">Download CV</button
        >
      </a>
    </div>
  </div>
</div>
