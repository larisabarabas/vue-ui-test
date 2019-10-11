<script>
import '../styles/main-style.css'; 
export default {
    name:'login',
    components: {

    },
    data(){
        return {
            activeTab: 0
        }
    }
}
</script>

<template>
    <div class="login-section">
        <b-tabs v-model="activeTab" position="is-centered" class='block' expanded>
            <b-tab-item label = "Client">
                <h2>Client Login</h2>
                <div class="container mrg-top-50">
                    <b-field >
                            <b-input type="email"
                                maxlength="30" placeholder="Email address">
                            </b-input>
                    </b-field>
                     <b-field>
                        <b-input type="password" placeholder="Password"
                            password-reveal>
                        </b-input>
                    </b-field>
                    <b-button type="is-light" size="is-medium">Login</b-button>
                </div>
            </b-tab-item>
            <b-tab-item label = "Supplier">
                <h2>Supplier login</h2>
                   <div class="container mrg-top-50">
                    <b-field >
                            <b-input type="email"
                                maxlength="30" placeholder="Email address">
                            </b-input>
                    </b-field>
                     <b-field>
                        <b-input type="password" placeholder="Password"
                            password-reveal>
                        </b-input>
                    </b-field>
                    <b-button type="is-light" size="is-medium">Login</b-button>
                </div>
            </b-tab-item>
        </b-tabs>
    </div>
</template>

<style scoped>
    div.login-section{
        width: 500px;
        margin: 50px 50px;
        background-color: white;
        border-radius: 5px;
    }
    .container{
        text-align: left;
    }
</style>