<template>
  <div>
    <nav class="navbar navbar-red bg-black justify-content-between flex no-wrap flex-row">
      <div class="container mt-3">
        <a class="navbar-brand float-left">EMPLOYEE MANAGEMENT SYSTEM<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="./assets/bhushan.jpg" alt="img-fluid" height="75"></a>
        <ul class="nav navbar-nav flex-row">

          <li class="nav-item">
            <router-link class="nav-link pr-3" to="/">Home</router-link>
          </li>
          <br /> 
          <li class="nav-item">
            <router-link class="nav-link" to="/addEmployee">Add Employee</router-link>
          </li>
          <br />
          <li class="nav-item">
            <router-link class="nav-link" to="/addEmployee">Employees</router-link>
          </li>
        </ul>
      </div>
    </nav>


    <!--Router View-->
    <div class="container mt-5">
      <router-view></router-view>
    </div>
  </div>
</template>

<script>

import AddEmployee from '../src/components/AddEmployee.vue'
export default {
    name:'App',
    data(){
      return{
        msg:"Welcome"
      }
    },
    components:{
      AddEmployee
    }
}
</script>

<style>
</style>
