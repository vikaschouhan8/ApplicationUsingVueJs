<template>
  <div>
    <app-header :title="title"></app-header>
    <app-ninjas :ninjas="ninjas"></app-ninjas>
    <app-footer :title="title"></app-footer>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Ninjas from './components/Ninjas.vue'

export default {
  components: {
    'app-header': Header,
    'app-footer': Footer,
    'app-ninjas': Ninjas
  },
  data () {
    return {
      ninjas: [
        {name:'vikash1', speciality:'He is a Batsman', show:'false'},
        {name:'vikash2', speciality:'He is a bowler2', show:'false'},
        {name:'vikash3', speciality:'He is a bowler', show:'false'},
        {name:'vikash4', speciality:'He is a bowler', show:'false'},
        {name:'vikash5', speciality:'He is a bowler', show:'false'},
        {name:'vikash6', speciality:'He is a bowler', show:'false'},        
      ],
      title: 'Vikas VueJs App'
    }
  }
}
</script>

<style>

</style>
