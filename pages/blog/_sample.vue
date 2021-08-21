<template>
  <div>
    <h2>サンプルページです</h2>
    <p>これは{{ $route.params.sample }}のエントリーです</p>
  </div>
</template>

<script>
export default {
  validate({ params }) {
    return /^\d+$/.test(params.sample)
  }
}
</script>
