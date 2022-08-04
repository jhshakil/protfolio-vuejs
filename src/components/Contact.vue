<template>
    <div class="m-16 bg-gray-300 rounded-lg">
        <h2 class="text-4xl font-bold text-center pt-8">Contact Me</h2>
        <div class="grid grid-cols-2 gap-8 items-center">
            <form class="p-8" @submit.prevent="sending()">
                <div class="my-4">
                    <label>Name</label>
                    <input type="text" v-model="user.name" 
                    class="border outline-none rounded border-black p-2 w-full" 
                    placeholder="Enter Your Name" required>
                </div>
                <div class="my-4">
                    <label>Email</label>
                    <input type="email" v-model="user.email" 
                    class="border outline-none rounded border-black p-2 w-full"
                    placeholder="Enter Your Email" required>
                </div>
                <div class="my-4">
                    <label>Message</label>
                    <input type="textarea" v-model="user.message" 
                    class="border outline-none rounded border-black p-2 w-full" 
                    placeholder="Enter Your Message" required>
                </div>
                <div class="my-4">
                    <input class="bg-orange-300 p-2 rounded-lg w-1/4 text-center font-bold" type="submit" value="Submit">
                </div>
            </form>
            <div>
                <div>
                    <div class="text-black p-2 rounded-md text-2xl text-center">Email: jhshakil11275@gmail.com</div>
                    <div class="text-black p-2 rounded-md text-2xl text-center">Mobile: +8801851891846</div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
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
            console.log(this.user)
        }
    }
}
</script>