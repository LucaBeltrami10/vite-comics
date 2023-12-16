<template>
    <main>
        <div class="jumbotron"></div>
        <div class="container">
            <div class="stiker">
                <p>current series</p>
            </div>
            <div class="card-container">
                <CardMainSection v-for="card in cardList" :imageSrc="card.thumb" :descriptionImage="card.series"
                    :title="card.series" />
            </div>
            <button>load more</button>
        </div>
    </main>
</template>

<script>
import CardMainSection from './CardMainSection.vue';
export default {
    name: 'AppMain',
    components: {
        CardMainSection,
    },
    data() {
        return {
            cardList: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book",
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book",
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel",
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel",
                },
            ],
        }

    },
    methods: {

    },
}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

main {
    background-color: $main-background;

    div.jumbotron {
        height: 280px;
        width: 100%;
        background-image: url(../assets/img/jumbotron.jpg);
        background-position: top;
        background-repeat: no-repeat;
        background-size: 100%;
    }

    div.container {
        position: relative;

        div.stiker {
            @include flex(row, center, center);
            background-color: $stiker-and-button-main;
            width: 160px;
            padding: 0.5rem 0;
            position: absolute;
            left: 0;
            top: 0;
            transform: translate(0px, -50%);


            p {
                color: white;
                text-transform: uppercase;
                font-weight: 800;
            }
        }

        div.card-container {
            width: 100%;
            @include flex(row, space-between, start);
            flex-wrap: wrap;
            padding-bottom: 40px;

            div.card {
                height: 140px;
                width: calc((100% / 6) - 16px);
                background-color: magenta;
                margin: 35px 8px 0 8px
            }

        }

        button {
            background-color: $stiker-and-button-main;
            border: none;
            text-transform: uppercase;
            color: white;
            padding: 0.5rem 1.5rem;
            margin-left: 50%;
            margin-bottom: 10px;
            transform: translate(-50%, 0px);
            font-size: 0.6rem;
            font-weight: 800;
        }
    }
}
</style>