<template>
    <v-container
        fluid
        class="ma-0 pa-0"

    >
            <v-parallax
                dark
                src="/img/heroImage.jpg"
                height=1000
                
            >
                <v-row
                align="center"
                justify="center"
                >
                <v-col
                    class="text-center"
                    cols="12"
                >
                    <h1 class="text-h1 font-weight-bold mb-4">
                    Always Drive Loaded
                    </h1>
                    <h4 class="text-h4 heroSubheading mb-6">
                        Market leader in tools for technology for moving companies to provide estimates, collect payments and get leads.                    
                    </h4>
                    <v-btn
                    elevation="3"
                    x-large
                    light
                    >Get A Free Demo</v-btn>
                </v-col>
                </v-row>
            </v-parallax>
    </v-container>
</template>
<script>
export default {
    name: "AppHero"
}
</script>

<style scoped>
.heroSubheading {
    max-width: 800px;
    margin: 0 auto;
}

</style>