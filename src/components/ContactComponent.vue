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
        background: white;
        padding: 30px;
        border-radius: 12px;
        box-shadow: 0 6px 18px rgba(0, 0, 0, 0.1);
        text-align: center;
        margin-top: 30px;
        max-width: 700px;
        margin-left: auto;
        margin-right: auto;
    }

    .contact h2 {
        color: #ff416c;
        font-size: 2rem;
        margin-bottom: 15px;
        text-transform: uppercase;
    }

    .contact p {
        font-size: 1.1rem;
        margin-bottom: 20px;
    }

    form {
        display: flex;
        flex-direction: column;
        gap: 15px;
    }

    input, textarea {
        padding: 12px;
        border: 1px solid #ccc;
        border-radius: 6px;
        font-size: 1rem;
        width: 100%;
    }

    textarea {
        min-height: 120px;
        resize: vertical;
    }

    button {
        background: #ff416c;
        color: white;
        border: none;
        padding: 12px;
        border-radius: 6px;
        font-size: 1rem;
        cursor: pointer;
        transition: 0.3s;
    }

    button:hover {
        background: #e1355c;
    }
</style>
    