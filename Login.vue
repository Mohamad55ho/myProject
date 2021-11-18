<template>

    <div class="bg-img">
        <div class="element">
            <img src="https://www.twoseatour.com/wp-content/uploads/2017/03/Two-Sea-Tour_LOGO.png" />
        </div>
        <div class="content">
            <form @submit.prevent="handleSubmit">
                <div class="form-group">
                    <input type="email" class="form-control" v-model="email" placeholder="Email" />
                </div>
                <div class="form-group">
                    <input type="password" class="form-control" v-model="password" placeholder="Password" />
                </div>
                <button class="btn btn-primary btn-block" @click="SubmitForm">Login</button>
                <hr />
                <button class="btn btn-success active btn-block">Create new account</button>
                </form>

        </div>

    </div>
</template>
<script>
  //   import axios from 'axios'
    export default {
        name: 'Login',
        data() {
            return {
                email: '',
                password: '',
            }
        },
      
        methods: {
            handleSubmit() {
                const data = {
                    email: this.email,
                    password: this.password

                };
                console.log(data);
            },
            /*async handleSubmit() {
                const response = await axios.post('/login', {
                    email : this.email,
                    password: this.password
                });
            console.log(response);
        }*/
           
        }
    }
 
</script>