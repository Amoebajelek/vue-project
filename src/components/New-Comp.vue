<template>
  <div class="container">
    <div class="row justify-content-center">
      <div class="col-lg-6 col-sm-12">
        <div class="form-group">
          <textarea
            class="form-control"
            rows="4"
            id="comment"
            placeholder="What's happening?"
          ></textarea>
        </div>
        <ul class="nav mt-3 justify-content-end">
          <!-- <li class="nav-item px-3">
            <img src="../assets/ic-status-1.png" alt="" class="icon" />
          </li>
          <li class="nav-item px-3">
            <img src="../assets/ic-status-2.png" alt="" class="icon" />
          </li>
          <li class="nav-item px-3">
            <img src="../assets/ic-status-3.png" alt="" class="icon" />
          </li>
          <li class="nav-item px-3">
            <img src="../assets/ic-status-4.png" alt="" class="icon" />
          </li>
          <li class="nav-item px-3">
            <img src="../assets/ic-status-5.png" alt="" class="icon" />
          </li> -->
          <li class="justify-content-end">
            <button type="button" class="btn btn-dark">Tweeta!</button>
          </li>
        </ul>
        <hr />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "NewComp",
};
</script>

<style>
.container {
  margin-top: 70px;
  margin-bottom: -50px;
  border: 1 solid black;
}

.btn-dark {
  font-size: 18px !important;
}

textarea {
  font-size: 22px !important;
}

.icon {
  width: 30px;
}
</style>
