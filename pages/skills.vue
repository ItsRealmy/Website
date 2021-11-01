<template>
  <div>
    <div class="flex h-screen bg-gradient-to-br from-green-400 to-blue-500">
      <div class="m-auto">
        <div
          class="
            p-10
            px-16
            shadow-lg
            content-center
            rounded-md
            bg-white
            max-w-xl
            mx-6
          "
        >
          <h1 class="text-center font-semibold text-3xl">My Skills</h1>

          <div class="grid gap-4 mt-6 h-80 overflow-auto">
            <p>
              <span class="font-semibold">Designing</span>: I love designing
              stuff. From graphic to CSS, I mostly manage to crank out something
              good-looking!
            </p>
            <p>
              <span class="font-semibold">JavaScript</span>: This is the
              language I basically always use, especially with NodeJS.
            </p>
            <p>
              <span class="font-semibold">CSS</span>: Most of the projects I
              make involve CSS, but I'm also trying out some other stuff,
              like...
            </p>
            <p>
              <span class="font-semibold">...Tailwind</span>: This website is
              actually my first Tailwind project!
            </p>
            <p>
              <span class="font-semibold">Vue/Nuxt</span>: This website is also
              written in Nuxt (v2).
            </p>
            <p>
              <span class="font-semibold">Express</span>: I'm very familiar with
              Express.
            </p>
            <p>
              <span class="font-semibold">Python</span>: I don't use Python all
              too often (mainly because it's way more complicated in terms of
              web development (in my opinion)), but I love the indentation-based
              syntax.
            </p>
            <p>
              <span class="font-semibold">Scraping</span>: I know a lot about
              scraping HTML and evading rate limiters.
            </p>
            <p>
              <span class="font-semibold">Affinity Photo</span>: Not everything
              has to be dev-related! I mainly use Affinity Photo to make
              <a
                href="https://reddit.com/r/sbubby"
                class="text-blue-500 hover:underline"
                >Sbubbies</a
              >
              and other fun stuff. Great cheap Photoshop alternative, I highly
              recommend it.
            </p>
            <p>
              <span class="font-semibold">Adobe XD/Figma</span>: Depends on how
              big the project is, but sometimes I use these programs to make
              prototype UI designs or simple logos.
            </p>

            <p>
              <span class="font-semibold">And more</span>: There's more, but I
              don't want to brag too much, since the things you see above are
              the things I'm best at.
            </p>
          </div>

          <div class="flex justify-center mt-8">
            <div class="inline-flex">
              <button class="Default-Button" @click="go(`/`)">Back</button>
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
    },
  },
};
</script>

<style scoped>
button.Default-Button {
  @apply bg-black text-white py-2 px-4 text-sm rounded-md shadow-md mx-auto block ml-2 hover:bg-white hover:text-black;
}
</style>
