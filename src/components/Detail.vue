<template>
  
  <div>
    <h3>상세페이지임 아무튼 그럼</h3>
    <h5>{{ blogWrite[$route.params.id].title }}</h5>
    <p>{{ blogWrite[$route.params.id].content }}</p>
    
  </div>
  
  <router-view></router-view>

</template>

<script>
export default {
    name: 'BlogDetail',
    props: {
        blogWrite: Array,
    },
}
</script>

<style>

</style>