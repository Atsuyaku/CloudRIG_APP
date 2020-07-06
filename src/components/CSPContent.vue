<template>
    <v-container fill-height class="CSPContent">
        <v-layout column pa-10>
            <v-row no-gutters>
                <v-col offset="5">
                    <div
                            class="font-weight-black white--text" style="font-size: xx-large; margin-bottom: 70px;"
                    >
                        Cloud Provider
                    </div>
                </v-col>
            </v-row>

            <v-row>
                <v-col cols="2">
                    <router-link tag="span" to="/">
                        <v-btn dark
                               depressed
                               class="white"
                               style=" background-color:transparent; border: dashed"
                               height="170px"
                               width="170px"
                        >

                                <img src="../assets/awslogo.png" height="100px;"width="100px;">

                        </v-btn>
                    </router-link>
                </v-col>

                <v-col cols="2">
                    <router-link tag="span" to="/">
                        <v-btn dark
                               depressed
                               style=" background-color:transparent; border: dashed"
                               height="170px"
                               width="170px"
                               class="white"

                        >
                            <v-icon color="white" size="150">

                            </v-icon>
                        </v-btn>
                    </router-link>
                </v-col>

                <v-col cols="2">
                    <router-link tag="span" to="/">
                        <v-btn dark
                               depressed
                               style=" background-color:transparent; border: dashed"
                               height="170px"
                               width="170px"
                               class="white"

                        >
                            <v-icon color="white" size="150">

                            </v-icon>
                        </v-btn>
                    </router-link>
                </v-col>

                <v-col cols="2">
                    <router-link tag="span" to="/">
                        <v-btn dark
                               depressed
                               style=" background-color:transparent; border: dashed"
                               height="170px"
                               width="170px"
                               class="white"

                        >
                            <v-icon color="white" size="150">

                            </v-icon>
                        </v-btn>
                    </router-link>
                </v-col>
            </v-row>
        </v-layout>
    </v-container>
</template>

<script>
    export default {
        name: "CSPContent"
    }
</script>

<style scoped>

</style>