<template>
    <div>
        <div>
            <input 
                type="checkbox"
                id="html"
                value="html"
                v-model="favoriteLang"
            />
            <label for="html">HTML</label>
        </div>
        <div>
            <input
                type="checkbox"
                id="css"
                value="css"
                v-model="favoriteLang" 
            />
            <label for="css">CSS</label>
        </div>
        <div>
            <input
                type="checkbox"
                id="js"
                value="js"
                v-model="favoriteLang" 
            />
            <label for="js">JAVASCRIPT</label>
        </div>
        <div>선택한 언어: {{ favoriteLang }}</div>
        
    </div>
</template>
<script>

export default{ 
    name:'',
    components:{},
    data(){
        return{
            favoriteLang: ['html','css']
        };
    },
    setup(){},
    created(){},
    mounted(){},
    unmounted(){},
    methods:{}
}
</script>