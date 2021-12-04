<template>
    <div>
        <layout-main>
            <div class="d-flex justify-content-between flex-wrap flex-md-nowrap align-items-center pt-3 pb-2 mb-3 border-bottom">
                <h1 class="text-light h2">User Details</h1>
            </div>
            <div class="text-dark">
                <div v-if="datausers==null" class="alert alert-danger" role="alert">
                    Data Not Found!
                </div>
                <div v-else class="card">
                    <img src="img/icons8-diamond-heart-90.png" class="card-img-top w-25" alt="...">
                    <div class="card-body">
                        <h5 class="card-title">{{datausers?.name}}</h5>
                        <address class="card-text">
                            <b>{{datausers?.username}}</b> <br>
                            {{datausers?.address.street}}, {{datausers?.address.suite}} <br>
                            {{datausers?.address.city}}, {{datausers?.address.zipcode}} <br>
                            {{datausers?.phone}} <br> {{datausers?.email}} <br>
                            {{datausers?.website}} <br>
                            <b>{{datausers?.company}}</b> <br>
                            {{datausers?.catchphrase}}
                        </address>
                    </div>
                </div>
            </div>
        </layout-main>
    </div>
</template>

<script>
import LayoutMain from '@/views/LayoutMain'

export default {
    components: {
        LayoutMain
    },
    data() {
        return {
            id : this.$route.params.id,
            username : this.$route.params.username,
            datausers: null,
            errormessage: null
        }
    },
    methods: {
        getDetailUsers(id){
            fetch("https://jsonplaceholder.typicode.com/users/" + id)
                .then(response => response.json()) //then 1, set response sebagai json
                .then(json => {
                    if(json?.id !== undefined){
                        this.datausers = json
                    } else {
                        this.errormessage = 'Data Not Found!';
                    }
                    
                    this.datausers = json;    
                    console.log(this.datausers)
                }) //then2, mengambil json dan ditampung/diset ke dalam data
                .catch(error => {
                    console.log(error);
                    this.errormessage = '404 Not Found :(';
                })
        }
    },
    mounted() {
        this.getDetailUsers(this.id)
    }
}
</script>