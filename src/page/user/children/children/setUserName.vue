<template>
  <div class="page">
    <mu-appbar title="修改用户名">
          <mu-icon-button icon="chevron_left" slot="left" @click="goBack"/>
    </mu-appbar>
    <mu-content-block>
      <mu-list>
        <mu-list-item>
          <mu-text-field hintText="输入用户名" maxLength="8" fullWidth/><br/>
        </mu-list-item>
        <mu-list-item>
          <mu-raised-button label="确认修改" fullWidth class="demo-raised-button" color="#e91e63"/>
        </mu-list-item>
      </mu-list>        
    </mu-content-block>
  </div>
</template>

<script>
export default{
  name: 'setUserName',
  data () {
    return {

    }
  },
  methods: {
    goBack(){
      this.$router.go(-1);
    }
  }
}
</script>

<style>
.page{
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: 2050;
  background-color: #fff;
}
</style>
