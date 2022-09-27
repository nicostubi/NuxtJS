<template>
  <div>
  <img :src="home.images[0]" style="width:200px" /><br />
  {{ home.title}}<br />
  {{ home.location.address}}{{ home.location.city}}{{ home.location.state}}<br />
  {{ home.guests}} guests<br />
  {{ home.pricePerNight}} / night<br />
  </div>
</template>
<script>
import { defineComponent } from '@vue/composition-api'

export default {
  props: {
    home: 
    {
    type: Object,
      required: true
    }
  }
</script>
