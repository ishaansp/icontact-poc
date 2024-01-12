<template>
  <div>
<nuxt-link to="/"> go to home </nuxt-link>

    	<button
						v-b-modal.modal-2
					>open</button>
    <b-modal @shown="showForm" id="modal-2" no-close-on-backdrop centered>
      <div>
      <div> loading </div>
      <div id="mycustomform"> </div>
      </div>

    </b-modal>
  </div>
</template>

<script>
import Contact from "../components/contact.vue";

export default {
  components: {
    Contact,
  },
  methods:{
    showForm(){
      console.log('form')
      var iDiv = document.createElement('div');
iDiv.id = 'icontactSignupFormWrapper473';
var a=document.getElementById("mycustomform");
a.appendChild(iDiv)
console.log("a",a)
// document.getElementsById('mycustomform').appendChild(iDiv);

const script = document.createElement('script')
		script.type = 'text/javascript'
		script.src = "https://app.icontact.com/icp/core/mycontacts/signup/designer/form/automatic?id=473&cid=1912706&lid=7659&divid=icontactSignupFormWrapper473"
		script.async = true
		script.defer = true

		this.scriptele = document.body.appendChild(script)


    }
  }
};
</script>
