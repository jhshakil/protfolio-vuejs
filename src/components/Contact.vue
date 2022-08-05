<template>
    <div class="my-12 lg:m-16 bg-gray-200 rounded-lg">
        <h2 class="text-2xl lg:text-4xl font-bold text-center pt-4 lg:pt-8">Contact Me</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8 items-center">
            <form ref="form" class="p-8" @submit.prevent="sending()">
                <div class="my-4">
                    <label>Name</label>
                    <input type="text" v-model="user.name" name='user_name' 
                    class="border outline-none rounded border-black p-2 w-full" 
                    placeholder="Enter Your Name" required>
                </div>
                <div class="my-4">
                    <label>Email</label>
                    <input type="email" v-model="user.email" name='user_email' 
                    class="border outline-none rounded border-black p-2 w-full"
                    placeholder="Enter Your Email" required>
                </div>
                <div class="my-4">
                    <label>Message</label>
                    <input type="textarea" v-model="user.message" name='message' 
                    class="border outline-none rounded border-black p-2 w-full" 
                    placeholder="Enter Your Message" required>
                </div>
                <div class="my-4">
                    <input class="bg-orange-300 p-2 rounded-lg w-1/4 text-center font-bold" type="submit" value="Submit">
                </div>
            </form>
            <div>
                <div>
                    <div class="p-1 lg:p-2 rounded-md text-lg lg:text-2xl text-center">Email: jhshakil11275@gmail.com</div>
                    <div class="p-1 lg:p-2 rounded-md text-lg lg:text-2xl text-center">Mobile: +8801851891846</div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import emailjs from '@emailjs/browser';

export default {
    name: 'contactMe',
    data: function(){
        return{
            user: {
                name: '',
                email: '',
                message: ''
            }
        }
    },
    methods: {
        sending: function( ) {
            console.log(this.$refs.form)
            emailjs.sendForm('service_a0bsj82', 'template_k26yajd', this.$refs.form, 'OCqvS9D0ZS5iL2fkz')
        .then((result) => {
            console.log('SUCCESS!', result.text);
            this.user.name = '';
            this.user.email = '';
            this.user.message = '';
        }, (error) => {
            console.log('FAILED...', error.text);
        });
        }
    }
}
</script>