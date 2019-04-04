<template>
    <div class="chat-log">
        <chat-message v-for="msg in messages" v-bind:message="msg" v-bind:key="m"></chat-message>
    </div>
</template>
<script>
export default {
    props: ['messages' , 'm']
}
</script>

<style>
    .chat-log .chat-message:nth-child(even) {
        
        background: #ccc;
    }
    .chat-log .chat-message {
        padding: 10px;
    }
</style>