<template>
  <section class="contact-us">
    <div class="center-flex-items header">
      <h1>趕快聯絡</h1>
    </div>
    <hr/>
    <div class="center-flex-items contacts">
      <div class="personal-contact" v-for="pc in personalContact">
        <div :style="{'background-image': `url(${pc.photo})`}" class="circle-photo"/>
        <h2>{{pc.name}}</h2>
        <h4>{{pc.lineId}}</h4>
        <p>{{pc.description}}</p>
      </div> 
    </div>
  </section>
</template>
<script>
  export default {
    name: 'Contact',
    data() {
      return {
        personalContact: [
          {
            name: 'Yicheng',
            lineId: 'LineId',
            description: 'Description',
            photo: 'http://cdn2-www.comingsoon.net/assets/uploads/gallery/best-to-worst-jason-voorhees-STYD/f-vs-jason.jpg',
          },
          {
            name: 'Jimmy',
            lineId: 'LineId',
            description: 'Description',
            photo: 'https://s-media-cache-ak0.pinimg.com/originals/67/f4/5b/67f45bfaec55243a3fe873c7e35def29.jpg',
          },
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>
  
  @import '../assets/common.scss';

  .contact-us {
    background-color: #ff4154;
    color: white;
    height: 500px;
  }
  .contacts {
    margin-top: 70px;
    justify-content: space-around;
  }
  .circle-photo {
    width: 144px;
    height: 144px;
    border:none;
    border-radius: 72px;
    background-color: #789;
    background-size:cover;
    background-position: center center;
  }
  .personal-contact {
    align-self: center;
  }

</style>