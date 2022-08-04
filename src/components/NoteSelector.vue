<template>
  <div class="note-selector active">
    <p class="note-selector-title">{{ note.body }}:{{ note.id }}</p>
    <p class="note-selector-timestamp">{{ note.timestamp }}</p>
  </div>
</template>

<script>
export default {
  props: ["note"],
};
</script>
