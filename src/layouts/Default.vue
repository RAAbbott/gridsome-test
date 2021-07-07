<template>
  <div>
    <header class="flex flex-row justify-between items-center h-28 px-24 text-black">
      <strong class="text-2xl">
        <g-link to="/">{{ $static.metadata.siteName }}</g-link>
        <span class="font-semibold ml-16 text-base relative"><span class="material-icons absolute bottom-0 -left-7">call</span>1-800-325-4516</span>
      </strong>
      <nav>
        <g-link class="nav__link mr-4 font-semibold text-gray-700" to="/quote/">SERVICES</g-link>
        <g-link class="nav__link mr-6 font-semibold text-gray-700" to="/quote/">LOCATIONS</g-link>
        <g-link class="nav__link mr-8 px-6 py-4 font-semibold bg-blue-400 text-white rounded-lg relative" to="/quote/">CHAT WITH US <span class="absolute -bottom-5 left-0 text-gray-400 text-xs">*No appointment needed</span></g-link>
      </nav>
    </header>
    <div class="w-full overflow-y-scroll pb-48">
      <slot/>
    </div>
    <footer class="h-64 bg-black w-full text-white">
      FOOTER
    </footer>
  </div>
</template>

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
