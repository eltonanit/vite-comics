<script>
import comics from './data/dc-comics.json';

export default {
    data() {
        return {
            comics
        }
    }
}
</script>

<template>
    <div class="bg-cartoon">
        <span class="badge text-bg-primary rounded-0 px-3 py-2">
            <h3>CURRENT SERIES</h3>
        </span>
    </div>
    <div>
        <div class="wrap bg-dark">
            <div class="container">
                <div class="row">
                    <div class="col-12 p-4 d-flex flex-wrap justify-content-center">
                        <div v-for="(comic, index) in comics" :key="index" class="col-6 col-md-4 col-lg-2 mb-4 d-flex">
                            <div class="card border-0 bg-transparent w-100 mx-3">
                                <img :src="comic.thumb" :alt="comic.series" class="card-img-top img-fluid">
                                <h5 class="text-white text-center pt-2">{{ comic.series }}</h5>
                            </div>
                        </div>
                    </div>
                </div>
                <div>
                    <button class="btn btn-primary rounded-0 px-5">LOAD MORE</button>
                </div>
            </div>
        </div>
    </div>
     
</template>



<style lang="scss" scoped>
.content-area {
    background-color: #222;
    color: #fff;
    font-weight: 600;
    padding: 20px;
}
</style>