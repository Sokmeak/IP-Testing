<template>
    <div class="fruits">
    <img :src="image" :alt="fruitName">
    <div class="name-price">
      <p>{{fruitName}}</p>
      <p class="price"><span>{{item}}</span>items</p>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    fruitName: String,
    item: Number, // Corrected prop type
    image: String,
  },
};
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Itim&display=swap');
   .fruits{
    border: 1px solid;
    display: flex;
    width: 120px;
    flex-direction: column;
    justify-content: center;
    align-items: center;
   }
   img{
  padding: 0;
  margin: 0;
  gap: 0;
  width: 120px;
  height: 120px;
   }
   .container{
    margin: 10px;
   }
   p{
    margin: 0;
    
   }
  p.price{
    display: flex;
   column-gap:10px;
   align-items: center;
   }
   .name-price{
    display: flex;
    flex-direction: column;
    align-items: center;
   }
   body{
    body {
  margin: 0;
  padding: 0;}
   }
   p{
    padding: 0;
  margin: 0;
  font-size: 16px;
  font-family:"Itim", cursive;
  font-style:oblique;
   }
   p span{
  font-size: 12px;
  color: gray;
}
.fruits{
  border: 1px solid #81b13d;
  background: #F2FCE4;
  border-radius: 10px;
 transition:all 0.2s ease-in-out;
}
.container{
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  padding-top: 10px;
}

.fruits:hover{
border: 1px solid #ca7878;
transform: scale(1.1);
transition: 0.2s;
}
</style>