<template>
    <div class="home">
        <PageTitle icon="fa fa-home" main="Dashboard"
            sub="Teste" />
        <div class="stats">
            <Stat title="Categorias" :value="stat.categories"
                icon="fa fa-folder" color="#F44336" />
            <Stat title="Artigos" :value="stat.articles"
                icon="fa fa-file" color="#4CAF50" />
            <Stat title="Usuários" :value="stat.users"
                icon="fa fa-user" color="#2196F3" />
        </div>
    </div>
</template>

<script>
import PageTitle from '../template/PageTitle'
import Stat from './Stat'
import axios from 'axios'
import { baseApiUrl } from '@/global'

export default {
    name: 'Home',
    components: { PageTitle, Stat },
    data: function() {
        return {
            stat: {}
        }
    },
    methods: {
        getStats() {
            axios.get(`${baseApiUrl}/stats`).then(res => this.stat = res.data)
        }
    },
    mounted() {
        this.getStats()
    }
}
</script>

<style>
    .stats {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
    }
    .fa-home {
        color: #3F51B5 !important;
    }
</style>
