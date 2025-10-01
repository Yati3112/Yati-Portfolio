<template>
  <v-container>
    <v-row>
      <v-col cols="4">
         <PersonalInformation/>
      </v-col>
      <v-col cols="8"><div id="about-section">
         <AboutView/></div>
         <v-divider class="my-8"></v-divider>
         <div id="experience-section"> <WorkExperience/> </div>  
         <v-divider class="my-8"> </v-divider>
          <div id="projects-section">   <ProjectLists/> </div>
        
      </v-col>
    </v-row>
  </v-container>


</template>

<script>
import { defineComponent } from 'vue';

// Components
import PersonalInformation from '@/components/PersonalInformation.vue';
import AboutView from './AboutView.vue';
import WorkExperience from '@/components/WorkExperience.vue';
import ProjectLists from '@/components/ProjectLists.vue';
export default defineComponent({
  name: 'HomeView',

  components: {
    AboutView,
    PersonalInformation,
    WorkExperience,
    ProjectLists
  },
});
</script>
