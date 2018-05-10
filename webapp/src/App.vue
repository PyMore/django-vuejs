<template>
  <div id="app">
    <Toobal/>
  </div>
</template>

<script>
import SignIn from './components/SignIn'
import Flex from './components/Flex'
import Grib from './components/Grib'
import Toobal from './components/Toolbar'

export default {
  name: 'App',
  components: {
    SignIn,
    Flex,
    Grib,
    Toobal,
  }
}
</script>

<style>
</style>
