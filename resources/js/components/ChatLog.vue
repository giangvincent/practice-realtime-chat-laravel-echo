<template>
    <div class="chat-log">
        <chat-message v-for="msg in messages" v-bind:message="msg" v-bind:key="msg"></chat-message>
    </div>
</template>
<script>
export default {
    props: ['messages']
}
</script>

<style>
    
</style>