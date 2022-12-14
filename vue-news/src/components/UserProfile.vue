<template>
    <div class="user-container">
        <div>
            <i class="fas fa-user"></i>
        </div>
        <div class="user-desc">
            <!-- <div>username : {{ info.id}}</div> -->
            <slot name="username">

            </slot>
            
            <div class="time">
                <!-- time : {{ info.created }} -->
                <slot name="time">

                </slot>
                <slot name="karma">
                
                </slot>
            </div>   
        </div>
    </div>
</template>

<script>
export default {
    props: {
        info: Object
    },
    // computed: {
    //     userInfo() {
    //         return this.$store.state.user;
    //     }
    // },

}
</script>

<style scoped>
.user-container {
    display: flex;
    align-items: center;
    padding: 0.5rem;
}

.fa-user {
    font-size: 2.5rem;
}

.user-desc {
    padding: 8px;

}

.time {
    font-size: .7rem
}
</style>