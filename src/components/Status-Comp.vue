<template>
  <div class="container" v-for="item in users" :key="item.id">
    <div class="row justify-content-center">
      <div class="col-lg-6 col-sm-12">
        <div class="row">
          <div class="col-1">
            <img src="../assets/img-1.png" alt="" class="img-profile" />
          </div>
          <div class="col-11">
            <strong>{{ item.name }}</strong> @{{ item.username }} · {{ item.date }} <br />
            <div class="status">
             {{ item.status }}
            </div>
            <ul class="nav mt-3 justify-content-between">
              <li class="nav-item px-3">
                <img src="../assets/ic-comment.png" alt="" class="icon" />
                <span class="px-2">{{ item.comments }}</span>
              </li>
              <li class="nav-item px-3">
                <img src="../assets/ic-start.png" alt="" class="icon" />
                <span class="px-2">{{ item.stars }}</span>
              </li>
              <li class="nav-item px-3">
                <img src="../assets/ic-share.png" alt="" class="icon" />
                <span class="px-2">{{ item.shares }}</span>
              </li>
              <li class="nav-item px-3">
                <img src="../assets/ic-save.png" alt="" class="icon" />
              </li>
            </ul>
            <hr />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import users from '../Mock/users.json';

export default {
  name: "StatusComp",
  data(){
    return {
      images:[
        {no: 1, url: "../assets/img-1.png"},
        {no: 2, url: "../assets/img-2.png"},
        {no: 3, url: "../assets/img-3.png"},
      ],
      users,
    };
  }
};
</script>

<style lang="scss">

.status {
  margin-top: 10px;
  margin-bottom: 20px;
  font-size: 22px;
}
.img-status {
  margin-top: 20px;
}
.img-profile {
  width: 50px;
}
.icon {
  width: 30px;
}
</style>
