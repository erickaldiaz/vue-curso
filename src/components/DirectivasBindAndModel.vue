<template>
    <el-row type="flex" justify="center">
        <el-col :span="6">
            <!-- <img :src="url" : [atributoMisterioso]="atributoMisteriosoValue"> -->
            <h1>{{edad}}</h1>
            <el-input v-model.lazy="edad">
            </el-input>
        </el-col>  
    </el-row>
</template>

<script>
export default {
    data: ()=> ({
        url:"https://pbs.twimg.com/media/EWPJiRLU8AIbuyb.jpg",
        atributoMisterioso: 'alt',
        atributoMisteriosoValue: 'Foto de Bob Esponja',
        edad:''
    }),
    methods: {

    }
}
</script>
