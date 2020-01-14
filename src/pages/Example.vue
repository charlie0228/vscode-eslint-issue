<template>
  <div>
    <h1>Example Page Component</h1>
    {{ pageData }}
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import { ThisTypedComponentOptionsWithRecordProps } from 'vue/types/options'

export default {
  methods: {
    test() {

    }
  },
  computed: {
    pageData() {
      return Date.now()
    }
  }
} as ThisTypedComponentOptionsWithRecordProps<Vue, {}, {}, {}, {}>
</script>
