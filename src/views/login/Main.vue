<template>
    <div>
        <div class="container">
        <div class="row mt-5">
            <div class="col-md-4 rounded py-4 offset-md-4 text-light">
                <form>
                    <h1 class="h3 fw-bold text-center">LOGIN</h1>
                    <br>
                    <div class="mb-3">
                      <label for="InputEmail1" class="form-label">Email address</label>
                      <input type="email" class="form-control" id="InputEmail1">
                    </div>
                    <div class="mb-3">
                      <label for="InputPassword1" class="form-label">Password</label>
                      <input type="password" class="form-control" id="exampleInputPassword1">
                    </div>
                    <br>
                    <div class="row">
                        <div class="col-md-12 d-grid">
                        <router-link class="text-center btn btn-primary" :to="{name: 'dashboard'}">LOGIN</router-link>
                        </div>
                    </div>
                    <br>
                    <div class="d-grid gap-2 col-6 mx-auto">
                        <label class="text-center text-light fs-6">Don't have an account?</label>
                        <router-link class="text-center" :to="{name: 'register'}">Register</router-link>
                      </div>
                  </form>
            </div>
        </div>
    </div>
    </div>
</template>

<script>
export default {
    name: 'login'
}
</script>