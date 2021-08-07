<template>
    <div>
        <v-row class="d-flex flex-row justify-center align-center">
            <v-button color="accent" fab>
                <v-icon v-for="button in buttons" :key="button" class="mx-2">
                    {{button.icon}}
                </v-icon>
            </v-button>
        </v-row>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                buttons: [
                    {icon: 'mdi-restart'},
                    {icon: 'mdi-pause'},
                    {icon: 'mdi-close'}
                    ]
            }
        },
   }
</script>