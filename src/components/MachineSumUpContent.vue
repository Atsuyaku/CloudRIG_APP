<template>
    <div style="padding-left: 56px;">
        <v-app
                id="inspire"
                style="padding: 40px; background-color: transparent; height: 400px "

        >
            <div
                    class="font-weight-black white--text"
                    style="font-size: xx-large; margin-bottom: 20px;"
            >
                Summary
            </div>
            <v-row>
                <v-col cols="6">
                    <v-col>
                        <v-row no-gutters>
                            <v-col md="5">
                                <div>
                                    <div>
                                        <v-row>
                                        <v-col style="text-decoration: underline;">Machine name: </v-col>
                                        <v-col>Machine001</v-col>
                                        </v-row>
                                    </div>
                                    <div>
                                        <v-row>
                                            <v-col style="text-decoration: underline;">Region: </v-col>
                                            <v-col>EUROPE WEST</v-col>
                                        </v-row>
                                    </div>
                                </div>
                            </v-col>
                            <v-col cols="1" align="center" ><v-divider class="mx-0" vertical dark></v-divider></v-col>

                            <v-col cols="5">
                                <div>
                                    <div>
                                        <v-row>
                                            <v-col style="text-decoration: underline;">Cloud Provider: </v-col>
                                            <v-col>AWS</v-col>
                                        </v-row>
                                    </div>
                                    <div>
                                        <v-row>
                                            <v-col style="text-decoration: underline;">Access Key Id: </v-col>
                                            <v-col>AKIAJSIE27KKMHXI3BJQ</v-col>
                                        </v-row>
                                    </div>
                                </div>
                            </v-col>

                        </v-row>
                        <v-row>

                            <v-col>
                                <router-link tag="span" to="/Credentials">
                                    <v-btn dark style="margin-top: 30px; margin-left: 20px;">Previous</v-btn>
                                </router-link>

                                <router-link tag="span" to="/MachineSumUp" style=" margin-left: 31%;">
                                    <v-btn style="margin-top: 30px;">CREATE</v-btn>
                                </router-link>
                            </v-col>

                        </v-row>
                    </v-col>
                </v-col>

            </v-row>
            <v-row></v-row>
            <v-row></v-row>
            <v-row></v-row>
            <v-row></v-row>
            <v-row></v-row>
            <v-row></v-row>
            <v-row></v-row>
            <v-row></v-row>
            <v-row></v-row>

        </v-app>
    </div>
</template>

<script>
    export default {
        name: "MachineSumUpContent"
    }
</script>

<style scoped>

</style>