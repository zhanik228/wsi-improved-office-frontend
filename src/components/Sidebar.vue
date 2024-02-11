<template>
    <div class="sidebar">
        <div class="sidebar-header">
            <h2 class="sidebar-title">Chat List</h2>
            <ChatList />
        </div>
        <div class="sidebar-body">
            <h2 class="sidebar-title">Chat</h2>
            <Chat />
        </div>
        <div class="sidebar-footer">
            <ProfileCard />
        </div>
    </div>
</template>

<script>
import avatar from '@/assets/avatars/avatar-01.svg'

import Chat from '@/components/Chat.vue'
import ChatList from '@/components/ChatList.vue'
import ProfileCard from '@/components/ProfileCard.vue'

export default {
    components: {
        Chat,
        ChatList,
        ProfileCard
    },
    data() {
        return {
            avatar
        }
    }
}
</script>

<style scoped>
.sidebar {
    box-shadow: 0px 1px 4px #eee7e7;
    border-radius: 15px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 100%;
    position: fixed;
}

.sidebar-title {
    text-transform: uppercase;
    padding-left: 5px;
    border-bottom: 1px solid #5269b4;
    padding-bottom: 5px;
    text-align: center;
}

.sidebar-header {
    padding-bottom: 10px;
}
/* user info */
.sidebar-header__user-info {
    border-top: 1px solid #5269b4;
}
/* list */

/* chat */
.sidebar__chat {
    border-top: 1px solid #5269b4;
}
</style>