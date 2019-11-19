<template>
  <div class="home">
      <myHead></myHead>
   <myindex></myindex>
   <myFooter></myFooter>
  </div>
</template>

<script>
// @ is an alias to /src
import myHead from '@/components/my_head.vue'
import myindex from '@/components/index.vue'
import myFooter from '@/components/my_footer.vue'
export default {
  name: 'home',
  components: {
    myindex,
    myHead,
    myFooter
  
  }
}
</script>
