<template>
    <div>
        <!-- <input type="search" @keyup="checkEnter($event)" v-model="searchText" /> -->
        <input type="search" @keyup.enter="doSearch" v-model="searchText" />
        <button @click="doSearch">조회</button>
        <button type="submit" @click.prevent="doSearch">전송</button>
    </div>
</template>

<script>
// .delete
// .space
// .tab
// .esc
// .space
// .up
// .down
// .left
// .right
// .stop - event.stopPropagation()

export default{ 
    name:'',
    components:{},
    data(){
        return{
            searchText: ''
        };
    },
    setup(){},
    created(){},
    mounted(){},
    unmounted(){},
    methods:{
        doSearch() {
            console.log(this.searchText)
        },
        checkEnter(event) {
            // console.log(event)
            if(event.keyCode === 13)
                this.doSearch();
        }
    }
}
</script>