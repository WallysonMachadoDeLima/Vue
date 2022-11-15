<template>
  <img :src="avatar" :alt="descricao" style="width: 150px" />
</template>

<script>
export default {
  name: "Picture",
  data() {
    return {
      avatar:
        "https://www.tailorbrands.com/wp-content/uploads/2020/07/mcdonalds-logo.jpg",
      descricao: "Logo Mc Jorge",
    };
  },
};
</script>