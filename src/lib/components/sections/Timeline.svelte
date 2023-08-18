<script>
  import { Timeline, TimelineItem, Button } from "flowbite-svelte";
  import HeaderTitle from "./HeaderTitle.svelte";
</script>

<div id="timeline-section">
  <HeaderTitle title="Timeline" subtitle="Seminar/Training Attended" />
  <div class="flex justify-center">
    <Timeline>
      <TimelineItem
        title="Vue JS Workshop Speaker @ DMMMSU SLUC"
        date="March 2023"
        data-aos="fade-left"
      >
        <p
          class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400"
          data-aos="fade-left"
        >
          Training computer science students on how to create a progressive web
          applications using Vue js.
        </p>
        <Button
          data-aos="fade-left"
          color="alternative"
          on:click={() =>
            window.open(
              "https://www.facebook.com/photo?fbid=665112145418366&set=pcb.665117418751172",
              "_blank"
            )}
          >Learn more<svg
            class="ml-2 w-3 h-3"
            fill="currentColor"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
            ><path
              fill-rule="evenodd"
              d="M12.293 5.293a1 1 0 011.414 0l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-2.293-2.293a1 1 0 010-1.414z"
              clip-rule="evenodd"
            /></svg
          ></Button
        >
      </TimelineItem>
      <TimelineItem
        title="MERN Stack Development Training"
        date="May 2022"
        data-aos="fade-left"
      >
        <p
          class="text-base font-normal text-gray-500 dark:text-gray-400"
          data-aos="fade-left"
        >
          MERN Stack Development Online Bootcamp.
        </p>
      </TimelineItem>
      <TimelineItem
        title="Hackathon 2019"
        date="March 9, 2019"
        data-aos="fade-left"
      >
        <p
          class="text-base font-normal text-gray-500 dark:text-gray-400"
          data-aos="fade-left"
        >
          Participate in Provincial School Hackathon 2019
        </p>
      </TimelineItem>
      <TimelineItem
        title="Web Design Technology Competition"
        date="March 5, 2019"
        data-aos="fade-left"
      >
        <p
          class="text-base font-normal text-gray-500 dark:text-gray-400"
          data-aos="fade-left"
        >
          Web Design Technology 10th La Union Provincial Skills Olympics
        </p>
      </TimelineItem>
    </Timeline>
  </div>
</div>
