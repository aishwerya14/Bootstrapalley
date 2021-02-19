<template>
    <div class="contact-us-wrap">
        <div class="container">
            <div class="row">
                <div class="col-sm-12 col-lg-3">
                    <div class="contact title-sec">
                        <h3 class="text-left">Say Hello</h3>
                    </div>
                    <h4>BOOTSTRAPALLEY</h4>
                    <h5> B-7/8, Anmol Pride, Baner<br> Pune 411045 </h5>
                    <h5> <a href="tel:+91 20 4075 1111">+91 20 4075 1111</a></h5>
                    <h5> <a href="tel:+91 20 4075 1177">+91 20 4075 1177</a></h5>
                    <a class="mail" href="mailto:bootstrap-alley@talentica.com">bootstrap-alley@talentica.com</a>
                </div>
                 <div class="col-sm-12 col-lg-3"></div>
                <div class="col-sm-12 col-lg-6">
                    <div class="title-sec">
                        <h3>Say Hello</h3>
                    </div>
                    <form :class="this.errors ? 'errors' : false">
                        <input type="text" placeholder="* Name" id="name" v-model="name" required @invalid="invalidateForm" >
                        <input type="email" placeholder="* Email Id" id="email" v-model="email" required  @invalid="invalidateForm">
                        <input type="number" placeholder="Contact no">
                        <textarea rows="1">Message</textarea>
                        <div class="ml-auto text-left">
                            <button type="submit" class="btn orange-btn">Submit</button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data () {
        return { 
            valid: false,
            name: '',
            errors:'',
            nameRules: [
              (v) => !!v || 'Name is required',
              (v) => v.length <= 10 || 'Name must be less than 10 characters'
            ],
            email: '',
            // emailRules: [
            //   (v) => !!v || 'E-mail is required',
            //   (v) => /^\w+([\.-]?\w+)*@\w+([\.-]?\w+)*(\.\w{2,3})+$/.test(v) || 'E-mail must be valid'
            // ]
        }
    },
    methods: {
            invalidateForm() {
            this.errors = true;
        }
    }
}
</script>