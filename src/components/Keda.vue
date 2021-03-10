<template>
<div>
  <h2><center>Keda Test, 03 March 2021 </center></h2>
  <v-container    >
   <h4>Number 1 </h4>
    <v-radio-group v-model="radioGroup">
      <v-radio
        v-for="n in 3"
        :key="n"
        :label="`Radio ${n}`"
        :value="n"
      ></v-radio>
    </v-radio-group>
  </v-container>

   <v-container >  
   <h4>Number 2 </h4>
    <v-date-picker
      v-model="picker"
      flat
    ></v-date-picker>
   </v-container>


   <v-layout row wrap>
    <v-datetime-picker
      label="From Date"
      v-model="fromDate"
      format="DD/MM/YYYY"
    ></v-datetime-picker>
  </v-layout>
</div>


</template>

