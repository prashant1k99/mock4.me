<template>
  <div class="home">
    <StackList>
      <li v-for="position in positions" :key="position.id">
        <stack-list-item>
          <p class="truncate text-sm font-medium text-indigo-600">{{ position.title }}</p>
          <div class="ml-2 flex flex-shrink-0">
            <p class="inline-flex rounded-full bg-green-100 px-2 text-xs font-semibold leading-5 text-green-800">{{ position.type }}</p>
          </div>
        </stack-list-item>
      </li>
    </StackList>

    <Tags class="bg-yellow-100 text-yellow-800 border-5 " large >I Am Happy</Tags>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import StackList from '@/components/template/StackList.vue';
import Tags from '../components/template/Tags.vue';
import StackListItem from '@/components/template/StackListItem.vue';

export default defineComponent({
  name: 'HomeView',
  components: {
    StackList,
    Tags,
    StackListItem
  },
  data() {
    return {
      positions
    }
  }
});
const positions = [
  {
    id: 1,
    title: 'Back End Developer',
    type: 'Full-time',
    location: 'Remote',
    department: 'Engineering',
    closeDate: '2020-01-07',
    closeDateFull: 'January 7, 2020',
  },
  {
    id: 2,
    title: 'Front End Developer',
    type: 'Full-time',
    location: 'Remote',
    department: 'Engineering',
    closeDate: '2020-01-07',
    closeDateFull: 'January 7, 2020',
  },
  {
    id: 3,
    title: 'User Interface Designer',
    type: 'Full-time',
    location: 'Remote',
    department: 'Design',
    closeDate: '2020-01-14',
    closeDateFull: 'January 14, 2020',
  },
]
</script>
