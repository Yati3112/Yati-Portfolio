<template>
    <v-row>
        <v-col cols="12">
            <h1 style="color: #5E608C;">Experience</h1>
        </v-col>
    </v-row>
    <v-row>
        <v-col cols="12" v-for="jobs in jobs" :key="jobs.companyName">
            <OverAllExperience :work=jobs></OverAllExperience>
        </v-col>
    </v-row>
</template>
<script>
import OverAllExperience from './OverAllExperience.vue';


export default({
    name:'WorkExperience',
    components:{OverAllExperience},
    data: () => ({
        jobs:[
            {
                position:"AAA( )",
                companyName:"AAA",
                des:["A job description in English is a formal document outlining the responsibilities, duties, necessary qualifications, and skills for a specific role within an organization."," It typically includes the job title, a summary of the position's purpose, key responsibilities, required experience and education, and information about the company and its benefits. The goal is to provide clear information for potential candidates to assess their fit and for the employer to attract the right talent."]
            },
            {
                position:"AAA( )",
                companyName:"AAA",
                des:["A job description in English is a formal document outlining the responsibilities, duties, necessary qualifications, and skills for a specific role within an organization."," It typically includes the job title, a summary of the position's purpose, key responsibilities, required experience and education, and information about the company and its benefits. The goal is to provide clear information for potential candidates to assess their fit and for the employer to attract the right talent."]
            },
            {
                position:"AAA( )",
                companyName:"AAA",
                des:["A job description in English is a formal document outlining the responsibilities, duties, necessary qualifications, and skills for a specific role within an organization."," It typically includes the job title, a summary of the position's purpose, key responsibilities, required experience and education, and information about the company and its benefits. The goal is to provide clear information for potential candidates to assess their fit and for the employer to attract the right talent."]
            },
            {
                position:"AAA( )",
                companyName:"AAA",
                des:["A job description in English is a formal document outlining the responsibilities, duties, necessary qualifications, and skills for a specific role within an organization."," It typically includes the job title, a summary of the position's purpose, key responsibilities, required experience and education, and information about the company and its benefits. The goal is to provide clear information for potential candidates to assess their fit and for the employer to attract the right talent."]
            },
        ]
        
    }),
})
</script>