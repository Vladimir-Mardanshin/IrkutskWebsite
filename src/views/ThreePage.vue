<template>
    <h1 style="font-family: Comic Sans MS;">Еда</h1>
    <v-container style="margin-bottom: 70px;">
        <v-row class="list__cafes-content">
            <MapPlace v-for="place in places" :key="place.id" :place="place"></MapPlace>
        </v-row>
    </v-container>
</template>
   
<script>
import MapPlace from '../components/MapPlace.vue';
export default {
    components: {
        MapPlace
    },
    data() {
        return {
            places: [
                {
                    id: 0,
                    name: "Охотников",
                    info: "Истинная кухня Сибири",
                    photo: "https://mykaleidoscope.ru/uploads/posts/2020-03/1583352524_25-p-frantsuzskie-deserti-visokoi-kukhni-57.jpg"
                },
                {
                    id: 1,
                    name: "Европа",
                    info: "Ресторан высокой кухни",
                    photo: "https://mykaleidoscope.ru/x/uploads/posts/2022-09/1663757793_19-mykaleidoscope-ru-p-mishlenovskie-blyuda-yeda-pinterest-19.jpg"
                },
                {
                    id: 2,
                    name: "Стрижи",
                    info: "Блюда для всех",
                    photo: "https://sobraniespeshilov.com/wp-content/uploads/2019/02/1-1.jpg"
                }
            ]
        }
    }
}
</script>
   
<style></style>
   