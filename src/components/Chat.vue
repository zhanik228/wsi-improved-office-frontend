<template>
    <div class="sidebar__chat chat">
        <h2 class="chat__title">The Office</h2>
        <div class="chat__container">
            <p class="chat__container-message message">
                username: Message
            </p>
        </div>
        <form class="message-form" action="">
            <input type="text" placeholder="message">
            <button class="btn">Send</button>
        </form>
    </div>
</template>

<style scoped>
.chat {
    padding: 10px;
}
.chat__title {
    font-size: 18px;
    font-weight: 700;
}
.chat__container {
    height: 200px;
    border: 1px solid #5269b4;
    overflow: auto;
}

.message-form {
    display: flex;
    margin: 10px 0;
    border: 1px solid #5269b4;
    border-radius: 15px;
    padding: 10px 5px;
}

.message-form input {
    width: 100%;
    border: none;
}
</style>