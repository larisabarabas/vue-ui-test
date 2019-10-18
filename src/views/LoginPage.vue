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
    <div class="container-is-fluid">
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
                    <div class="card">
                        <div class="card-image">
                            <figure class="image is-4by3">
                            <img src="https://bulma.io/images/placeholders/1280x960.png" alt="Placeholder image">
                            </figure>
                        </div>
                        <div class="card-content">
                            <div class="media">
                            <div class="media-left">
                                <figure class="image is-48x48">
                                <img src="https://bulma.io/images/placeholders/96x96.png" alt="Placeholder image">
                                </figure>
                            </div>
                            <div class="media-content">
                                <p class="title is-4">John Smith</p>
                                <p class="subtitle is-6">@johnsmith</p>
                            </div>
                            </div>

                            <div class="content">
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                            Phasellus nec iaculis mauris. <a>@bulmaio</a>.
                            <a href="#">#css</a> <a href="#">#responsive</a>
                            <br>
                            <time datetime="2016-1-1">11:09 PM - 1 Jan 2016</time>
                            </div>
                        </div>
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