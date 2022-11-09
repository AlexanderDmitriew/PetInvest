<template>
    <div class="container">
        <div class="signup">
            <h2>Вход</h2>
            <input type="text" placeholder="Электронная почта">
            <input type="password" placeholder="Пароль">
            <button class="primary" @click="SingIn">Войти</button>
            <a @click="HelpPassword">Забыли пароль?</a>
        </div>
    </div>
</template>
  
<script>
import { ref } from 'vue'

export default {
    setup() {
        return {
            text: ref('')
        }
    },
    methods: {
        SingIn: function () {
            alert("Вы успешно вошли")
        },
        HelpPassword: function () {
            alert("Помощь по паролю")
        }
    }
}
</script>
  
<style>
a {
    cursor: pointer;
}

h2 {
    font-weight: 500;
    font-size: 2.6rem;
    top: -10px;
}

.signup {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

input {
    margin: 2%;
    background: none;
    color: white;
    padding: 8px 16px;
    min-height: 48px;
    min-width: 256px;
    border: 2px solid hsla(160, 100%, 37%, 1);
    border-radius: 8px;

}

.primary {
    background-color: hsla(160, 100%, 37%, 1);
    border: 2px solid hsla(160, 100%, 37%, 1);
    padding: 8px 16px;
    border-radius: 4px;
    min-width: 256px;
    color: #FAFAFA;
    cursor: pointer;
}


@media (max-width: 1024px) {
    .signup {
        min-height: 30vh;

    }
}
</style>
  