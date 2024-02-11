<template>
    <div class="sidebar-header__user-info user-info">
        <img :src="avatar" width="64" alt="avatar" class="user-info__img">
        <div class="user-info__content">
            <p class="user-info__username">Username</p>
            <p class="user-info__session-length">Being at work 3h 46m</p>
        </div>
        <button class="btn btn_danger">log out</button>
    </div>
</template>

<script>
import avatar from '@/assets/avatars/avatar-01.svg'

export default {
    data() {
        return {
            avatar
        }
    }
}
</script>

<style scoped>
.user-info {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 10px;
    padding: 10px;
}

.user-info__content {
    flex-shrink: 0;
}

.user-info__username {
    font-size: 18px;
    color: #5269b4;
}

.user-info__session-length {
    color: #5269b4;
    opacity: .7;
}
</style>