<template>
<Container>
<ChatWindow>
<ChatMessage>
</ChatMessage>
</ChatWindow>
</Container>
</template>
<script>
import Container from "./components/MyContainer.vue";

export default {
  name: "App",
  components: {
    Container,
  },
};
</script>
<style>
body {
  margin: 0;
  background-color: #f9f9fa;
}
</style>
