<template>
  <div class="user-card">
    <img :src="userImage" alt="avatar" class="user-avatar"/>
    <h2 class="titulo">{{ userName }}</h2>
    <p class="texto">{{ userEmail }}</p>
    <p class="texto">{{ userBio }}</p>
  </div>
</template>

<script>
export default {
  props: {
    userName:{
      type: String,
      required: true,
    },
    userEmail: {
      type: String,
      required: true,
    },
    userBio:{
      type: String,
      required: true,
    },
    userImage:{
      type: String,
      required: true,
    },
  },
};
</script>
<style>
.user-card{
  border: 1px solid #ccc;
  padding: 16px;
  margin: 16px;
  width: 300px;
  background-color: #f8f8f8;
  border-radius: 12px;
  box-shadow: 0 0 5px rgba(0,0,0,0.2);
  text-align: center;

}
.texto{
  color: #2c3e50;
}
.titulo{
  color: #181818;
}
.user-avatar{
  max-width: 100%;
  height: auto;
  //border-radius: 89%;
}
</style>