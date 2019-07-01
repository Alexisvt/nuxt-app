<template>
  <h1>A single user, with ID: {{ $route.params.id }}</h1>
</template>

<script>
export default {
  validate(data) {
    return !Object.is(Number(data.params.id), NaN)
  }
}
</script>
