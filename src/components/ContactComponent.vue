<template>
    <div class="contact">
        <h2>Contact Me</h2>
        <p>Email: {{form.email}}</p>
        <!--<p>If you'd like to contact me, feel free to use the form below:</p>
        <form @submit.prevent="submitForm">
            <input type="text" v-model="form.name" placeholder="Your Name" required />
            <input type="email" v-model="form.email" placeholder="Your Email" required />
            <textarea v-model="form.message" placeholder="Your Message" required></textarea>
            <button type="submit">Send</button>
        </form>-->
    </div>
</template>

<script>
    export default {
        name: "ContactComponent",
        data() {
            return {
                form: {
                    name: "",
                    email: "hossam.4na@hotmail.com",
                    message: ""
                }
            };
        },
    };
</script>

<style scoped>
    .contact {
        padding: 1.875rem;            
        margin-top: 1.875rem;        
        border-bottom: 0.125rem solid #dfdada; 
    }

    .contact p {
        font-size: 1.1rem;    
        margin-bottom: 1.25rem;        
    }
</style>
    