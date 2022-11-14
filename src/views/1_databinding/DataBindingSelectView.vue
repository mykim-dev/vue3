<template>
    <div>
        <select v-model="selectedCity" @change="selectChange()">
            <option value=""></option>
            <option value="02">서울</option>
            <option value="051">부산</option>
            <option value="064">제주</option>
        </select>
        
    </div>
</template>

<script>
export default{ 
    name:'',
    components:{},
    data(){
        return{
            selectedCity:'051'
        };
    },
    setup(){},
    created(){},
    mounted(){},
    unmounted(){},
    methods:{
        selectChange() {
            
        }
    }
}
</script>