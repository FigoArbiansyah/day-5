<template>
  <main class="bg-gradient-to-tr from-white to-blue-100 min-h-screen">
    <Navbar />
    <section class="min-h-screen flex justify-center items-center max-md:px-4">
      <div class="text-center">
        <div class="md:text-4xl text-2xl font-bold">
          <h1>Get Connected to the Best Remote</h1>
          <br />
          <h1 class="-mt-8">Jobs in Your Field</h1>
        </div>
        <p class="text-slate-600 mt-6 md:text-lg">
          Discover a wide range of remote opportunities on our platform take
          control of your career
        </p>
        <div
          class="flex max-md:flex-col max-md:gap-y-8 gap-x-8 mt-7 justify-center"
        >
          <div>
            <a
              href="#"
              class="px-5 py-3 rounded-full bg-blue-700 text-white shadow-lg shadow-blue-200 hover:shadow-none transition-all ease duration-300"
              >Explore Remote Jobs</a
            >
          </div>
          <div>
            <a
              href="#"
              class="px-5 py-3 rounded-full text-blue-700 underline font-semibold"
              >How it works?</a
            >
          </div>
        </div>
      </div>
    </section>
    <div class="md:px-24 px-3 mb-3">
      <p class="text-lg font-semibold">Featured Jobs</p>
    </div>
    <section
      class="md:px-24 px-3 flex justify-center max-md:flex-col items-center gap-x-4 pb-20"
    >
      <Card
        img="~/assets/figma.png"
        judul="Front End Developer"
        tech="Figma"
        deskripsi="We are looking for an experienced front-end developer to join our team."
        lang="Rust"
        gaji="$70,000 - $90,000"
      >
        <img
          src="~/assets/figma.png"
          class="object-cover w-full h-full"
          alt=""
        />
      </Card>
      <Card
        judul="Data Scientist"
        tech="Facebook"
        deskripsi="We are seeking a data scientist to join our team."
        lang="Python"
        gaji="$100,000 - $130,000"
      >
        <img
          src="~/assets/facebook.png"
          class="object-cover w-full h-full"
          alt=""
        />
      </Card>
      <Card
        judul="Technical Writter"
        tech="Github"
        deskripsi="We are seeking a technical writter to join our team."
        lang="Documentation"
        gaji="$60,000 - $80,000"
      >
        <img
          src="~/assets/github.png"
          class="object-cover w-full h-full"
          alt=""
        />
      </Card>
    </section>
    <Footer />
  </main>
</template>

<script>
export default {
  data() {
    return {
      layouts: {
        navbar: "navbar-main",
      },
    };
  },
};
</script>
