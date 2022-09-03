<template>
  <div class="home">
    <StackList />
    <Tags class="bg-yellow-100 text-yellow-800 border-5 " large >I Am Happy</Tags>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import StackList from '@/components/template/StackList.vue';
import Tags from '../components/template/Tags.vue'; // @ is an alias to /src

export default defineComponent({
  name: 'HomeView',
  components: {
    StackList,
    Tags
},
});
</script>
