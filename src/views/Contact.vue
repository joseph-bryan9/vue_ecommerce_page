<template>
  <div class="contact">
    <ContactBanner />
    <ContactDetails />
  </div>
</template>

<script>
import ContactBanner from "../components/Contact/ContactBanner";
import ContactDetails from "../components/Contact/ContactDetails";

export default {
  name: "Contact",
  components: {
    ContactBanner,
    ContactDetails,
  },
};
</script>
