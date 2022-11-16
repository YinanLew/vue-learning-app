<template>
  <li>
    <base-card>
      <header>
        <h3>{{ res.title }}</h3>
        <base-button mode="flat" @click="removeResource(res.id)"
          >Delete</base-button
        >
      </header>
      <p>{{ res.description }}</p>
      <nav>
        <a :href="res.link">View Resource</a>
      </nav>
    </base-card>
  </li>
</template>

<script>
export default {
  props: ["res"],
  inject: ["removeResource"],
};
</script>

<style scoped>
li {
  margin: auto;
  max-width: 40rem;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

a {
  text-decoration: none;
}
</style>
