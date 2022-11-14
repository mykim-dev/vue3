<template>
    <div>
        <h1> Hello {{ userName }}</h1>
        <p>{{ message }}</p>
    </div>    
</template>
<script>
export default {
    data() {
        return {
            userName: "Jone Doe",
            message: "Welcome 개발자의 품격",
            arr: [],
            obj: {}
        }
    }
}
</script>
<style scoped>
/* 이 화면에서만 사용해야할 스타일을 정의 할때  scoped */
</style>