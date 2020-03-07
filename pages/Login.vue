<template>
    <div>

    <md-toolbar class="md-accent">
      <h3 class="md-title">NuxtPlay</h3>
    </md-toolbar>

        <md-card>
            <md-card-header>
                <label>Log In</label>
            </md-card-header>

            <md-card-content>
                <md-field>
                    <label>Email</label>
                    <md-input v-model="username"></md-input>
                </md-field>

                <md-field>
                    <label>Password</label>
                    <md-input v-model="password" type="password"></md-input>
                </md-field>
            </md-card-content>

            <md-button class="md-accent md-raised" @click="logCredentials()">Log In</md-button>

        </md-card>
    </div>
</template>

<script>
export default {
    name: 'MaterialIcons',
    data: () => ({
        username: '',
        password: '',
    }),

    methods: {
        logCredentials() {
            console.log(this.username)
            console.log(this.password)
        },
    }
}
</script>

<style scoped>
.image {
    position: relative;
    left: 18%
}

.md-card {
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 50%;
    margin: 4px;
    display: inline-block;
    vertical-align: top;
}
</style>