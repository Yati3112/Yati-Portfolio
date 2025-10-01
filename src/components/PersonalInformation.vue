<template>
    <v-row>
        <v-col cols="12" style="color: #111226; font-family: 'Times New Roman', Times, serif; font-size: 300%;">
            YATI PHOO
        </v-col>
    </v-row>
    
       <v-table striped="even" style="background-color: #9C9BBF; font-family: 'Times New Roman', Times, serif;">
    <tbody>
      <tr
        v-for="information in inf"
        :key="information.text"
      >
        <td> <v-icon style="color: #012840; font-size: 80%;">{{ information.icon }}</v-icon> &nbsp;&nbsp;{{ information.text }}</td>
      </tr>
    </tbody>
  </v-table>
    <v-row>
        <v-col cols="12">
        <v-card
    class="mx-auto my-16"
    max-width="400"
  >
    <v-img
      class="align-end text-white"
      height="200"
        :src="require('../assets/yati.jpg')"
      cover
    ></v-img>
   </v-card>
   </v-col>
    </v-row>
    <v-row>
        <v-col cols="12">
            <v-breadcrumbs :items="items"></v-breadcrumbs>
        </v-col>
    </v-row>
</template>
<script>
export default({
    name:'PersonalInformation',
    data: () => ({
        inf:[
            {
            icon:'mdi-phone-in-talk',
            text:'(+66)814690681'
            },
            {
            icon:'mdi-phone-in-talk',
            text:'yatiphoo1996@gmail.com'
            },
            {
            icon:'mdi-phone-in-talk',
            text:'github.com.yati3112'
            },
            {
            icon:'mdi-phone-in-talk',
            text:'https://www.linkedin.com/in/yati-phoo-32a19624b'
            },
            {
            icon:'mdi-phone-in-talk',
            text:'227/13 Rama I Rd, Khwaeng Rong Muang, Pathum Wan, Krung Thep Maha Nakhon 10330'
            }
            
        ],
        items:[
          {
          title:'About',
          disabled:false,
          href:'#about-section'
        },
        {
          title:'Experience',
          disabled:false,
          href:'#experience-section'
        },
        {
          title:'Project',
          disabled:false,
          href:'#projects-section'
        },

        ]
    })
})
</script>