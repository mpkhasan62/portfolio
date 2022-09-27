<template>
  <div v-for="project in projects" :key="project.id">
    <CertificateDetails :project="project" />
  </div>
</template>

<script>
import CertificateDetails from "./CertificateDetails.vue";
export default {
  props: {
    projects: {
      type: Array,
      default: [],
    },
  },

  components: {
    CertificateDetails,
  },
};
</script>
