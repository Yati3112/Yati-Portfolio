<template>
    <v-row>
        <v-col cols="12">
            <h1 style="color: #5E608C; height: 150px;">Projects</h1>
        </v-col>
    </v-row>
     <v-row>
    <v-col cols="6" v-for="prj in projects" :key="prj.title">
      <v-card>
        <v-card-title>
            {{ prj.title }}
        </v-card-title>
        <v-card-subtitle><a :href=prj.link target="_blank">link</a>
        </v-card-subtitle>
        <v-card-text>
            {{ prj.des }}
        </v-card-text>
      </v-card>

      <div class="text-center text-caption">Using Props Only</div>
    </v-col>
     </v-row>
</template>
<script>
export default({
    data: () => ({
        projects:[
            {
                title: 'BabyStore',
                link:"https://github.com/Yati3112/BabyStore.Vue",
                des:'create a online-shopping proji use Vue.js, Vuetify, Router, Store'
            },
            {
                title: 'Student Record',
                link:  "https://github.com/Yati3112/DataAccessLayerWithSpringBoot",
                des:' create a Student Record  project deeply use mapping concepts with Spring-boot, Jpa, MySQL'
            },
        ]
    })
})
</script>