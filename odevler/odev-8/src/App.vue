<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12">
                <br>
                <button class="btn btn-primary">Mavi Temayı Yükle</button>
                <button class="btn btn-success">Yeşil Temayı Yükle</button>
                <button class="btn btn-danger">Kırmızı Temayı Yükle </button>
                <hr>
                <app-blue></app-blue>
                <app-green></app-green>
                <app-red></app-red>
            </div>
        </div>
    </div>
</template>

<script>
    import Blue from './components/Blue.vue';
    import Green from './components/Green.vue';
    import Red from './components/Red.vue';

    export default {
        components: {
            appBlue: Blue,
            appGreen: Green,
            appRed: Red
        }
    }
</script>

<style>
</style>
