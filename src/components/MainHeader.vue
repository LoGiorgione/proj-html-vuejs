<template>
  <section class="mt-5">
    <Paragraph
      class="mb-5"
      :icon="icon"
      :title="title"
      :paragraph="paragraph"
      :buttonText="buttonText"
      :buttonColor="buttonColor"
      :illustration="illustration"
      :invert="invert"
    />
  </section>
</template>

<script>
import Paragraph from "./Paragraph.vue";
export default {
  name: "MainHeader",
  components: {
    Paragraph,
  },
  data() {
    return {
      icon: require("../assets/img/Books-icon.png"),
      title: "Thousands of courses for any type of student",
      paragraph:
        "At EduPrime, it doesn't matter what domanin you wish to pursue a career in. Here you can find a course that satisfies your needs within a click away and applies for a course in a matter of minutes. EduPrime is ranked as the most versatile university in the world, thanks to the number of courses it provides.",
      buttonText: "Browse through courses",
      buttonColor: "bg-yellow",
      illustration: require("../assets/img/Graduation-Illustration.png"),
      invert: false,
    };
  },
};
</script>

<style lang="scss" scoped>
a {
  &:hover {
    background-color: #fff;
    color: $both-primary;
  }
}
</style>