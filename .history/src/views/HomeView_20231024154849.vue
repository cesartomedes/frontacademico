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
              
              <tbody class="table-group-divider" id="contenido">
                  <tr v-if="cargando">

                  </tr>
              </tbody>
            </table>
          </div>
        </div>       
      </div>
</template>

<script>
  import axios from 'axios';
  
  export default{
      data(){
        return{
          estudiantes:null,
          cargando:false
        }
      }
  }
</script>
