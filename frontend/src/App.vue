<template>
    <v-app>
        <v-navigation-drawer v-model="sideNav">
            <v-list>
                <v-list-tile>
                    <v-list-tile-action>
                        <v-icon>supervisor_account</v-icon>
                    </v-list-tile-action>
                    <v-list-tile-content>login</v-list-tile-content>
                </v-list-tile>
            </v-list>
        </v-navigation-drawer>
        <v-toolbar dark class="primary">
            <v-toolbar-side-icon
                    @click.stop="sideNav = !sideNav"
                    class="hidden-xs-and-up "></v-toolbar-side-icon>
            <v-toolbar-title>Checkers</v-toolbar-title>
            <v-spacer></v-spacer>
            <v-toolbar-items class="hidden-xs-only">
                <v-btn flat>
                    <v-icon left dark>supervisor_account</v-icon>
                    login
                </v-btn>
            </v-toolbar-items>
        </v-toolbar>
        <main>

        </main>
    </v-app>
</template>

<script>
    export default {
        data() {
            return {
                sideNav: false,

            }
        }
    }
</script>

<style lang="stylus">
    @import '../node_modules/vuetify/src/stylus/main.styl'

</style>
