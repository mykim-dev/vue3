<template>
    <div>
        <!-- <select v-on:change="changeCity" v-model="selectedCity"> -->
        <select @change="changeCity($event)" v-model="selectedCity">
            <option>-- 도시선택 --</option>
            <option 
            :key="city.cityCode" 
            :value="city.cityCode" 
            v-for="city in cityList">
            {{ city.cityTitle }}
        </option>
        </select>
        <select>
            <option>-- 동선택 --</option>
            <option 
            :key="dong.dongCode" 
            :value="dong.dongCode"
             v-for="dong in selectDongList">
             {{ dong.dongTitle }}
            </option>
        </select>
    </div>
</template>

<script>
export default{ 
    name:'',
    components:{},
    data(){
        return{
            selectedCity: '',
            cityList: [
                { cityCode: '02', cityTitle: '서울'},
                { cityCode: '051', cityTitle: '부산'},
                { cityCode: '064', cityTitle: '제주'},
            ],
            dongList: [
                { cityCode: '02', dongCode: '1',  dongTitle: '서울 1동' },
                { cityCode: '02', dongCode: '2',  dongTitle: '서울 2동' },
                { cityCode: '02', dongCode: '3',  dongTitle: '서울 3동' },
                { cityCode: '02', dongCode: '4',  dongTitle: '서울 4동' },
                { cityCode: '051', dongCode: '1',  dongTitle: '부산 1동' },
                { cityCode: '051', dongCode: '2',  dongTitle: '부산 2동' },
                { cityCode: '051', dongCode: '3',  dongTitle: '부산 3동' },
                { cityCode: '064', dongCode: '1',  dongTitle: '제주 1동' },
                { cityCode: '064', dongCode: '2',  dongTitle: '제주 2동' },
            ],
            selectDongList: []
        }
    },
    setup(){},
    created(){},
    mounted(){},
    unmounted(){},
    methods:{
        changeCity(event) {
            console.log(event.target.tagName);
            this.selectDongList = this.dongList.filter(dong => dong.cityCode === this.selectedCity)
        }
    }
}
</script>