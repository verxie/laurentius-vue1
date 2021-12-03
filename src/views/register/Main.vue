<template>
    <div>
        <div class="container">
        <div class="row mt-5">
            <div class="col-md-4 rounded py-4 offset-md-4 text-light">
                <form>
                    <div class="text-center">
                        <img src="img/icons8-diamond-heart-90.png" width="30%" class="mb-2 " alt="">
                    </div>
                    <h1 class="h3 fw-bold text-center">REGISTER</h1>
                    <br>
                    <div class="mb-3">
                        <input type="name" class="form-control mb-1" id="InputName" placeholder="Name">
                        <input type="email" class="form-control mb-1" id="InputEmail1" placeholder="Email">
                        <input type="password" class="form-control" id="InputPassword1" placeholder="Password">
                    </div>
                    <hr>
                    <div class="row">
                        <div class="col-md-6 offset-md-3 d-grid gap-1">
                            <button type="submit" class="btn btn-primary">SIGN UP</button>
                        </div>
                    </div>
                    <br>
                    <div class="d-grid gap-2 col-6 mx-auto">
                        <label class="text-center text-light fs-6">Have an account?</label>
                        <label class="text-center text-light fs-6"><a href="#">LOGIN</a></label>
                      </div>
                  </form>
            </div>
        </div>
    </div>
    </div>
</template>

<script>
export default {
    name: 'register'
}
</script>