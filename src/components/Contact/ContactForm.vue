<template>
  <form class="contact-form">
    <input type="text" name="name" placeholder="Name" />
    <input type="email" name="email" placeholder="Email" />
    <input type="text" name="phone" placeholder="Phone Number" />
    <textarea placeholder="Message"></textarea>
    <input type="button" value="Send" />
  </form>
</template>

<script>
export default {
  name: "ContactForm"
};
</script>

<style scoped>
.contact-form {
  width: 70%;
  margin: 0 auto;
  height: 26rem;
  text-align: center;
}
.contact-form input[type="text"],
.contact-form input[type="email"],
.contact-form textarea {
  box-sizing: border-box;
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  outline: none;
  display: block;
  width: 100%;
  border: none;
  border-bottom: 1px solid #ffffff;
  background: transparent;
  margin-bottom: 10px;
  height: 4rem;
  font-size: 12px;
  color: #ffffff;
}
.contact-form input[type="button"] {
  margin-top: 2rem;
  width: 10rem;
  height: 2.3rem;
  background: #eda911;
  color: #ffffff;
  border: none;
  border-radius: 20px;
}
::placeholder {
  color: #ffffff;
}
</style>
