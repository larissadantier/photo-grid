<template>
<v-app>
    <div class="pt-10">
    <v-container id="container" >
        <v-avatar
        class="avatar"
        color="primary"
        size="75"
        ></v-avatar>

        <div class="title-text ml-10">
        <h1>Larissa Ruthyle Photo Grid</h1>
        <p>I'am a frontend developer from Rio de Janeiro, Brasil</p>
        </div>  
    </v-container>

    <div class="photo-card">
            <v-row>
                <v-col 
                v-for="n in 12"
                class="d-flex child-flex" 
                cols="4"
                :key="n"
                > 

                    <v-card
                    class="mx-auto"
                    max-width= 100%
                    >

                    <v-img
                    src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                    height="200px"
                    ></v-img>

                    <v-card-title>
                    ❤ Photo
                    </v-card-title>

                    </v-card>
                    
                </v-col>
            </v-row>
        </div>

    <div class="final">
        <h5>My photo grid desenvolvido por <strong>Larissa Ruthyle</strong> | WoMakersCode RJ </h5>
    </div>
 </div>
</v-app>
    

</template>

<script>
export default {
    name:'PhotoGrid',
}

</script>

<style scoped>
    #container{
        display: flex;
        justify-content: center;
    }
    .final{
        display: flex;
        justify-content: center;
    }
    .photo-card{
        padding: 3.5%;
    }
    @media screen and (max-width: 600px){
        .title-text{
            font-size: 0.8em;
        }
        .final{
            font-size: 0.7em;
        }
    }
</style>