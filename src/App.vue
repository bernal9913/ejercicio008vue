<template>
  <div>
    <h1>PErfil de usuario</h1>
    <user-card
        user-bio="Desarrollador movil frustrado usando vue"
        user-email="bernalgas@gmail.com"
        user-name="Carlos ramirez"
        user-image="https://assets.stickpng.com/images/580b57fcd9996e24bc43c325.png"
    />

  </div>
</template>
<script>
import UserCard from "@/UserCard.vue";
export default {
  components:{
    UserCard,
  },
};
</script>