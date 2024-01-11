<template>
  <div>
<nuxt-link to="/"> go to home </nuxt-link>

    	<button
						v-b-modal.modal-2
					>open</button>
    <b-modal id="modal-2" no-close-on-backdrop centered>
<div id="icontactSignupFormWrapper473"><script type="text/javascript" async src="https://app.icontact.com/icp/core/mycontacts/signup/designer/form/automatic?id=473&cid=1912706&lid=7659&divid=icontactSignupFormWrapper473"></script></div>

    </b-modal>
  </div>
</template>

<script>
import Contact from "../components/contact.vue";

export default {
  components: {
    Contact,
  },
};
</script>
