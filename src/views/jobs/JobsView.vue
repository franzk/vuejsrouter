<template>
  <h1>Jobs</h1>
  <div v-for="job in jobs" :key="job.id">
    <router-link :to="{ name: 'jobDetails', params: { id: job.id} }"> {{ job.title }}</router-link>
  </div>
</template>

<script>
export default {
  data() {
    return {
      jobs: [
        {title: 'Java developer', id: 1, details: 'lorem'},
        {title: 'Angular developer', id: 2, details: 'lorem'},
        {title: 'Vue developer', id: 3, details: 'lorem'},
      ]
    }
  }
}
</script>

<style>

</style>