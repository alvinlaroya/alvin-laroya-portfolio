<script>
  import { AccordionItem, Accordion, Progressbar } from "flowbite-svelte";
  import HeaderTitle from "./HeaderTitle.svelte";
  const frontendStack = [
    {
      title: "Vue",
      percent: 99,
    },
    {
      title: "Vuex, Pinia",
      percent: 99,
    },
    {
      title: "Vuetify",
      percent: 99,
    },
    {
      title: "Nuxt",
      percent: 99,
    },
    {
      title: "React",
      percent: 85,
    },
    {
      title: "React Native",
      percent: 85,
    },
    {
      title: "Redux, Zustand",
      percent: 85,
    },
    {
      title: "Svelte",
      percent: 90,
    },
    {
      title: "Svelte kit",
      percent: 90,
    },
    {
      title: "Tailwind CSS",
      percent: 99,
    },
    {
      title: "Flowbite",
      percent: 99,
    },
  ];

  const backendstack = [
    {
      title: "Node JS",
      percent: 99,
    },
    {
      title: "Express",
      percent: 99,
    },
    {
      title: "MySQL",
      percent: 85,
    },
    {
      title: "MongoDB",
      percent: 89,
    },
    {
      title: "Firebase",
      percent: 85,
    },
    {
      title: "Pocketbase",
      percent: 90,
    },
    {
      title: "Rest API",
      percent: 99,
    },
    {
      title: "GraphQL",
      percent: 85,
    },
    {
      title: "Storefront",
      percent: 85,
    },
  ];
</script>

<div id="skills-section">
  <HeaderTitle title="Skills" subtitle="My Tech Stack" />
  <div
    class="grid grid-cols-1 md:grid-cols-2 content-center gap-9 mt-7 md:px-80"
  >
    <div class="order-2 md:order-1 text-sm" data-aos="fade-right">
      <Accordion flush>
        <AccordionItem open>
          <span slot="header" class="text-sm font-normal"
            >Frontend Developer</span
          >
          {#each frontendStack as stack}
            <div class="my-3">
              <div class="mb-1 text-xs md:text-sm font-light dark:text-white">
                {stack.title}
              </div>
              <Progressbar
                color="purple"
                progress={stack.percent}
                size="h-1.5"
              />
            </div>
          {/each}
        </AccordionItem>
        <AccordionItem>
          <span slot="header">Backend Developer</span>
          {#each backendstack as stack}
            <div class="my-3">
              <div class="mb-1 text-xs md:text-sm font-light dark:text-white">
                {stack.title}
              </div>
              <Progressbar
                color="purple"
                progress={stack.percent}
                size="h-1.5"
              />
            </div>
          {/each}
        </AccordionItem>
      </Accordion>
    </div>
    <div class="order-1 md:order-2 grid content-center" data-aos="fade-left">
      <img
        src="https://static.geekinsta.com/content/2020/05/web-development-frameworks.png"
        alt="techs"
      />
    </div>
  </div>
</div>
