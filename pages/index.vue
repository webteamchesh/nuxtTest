<script setup>
// This is the index page, so set the rest of the metadata.
const title = useState("title");
const description = useState("description");

useHead({
  title: title.value,
  meta: [{
    name: 'description',
    content: description.value
  }]
});
</script>

<template>
  <div class="container">
    <div class="row g-0">
      <h1>{{title}}</h1>
      <EntryListing />
    </div>
  </div>
</template>
