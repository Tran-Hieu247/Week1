<template>
  <div>
    <div class="contact-list">
    <div class="mess">
        <div class="logo">
            SHOP.CO
        </div>
        <p>We have clothes that suits your style and which you’re proud to wear. From women to men.</p>
        <div class="social">
            <img src="../../assets/1.png">
            <img src="../../assets/2.png">
            <img src="../../assets/3.png">
            <img src="../../assets/4.png">
        </div>
    </div>
    <contact-item
      v-for="item in contactItems"
      :key="item.title"
      :title="item.title"
      :detail1="item.detail1"
      :detail2="item.detail2"
      :detail3="item.detail3"
      :detail4="item.detail4"
    ></contact-item>
  </div>
  <div>
    <v-divider></v-divider>
  </div>
  <div class="pay">
    <div>
        <div class="pay-title">Shop.co © 2000-2023, All Rights Reserved</div>
    </div>
    <div >
        <img src="../../assets/Visa.png">
        <img src="../../assets/Mastercard.png">
        <img src="../../assets/Paypal.png">
        <img src="../../assets/Pay.png">
        <img src="../../assets/GPay.png">
    </div>
  </div>
  </div>
</template>

<script>
import ContactItem from '../Contact/Item/ContactItem.vue'

export default {
  components: {
    ContactItem
  },
  data() {
    return {
      contactItems: [
        {
          title: 'COMPANY',
          detail1: 'About',
          detail2: 'Features',
          detail3: 'Works',
          detail4: 'Career'
        },
        {
          title: 'HELP',
          detail1: 'Customer Support',
          detail2: 'Delivery Details',
          detail3: 'Terms and Conditions',
          detail4: 'Privacy Policy'
        },
        {
          title: 'FAQ',
          detail1: 'Account',
          detail2: 'Manage Deliveries',
          detail3: 'Orders',
          detail4: 'Payments'
        },
        {
          title: 'RESOURCES',
          detail1: 'Free eBooks',
          detail2: 'Development Tutorial',
          detail3: 'How to Blog',
          detail4: 'Youtube Playlist'
        }
      ]
    }
  }
}
</script>

<style scoped>
.mess{
    width: 35%;
    height: 100%;
    padding-right: 130px;
}
.logo{
    font-family: Integral CF, sans-serif;
    font-size: 32px;
    letter-spacing: -.09em;
    font-weight: 800;
    line-height: 38.4px;
    text-align: left;
    margin-right: 50px;
    margin-top: -20px;
}

.mess p{
    font-family: Satoshi, sans-serif;
    font-size: 16px;
    text-align: left;
}

.contact-list{
    height: 350px;
    width: 100%;
    padding: 150px 100px;
    display: flex;
    justify-content: space-between;
    gap: 10px;
    background-color: #f0f0f0;
    border-radius: 10px;
}

p{
    width: 100%;
    height: 80%;
    font-weight: 400;
    line-height: 27px;
    opacity: 60%;
    margin-top:20px ;
}
v-divider{
    width: calc(100% - 200px);
    height: 1px;
    background-color: #000;
    opacity: .3;
    margin: 20px 100px 0 100px;
    position: relative
}
.pay{
    width: 100%;
    height: 100px;
    margin: 0 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #f0f0f0;
    margin-left: 0;
}
.pay-title{
    color: black;
    opacity: 60%;
    margin: 0 100px;
}

.social img{
    margin: 30px;
    border-radius: 50px;
    width: 30px;
    height: 30px;
    margin-left:0 ;
    
}

.social{
    display: flex;
    margin-top:20px ;
}
.pay img{
    display: flex;
}

</style>