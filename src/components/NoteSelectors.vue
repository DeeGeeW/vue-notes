<template>
  <div class="note-selectors">
    <NoteSelector v-for="note in notes" v-bind:key="note.id" v-bind:note="note" />
  </div>
</template>

<script>
import NoteSelector from "./NoteSelector.vue";

export default {
  components: {
    NoteSelector,
  },
  data: function () {
    return {
      notes: [
        { id: 1, body: "This is a first test", timestamp: Date.now() },
        { id: 2, body: "This is a second test", timestamp: Date.now() },
        { id: 3, body: "This is a third test", timestamp: Date.now() },
        { id: 4, body: "This is a fourth test", timestamp: Date.now() },
      ],
    };
  },
};
</script>
