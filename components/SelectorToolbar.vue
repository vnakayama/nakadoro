<template>
    <div>
        <v-row class="d-flx flex-row justify-end align-center">
            <v-btn color="accent" fab>
                <v-icon>
                    mdi-white-balance-sunny
                </v-icon>
            </v-btn>
        </v-row>
    </div>
</template>

<script>
    export default {
        data () {
            return {
                themes: {
                    light: {
                        icon: 'mdi-white-balance-sunny'
                        
                    }
                }
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>