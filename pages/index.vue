<template>
  <div>
    <div class="flex h-screen bg-gradient-to-br from-green-400 to-blue-500">
      <div class="m-auto">
        <div class="p-10 px-16 shadow-lg content-center rounded-md bg-white mx-6">
          <h1 class="text-center font-semibold text-2xl">Hey, I'm Realmy!</h1>
          <p class="text-center mt-4">
            Your average, Dutch 15-year-old web developer.
          </p>

          <div class="flex justify-center mt-8">
            <div class="inline-flex">
              <button class="Default-Button" @click="go(`/skills`)">My Skills</button>

              <a href="https://discord.gg/UfvcuKUThh"><button class="Default-Button">Discord Server</button></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    go(page) {
      this.$router.push(page);
    }
  }
};
</script>

<style scoped>
button.Default-Button {
  @apply bg-black text-white py-2 px-4 text-sm rounded-md shadow-md mx-auto block ml-2 hover:bg-white hover:text-black;
}
</style>
