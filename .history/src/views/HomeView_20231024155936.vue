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

                  <tr v-if="this.cargando">
                      <td colspan="6"><h3>Cargando...</h3></td>
                  </tr>
                  
                  <tr v-else v-for="est, i in this.estudiantes" :key="est.id">
                      <td v-text="(i+1)"></td>
                      <td v-text="(est.id)"></td>
                      <td v-text="(est.foto)"></td>
                      <td v-text="(est.nombre)"></td>
                      <td v-text="(est.apellido)"></td>
                      <td v-text="(est.created_at)"></td>
                      <td>

                      </td>
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
      },
      mounted(){
        this.getEstudiantes();
      },

      methods:{
        getEstudiantes(){
          this.cargando = true;
          axios.get()
        }
      }
  }
</script>
