<template>
  <div>
    <h5>
        <router-link to="/detail">
            {{ blogWrite[0].title }}
        </router-link>
    </h5>
    <p>{{ blogWrite[0].date }}</p>
  </div>
  <div>
    <h5>
        {{ blogWrite[1].title }}</h5>
    <p>{{ blogWrite[1].date }}</p>
  </div>
  <div>
    <h5>{{ blogWrite[2].title }}</h5>
    <p>{{ blogWrite[2].date }}</p>
  </div>
</template>

<script>
export default {
    name: 'BlogList',
    props: {
        blogWrite: Array,
    },
    data() {
        return {

        }
    }
}
</script>

<style>

</style>