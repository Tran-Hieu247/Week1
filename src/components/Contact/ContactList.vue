<template>
    <div class="contact-list">
        <contact-item :Title="COMPANY" :detal1="About" :detal2="Features" :detal3="Works" :detal4="Carrer"></contact-item>
        <contact-item :Title="HELP" :detal1="Customer-Support" :detal2="Delivery-Details" :detal3="Terms-and-Conditions" :detal4="Privacy-policy"></contact-item>
        <contact-item :Title="FAQ" :detal1="Account" :detal2="Manage-Deliveries" :detal3="Orders" :detal4="Payments"></contact-item>
        <contact-item :Title="RESOURCES" :detal1="Free-eBooks" :detal2="Development-Tutorial" :detal3="How-to - Blog" :detal4="Youtube-Playlist"></contact-item>
    </div>
</template>
<script>
import ContactItem from './Item/ContactItem.vue'
export default {
  components: { ContactItem },
    component:{
        ContactItem
    }
}
</script>

<style scoped>

</style>