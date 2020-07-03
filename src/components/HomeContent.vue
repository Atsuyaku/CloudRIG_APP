<template>
    <v-container fill-height class="home-content">
        <v-layout justify-center align-center column pa-10>
            <v-row no-gutters align="center">
                <v-col>
                    <div
                        class="display-4 font-weight-black white--text text-center "
                    >
                         My Computers
                    </div>
                </v-col>
            </v-row>


            <v-row>
                <v-col>
                    <v-btn dark
                           depressed
                       style=" background-color:transparent;"
                       class="white"
                    >
                        <v-icon large color="white">
                            far fa-plus-square
                        </v-icon>
                    </v-btn>
                </v-col>
            </v-row>
        </v-layout>
    </v-container>
</template>

<script>
export default {
    name: 'HomeContent'
};
</script>

<style scoped>
.v-btn {
    text-indent: initial;
    text-transform: none;
}
</style>
