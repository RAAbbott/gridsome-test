<template>
  <div>
    <header class="flex flex-row justify-between items-center h-20 px-48 text-black">
      <strong class="text-2xl">
        <g-link to="/">{{ $static.metadata.siteName }}</g-link>
      </strong>
      <nav>
        <span class="font-semibold mx-2 text-lg transform transition-all ease-in-out duration-500 hover:text-xl cursor-pointer">1-800-325-4516</span>
        <g-link class="nav__link px-6 py-4 font-semibold bg-blue-400 text-white rounded-lg capitalize" to="/quote/">REQUEST A QUOTE</g-link>
      </nav>
    </header>
    <div class="w-full m-auto overflow-y-scroll pb-48">
      <slot/>
    </div>
    <footer class="h-48 bg-black w-full text-white">
      FOOTER
    </footer>
  </div>
</template>


<script>
export default {
  data() {
    return {

    }
  },

  mounted() {
    console.log('MOUNTED')
  }
}
</script>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>
body {
  font-family: -apple-system,system-ui,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
  margin:0;
  padding:0;
  line-height: 1.5;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
}

.nav__link {
  margin-left: 20px;
}
</style>
