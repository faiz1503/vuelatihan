<template>
  <div class="profile">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-lg-6">
          <div class="media text-left">
            <img src="../assets/profile.jpg" class="user-pic mr-3" />
            <div class="media-body">
              <h5 class="mt-0">Faiz Keren</h5>
              <p>
                Cras sit amet nibh libero, in gravida nulla. Nulla vel metus
                scelerisque ante sollicitudin. Cras purus odio, vestibulum in
                vulputate at, tempus viverra turpis. Fusce condimentum nunc ac
                nisi vulputate fringilla. Donec lacinia congue felis in
                faucibus.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import "bootstrap/dist/css/bootstrap.css";

export default {
  name: "Profile",
  components: {},
};
</script>

<style scoped>
.user-pic {
    border-radius: 200%;
    height: 100px;
    width: 100px;
}
</style>
