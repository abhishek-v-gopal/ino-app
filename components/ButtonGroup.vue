<template>
    <div class="flex flex-wrap justify-center gap-2 p-4">
      <button
        v-for="(button, index) in buttons"
        :key="index"
        @click="toggleButton(index)"
        :class="[
          'px-4 py-2 rounded-full text-sm font-medium transition-colors',
          selectedIndices.includes(index)
            ? 'bg-blue-200 text-blue-800'
            : 'bg-gray-200 text-gray-800 hover:bg-gray-300',
          { 'opacity-50 cursor-not-allowed': selectedIndices.length >= 3 && !selectedIndices.includes(index) }
        ]"
        :disabled="selectedIndices.length >= 5 && !selectedIndices.includes(index)"
      >
        {{ button }}
      </button>
    </div>
    <!-- <p v-if="selectedIndices.length === 0" class="text-red-500 text-center mt-2">
      Please select at least one skill.
    </p> -->
    <!-- <p v-if="selectedIndices.length >= 4" class="text-blue-500 text-center mt-2">
      Maximum number of skills selected.
    </p> -->
  </template>
  
  <script>
  export default {
    data() {
      return {
        buttons: [
          'PROGRAMMING',
          'TECHNOLOGY',
          'ARTS',
          'ENTREPRENEURSHIP',
          'CREATIVE DESIGNER'
        ],
        selectedIndices: []
      }
    },
    methods: {
      toggleButton(index) {
        if (this.selectedIndices.includes(index)) {
          // If already selected, remove it
          this.selectedIndices = this.selectedIndices.filter(i => i !== index);
        } else if (this.selectedIndices.length < 3) {
          // If not selected and less than 5 are selected, add it
          this.selectedIndices.push(index);
        }
      }
    }
  }
  </script>