<script setup>

import Button from './core/Button.vue'
import InputBlock from './core/InputBlock.vue';
import Form from './core/Form.vue';

// new Core(AuntificationModel).init()
localStorage.setItem("theme", "light-theme");

// export default createRouter
//   ({
//     history: createWebHashHistory(),
//     routes:
//       [
//         { path: '/sus', component: HelloWorld },
//         { path: '/sus2', component: TheWelcome }
//       ]
//   })

</script>

<template>
  <!-- <router-view></router-view> -->

  <Form confirm_name="Войти"/>
  <!-- <header>
                  <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

                  <div class="wrapper">
                    <HelloWorld msg="You did it!" />
                  </div>
                </header> -->

  <!-- <main>
                  <TheWelcome />
                </main> -->
</template>

<!-- <style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style> -->
