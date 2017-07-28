<template>
  <div>
    <p ref="name">姓名：{{user.name}}</p>
    <p>年龄：{{user.age}}</p>
    <!-- <ul>
      <li v-for="item in list" :key="item.id">
        <span>{{item.name}}</span>
        <span>{{item.age}}</span>
        <span>{{item.hobby}}</span>
      </li>
    </ul> -->
    <!-- <m-header></m-header> -->
  </div>  
</template>
<script>
// import MHeader from 'components/m-header/m-header'
export default {
  components: {
    // MHeader
  },
  data() {
    return {
      user: {},
      list: []
    }
  },
  created() {
    const data = {
      name: 'Timokie',
      age: 18
    }
    this.$data.user = data
    const dataList = [{
      id: 1,
      name: '宗元',
      age: 30,
      hobby: '王者荣耀'
    }, {
      id: 2,
      name: '章磊',
      age: 32,
      hobby: '打麻将'
    }, {
      id: 3,
      name: '陈小静',
      age: 33,
      hobby: '送人头'
    }]
    this.list = dataList
    // let dom = this.$refs.name
    // console.log(dom)
  },
  mounted() {
    // let dom = this.$refs.name
    // console.log(dom)
  }
}
</script>
<style lang="scss">

</style>

