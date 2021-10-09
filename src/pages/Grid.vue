<template>
    <div class="row justify-center" style="height: 100vh">


         <div class="col-6 col-md-3 self-center" >

          <q-card
            class="my-card text-white"

          >
            <q-card-section class="q-pt-none">




              <q-card-section>
                <q-card-section class="col-5 flex flex-left">

                  <img alt="tu colegio"
                       width="240"
                       height="50"
                       style="margin-left: -43px"
                       src="../assets/login.svg">


                </q-card-section>
                <div class="text-h6 text-black q-pa-sm">Inicia Sesion</div>
                <div class="text-pink-9 q-pa-sm">Usuario</div>
                <q-input outlined v-model="text" :dense="dense"/>
                <div class="text-pink-9 q-pa-sm">contraseña
                  <q-icon
                    name="visibility"
                    size="15px"
                    class="text-red; float-right"
                  />
                </div>
                <q-input outlined v-model="text" :dense="dense"/>
              </q-card-section>
              <q-card-section>
                <q-btn
                  label="Iniciar sesion"
                  class="full-width text-white"
                  color="warning"
                />
              </q-card-section>
            </q-card-section>
          </q-card>

        </div>
        <div class="col-6 col-md-3   self-center" >
          <q-card
          class="my-card text-white bg-primary "

        >

          <q-card-section class="q-pt-none">

            <img  height="380" width="300"  src="../assets/login-img.svg" >
          </q-card-section>
        </q-card></div>

    </div>
</template>

<script>
import {defineComponent} from 'vue'
import { ref } from 'vue'


export default defineComponent({
  name: 'Grid',
  setup () {
    return {
      dense: ref(true)
    }
  }
})
</script>
