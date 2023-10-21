<template>
    <td v-if="!input">{{ value }}</td>
    <td v-else>
      <div class="innerCells">
        <input :value="value" :disabled="true" type="text" />
      </div>
    </td>
</template>
  
<script>
  export default {
    props: {
      value: {
        required: true
      },
      input: {
        type: Boolean,
        default: false
      }
    }
  };
</script>
  