<template>
  <div id="app">
    <Layout>
      <router-view />
    </Layout>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>