<template>
    <div class="clearAllContainer">
        <span class="clearAllBtn" @click="clearTodo">Clear All</span>
    </div>
</template>

<script>
export default {
    methods: {
        // removeAll 이벤트를 발생시켜 App 컴포넌트로 전달하는 로직
        clearTodo() {
            this.$emit('removeAll');
        }
    }
}
</script>

<style scoped>
.clearAllContainer {
    width: 8.5em;
    height: 50px;
    line-height: 50px;
    background-color: white;
    border-radius: 5px;
    margin: 0 auto;    
}
.clearAllBtn {
    color: #e20303;
    display: black;
}
</style>