<template>
  <div class="row">
    <div class="col-3" v-for="user in users" :key="user.id">
      <CardCom :data="user"/>
    </div>
  </div>
  <div class="row mt-3">
    <AlertComVue v-for="user in users" :key="user.id" :name="user.name"/>
  </div>
</template>

<script>
// @ is an alias to /src
import CardCom from '@/components/CardCom.vue'
import AlertComVue from '@/components/AlertCom.vue'
export default {
  name: 'HomeView',
  components: {
    CardCom,
    AlertComVue
  },
  data() {
    return {
      users: [
        {
          id: 1,
          name: "Visal",
          image: 'https://t3.ftcdn.net/jpg/06/17/13/26/360_F_617132669_YptvM7fIuczaUbYYpMe3VTLimwZwzlWf.jpg',
          description: 'You now have a Vue 3 project set up with Vue Router and Bootstrap.'
        },
        {
          id: 1,
          name: "Chetra",
          image: 'https://t3.ftcdn.net/jpg/06/17/13/26/360_F_617132669_YptvM7fIuczaUbYYpMe3VTLimwZwzlWf.jpg',
          description: 'You now have a Vue 3 project set up with Vue Router and Bootstrap. '
        },
        {
          id: 1,
          name: "Dara",
          image: 'https://t3.ftcdn.net/jpg/06/17/13/26/360_F_617132669_YptvM7fIuczaUbYYpMe3VTLimwZwzlWf.jpg',
          description: 'You now have a Vue 3 project set up with Vue Router and Bootstrap. '
        },
        {
          id: 1,
          name: "Romdul",
          image: 'https://t3.ftcdn.net/jpg/06/17/13/26/360_F_617132669_YptvM7fIuczaUbYYpMe3VTLimwZwzlWf.jpg',
          description: 'You now have a Vue 3 project set up with Vue Router and Bootstrap. '
        }
      ]
    }
  }
}
</script>
