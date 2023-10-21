<template>
    <tr v-for="(v, k) in rowData">
      <!-- product -->
      <TableCell :value="v.Product" />
      
      <!-- Lithography -->
      <TableCell :value="v.Lithography" />
      
      <!-- Threads -->
      <TableCell :value="v.Threads" :input="true" />
  
      <!-- Base Freq -->
      <TableCell :value="v.Base_Freq" :input="true" />
  
      <!-- Max Turbo Freq -->
      <TableCell :value="v.Max_Turbo_Freq" :input="true" />
    </tr>
</template>
  
<script>
  import TableCell from './TableCell.vue';
  
  export default {
    components: {
      TableCell
    },
    props: {
      rowData: {
        type: Object,
        required: true
      }
    }
  };
</script>
  