<template>
    <h1 style="font-family: Comic Sans MS;">Достопримечательности</h1>
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
                    name: "Бабр",
                    info: "Визитная карточка Иркутска",
                    photo: "https://dostoprimechatelnosti-rus.ru/assets/images/evropa/rossiya1/irkutsk/babr.jpg"
                },
                {
                    id: 1,
                    name: "Остров Юность",
                    info: "Популярное место для отдыха",
                    photo: "https://extraguide.ru/images/pthumb/blog/2021/11-23-27inhp-ostrov-yunost.cd9f7e96.jpg"
                },
                {
                    id: 2,
                    name: "Ледокол «Ангара»",
                    info: "Один из старейших в мире",
                    photo: "http://s3.fotokto.ru/photo/full/282/2829587.jpg"
                },
                {
                    id: 3,
                    name: "Театр Охлопкова",
                    info: "Спектакли разных авторов",
                    photo: "https://extraguide.ru/images/pthumb/blog/2021/03-11-k36fy4-irkutskiy-akademicheskiy-dramaticheskiy-teatr-imeni-np-ohlopkova.cd9f7e96.jpg"
                },
                {
                    id: 4,
                    name: "Галерея Бронштейна",
                    info: "Современное искусство",
                    photo: "https://irkfashion.ru/_stock/texts/part_5/5835/docs/Galereya%20Viktora%20Bronshtejna.jpg"
                },
                {
                    id: 5,
                    name: "Музей истории",
                    info: "Главное здание истории Иркутска",
                    photo: "https://iiaun.ru/images/directions/arctic/nils-9.jpg"
                }
            ]
        }
    }
}
</script>

<style></style>
