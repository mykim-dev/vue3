<template>
    <div>
        <!-- v-model은 양방향 Bingding인데 양방향 Binding이 필요없을 경우 v-bind 사용  -->
        <input type="text" name="" id="" v-bind:value="userId" readonly />
        <br />

        <!-- v-bind는 생략이 가능하다 -->
        <input type="text" name="" id="" :value="userId" readonly />
        <br />

        <!--  -->
        <img :src="imgSrc" alt="" style="width:100px; height:auto;" />
        <br />

        <input type="search" v-model="txt1" />
        <button :disabled="txt1 === ''">조회</button>
    </div>
</template>
<script>

export default{ 
    name:'',
    components:{},
    data(){
        return{
            userId:'mykim',
            imgSrc: "https://vuejs.org/images/vuemastery/logo-vuemastery.svg",
            txt1: ""
        };
    },
    setup(){},
    created(){},
    mounted(){},
    unmounted(){},
    methods:{}
}
</script>