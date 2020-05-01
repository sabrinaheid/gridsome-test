<template>
  <div class="container">
    <header class="header">
      <g-link class="title is-size-3" to="/">{{ $static.metaData.siteName }}</g-link>
      <g-link class="subtitle is-size-3" to="/about/">About</g-link>
    </header>
    <slot/>
  </div>
</template>

<static-query>
query {
  metaData {
    siteName
  }
}
</static-query>