<template>
    <div class="chat-composer">
        <input type="text" placeholder="Type your message ...." v-model="message" v-on:keyup.enter="sendMessage">
        <button class="btn btn-primary" @click="sendMessage">Send</button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            message: ''
        }
    },
    methods: {
        sendMessage() {
            this.$emit('messagesent' , {
                message: this.message,
                user: 'vincent'
            });
            this.message = '';
        }
    }

}
</script>

<style lang="css">
.chat-composer {
    display: flex;
}
.chat-composer input {
    flex: 1 auto;
}
.chat-composer button {
    border-radius: 0;
}
</style>