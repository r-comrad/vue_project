<script setup>
import { ref } from "vue";
import InputBlock from "./InputBlock.vue";
import Button from "./Button.vue";

defineProps(['confirm_name'])

const username = ref("");
const password = ref("");
const res = ref("AAAAAA")
const inputs = ref([
    { id: 1, name: 'Логин', text: '' },
    { id: 2, name: 'Пароль', text: '' }
])

// const error = ref(null)

// const errorTag = computed(() => ({
//     'text-danger': error.value && error.value.type === 'fatal'
// }))

</script>

<template>
    <InputBlock v-for="inp in inputs" :key="inp.id" :name="inp.name" @textUpdated="(n) => inp.text = n"></InputBlock>
    <Button :text=confirm_name />
    <br>

    <div v-for="inp in inputs" :key="inp.id">
        <p>{{ inp.text }}</p>
        <br>
    </div>
    



    <!-- <div class="d-flex justify-content-center align-items-center py-5" style="height: 80vh">
            <div class="col-4 card ">
                <div class="card-body">
                    <div class="alert alert-danger" role="alert" :class="errorTag">Неправильный логин или пароль</div>

                    <div class="form-group my-3">
                        <label for="username" class="form-label">Имя пользователя</label>
                        <input type="text" name="username" id="username" class="form-control" v-model="username">
                    </div>
                    <div class="form-group">
                        <label for="username" class="form-label">Пароль</label>

                        <div class="input-group my-3" id="show_hide_password">
                            <input type="password" name="password" id="pass" class="form-control" v-model="password">
                            <button class="btn btn-secondary" type="button" onclick="">
                                <i id="icon" class="bi bi-eye-fill"></i>
                            </button>
                        </div>
                    </div>
                    <button class="btn btn-primary my-3" @click="login">Зайти</button>
                </div>
            </div>
        </div> -->
</template>

<style scoped></style>
