<template>
 <div class="row">
  <div class="col-3" v-for="employees in employees" :key="employees.id">
    <CardComVue :data="employees"/>
  </div>
 </div>
 <div class="row mt-3">
  <ul class="list-group" >
    <ListComVue v-for="employees in employees" :key="employees.id" :name="employees.name"/>
  </ul>
 </div>
</template>

<script>
import CardComVue from '@/components/CardCom.vue';
import ListComVue from '@/components/ListCom.vue';
export default {
  name: "AboutView",
  components: {
    CardComVue,
    ListComVue
  },
  data() {
    return {
      employees: [
        {
          id: 1,
          name: "Koko",
          image:
            "https://fiverr-res.cloudinary.com/images/t_main1,q_auto,f_auto,q_auto,f_auto/gigs2/321289941/original/ef78d4523ccbfea028c454417c2f3504572a3de5/draw-avatar-cartoon-from-your-photo.jpg",
          description:
            "You now have a Vue 3 project set up with Vue Router and Bootstrap. ",
        },
        {
          id: 1,
          name: "Dodo",
          image:
            "https://fiverr-res.cloudinary.com/images/t_main1,q_auto,f_auto,q_auto,f_auto/gigs2/321289941/original/ef78d4523ccbfea028c454417c2f3504572a3de5/draw-avatar-cartoon-from-your-photo.jpg",
          description:
            "You now have a Vue 3 project set up with Vue Router and Bootstrap. ",
        },
        {
          id: 1,
          name: "Juju",
          image:
            "https://fiverr-res.cloudinary.com/images/t_main1,q_auto,f_auto,q_auto,f_auto/gigs2/321289941/original/ef78d4523ccbfea028c454417c2f3504572a3de5/draw-avatar-cartoon-from-your-photo.jpg",
          description:
            "You now have a Vue 3 project set up with Vue Router and Bootstrap. ",
        },
        {
          id: 1,
          name: "Ruru",
          image:
            "https://fiverr-res.cloudinary.com/images/t_main1,q_auto,f_auto,q_auto,f_auto/gigs2/321289941/original/ef78d4523ccbfea028c454417c2f3504572a3de5/draw-avatar-cartoon-from-your-photo.jpg",
          description:
            "You now have a Vue 3 project set up with Vue Router and Bootstrap. ",
        },
      ],
    };
  },
};
</script>