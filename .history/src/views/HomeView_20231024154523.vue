<template>
      <div class="row">
        <div class="col-lg-8 offset-lg-2">
          <div class="table-responsive">
            <table class="table table-bordered table-hover">
              <thead>
                <tr>
                  <th>#</th>
                  <th>ID</th>
                  <th>FOTO</th>
                  <th>NOMBRES</th>
                  <th>APELLIDOS</th>
                  <th>FECHA DE REGISTRO</th>
                  <th></th>
                </tr>
              </thead>
              
              <tbody class="table ">

              </tbody>
            </table>
          </div>
        </div>       
      </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}
</script>
