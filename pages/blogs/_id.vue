<template>
  <section>Blog {{}}</section>
</template>

<script>
export default {
  validate({params}) {
    return /^\d+$/.test(params.id)
  }
}
</script>