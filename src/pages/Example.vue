<template>
  <div>
    <h1>Example Page Component</h1>
    {{ pageData }}
    <!-- eslint-disable-next-line vue/require-component-is -->
    <component :is="componentType">
      {{ componentType }}
    </component>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import { ThisTypedComponentOptionsWithRecordProps } from 'vue/types/options'

export default {
  methods: {
    test() {},
  },
  computed: {
    pageData() {
      return Date.now()
    },
    componentType() {
      return this.pageData % 2 ? 'button' : 'p'
    },
  },
} as ThisTypedComponentOptionsWithRecordProps<Vue, {}, {}, {}, {}>
</script>
