<template>
  <div>
    <h1>Example Page Component</h1>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import { ThisTypedComponentOptionsWithRecordProps } from 'vue/types/options'

export default {
  computed: {
    pageData() {
      return Date.now()
    }
  }
} as ThisTypedComponentOptionsWithRecordProps<Vue, {}, {}, {}, {}>
</script>
