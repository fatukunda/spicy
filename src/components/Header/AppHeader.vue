<template>
  <div class="container-fluid main">
    <div class="row">
      <div class="col-md-6">
        <div class="row">
          <div class="col-md-4">
            <h5 class="brand">Spicy</h5>
          </div>
          <div class="col-md-8 nav-items">
            <NavItems />
          </div>
        </div>
        <div class="row">
          <AppIntro />
        </div>
      </div>
      <div class="col-md-6">
        <div class="row call-row">
          <div class="col-md-12">
            <p class="call-us">Call Us: +256 772 16 7656</p>
          </div>
        </div>
        <div class="row contact mt-4">
          <div class="col-md-12">
            <ContactForm />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import NavItems from "../Navigation/NavItems";
import AppIntro from "./AppIntro";
import ContactForm from "../Contact/ContactForm";
export default {
  name: "AppHeader",
  components: {
    NavItems,
    AppIntro,
    ContactForm
  }
};
</script>

<style scoped>
.main {
  background-color: #eae9e4;
  height: 600px;
}
.brand {
  color: #5a2f27;
  font-weight: bold;
  padding-top: 2rem;
  margin-left: 10rem;
}
a {
  color: #eda911;
}
.nav-items {
  padding-top: 2rem;
}
.contact {
  width: 50%;
  background: #5a2f27;
  border-radius: 5px;
  box-shadow: 0px -6px 3px #eda911;
}
.call-row {
  width: 50%;
  margin-top: 2rem;
  color: #eda911;
}
.call-us {
  float: right;
  font-size: 13px;
}

@media screen and (max-width: 600px) {
  .brand {
    margin-left: 0;
    text-align: center;
  }
  .contact {
    width: 100%;
    margin: 0 auto;
  }
}
</style>
