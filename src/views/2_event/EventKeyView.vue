<template>
    <div>
        <!-- <input type="search" @keyup="checkEnter($event)" v-model="searchText" /> -->
        <input type="search" @keyup.enter="doSearch" v-model="searchText" />
        <button @click="doSearch">์กฐํ</button>
        <button type="submit" @click.prevent="doSearch">์ ์ก</button>
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