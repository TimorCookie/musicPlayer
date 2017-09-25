<template>
  <div class="singer" ref="singer">
  </div>  
</template>
<script>
import {getSingerList} from 'api/singer'
import {ERR_OK} from 'api/config'
export default {
  data() {
    return {
      singers: []
    }
  },
  methods: {
    _getSingerList() {
      getSingerList().then(res => {
        if (res.code === ERR_OK) {
          console.log(res.data.list)
        }
      })
    }
  },
  mounted() {
    this._getSingerList()
  }
}
</script>
<style lang="scss">

</style>