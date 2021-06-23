<template>
  <div>
  <div id="wrapper">
      <div id="page-wrapper">
      <section class="container">
        <form id="val" @submit="checkForm" action="/something" method="post">
          <div id="app">
            <Surname msg="Фамилия"/>
            <Name msg="Имя"/>
            <Patronymic msg="Отчество"/>
            <DateOfBirth msg="Дата рождения"/>
            <Phone msg="Номер телефона"/>
            <Sex msg="Пол"/>
            <GroupOfClient msg="Группа клиентов"/>
            <Doctor msg="Лечащий врач"/>
            <Sms msg="Не отправлять СМС"/>
            <p/>
            <AddressIndex msg="Индекс"/>
            <Country msg="Страна"/>
            <Region msg="Область"/>
            <Town msg="Город"/>
            <Street msg="Улица"/>
            <House msg="Дом"/>
            <p/>
            <Document msg="Документ"/>
            <Series msg="Серия"/>
            <Number msg="Номер"/>
            <IssuedBy msg="Кем выдан"/>
            <DateOfIssue msg="Дата выдачи"/>
            <Validate type="submit"/>
          </div>
        </form>
      </section>
    </div>

  </div>
<Footer/>
  </div>
</template>

<script>
import Surname from './components/Surname.vue'
import Name from './components/Name.vue'
import Patronymic from "@/components/Patronymic";
import DateOfBirth from "@/components/DateOfBirth";
import Phone from "@/components/Phone";
import Sex from "@/components/Sex";
import Doctor from "@/components/Doctor";
import Sms from "@/components/Sms";
import AddressIndex from "@/components/AddressIndex";
import Country from "@/components/Country";
import Region from "@/components/Region";
import Town from "@/components/Town";
import Street from "@/components/Street";
import House from "@/components/House";
import Document from "@/components/Document";
import Series from "@/components/Series";
import Number from "@/components/Number";
import IssuedBy from "@/components/IssuedBy";
import DateOfIssue from "@/components/DateOfIssue";
import Validate from "@/components/Validate";
import GroupOfClient from "@/components/GroupOfClient";
import Footer from "@/components/Footer";

export default {
  el:'#val',
  components: {
    Footer,
    GroupOfClient,
    Validate,
    DateOfIssue,
    IssuedBy,
    Number,
    Series,
    Document,
    House,
    Street,
    Town,
    Region,
    Country,
    AddressIndex,
    Sms,
    Doctor,
    Sex,
    Phone,
    DateOfBirth,
    Patronymic,
    Surname,
    Name
  }
}

const val = new Vue({
  el:'#val',
  data:{
    errors:[],
    name:null,
    surname:null,
    movie:null
  },
  methods:{
    checkForm:function(e) {
      if(this.name && this.age) return true;
      this.errors = [];
      if(!this.name) this.errors.push("Name required.");
      if(!this.age) this.errors.push("Age required.");
      e.preventDefault();
    }
  }
})
</script>

<style>
@media screen and (max-width: 1000px) {
  #app,body, #wrapper, section,  form, input, label,div, select {
    width: 100%;
    margin-top: 0;
    padding: 0px 0px;
    text-align: left;
  }
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  box-shadow: 0px 0px 10px 5px rgba(0, 0, 0, .2);
  background: #ffe8e6;
  padding: 10%;
  float:left;
}
body {
  margin: 50px 0px 0px 0px;
  padding: 0;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 12px;
  color: #8F8F8F;
}


section {
  overflow: hidden;
  width: 90%;
  margin: 0px auto;
  padding: 5% 5%;
}

#wrapper {
  overflow: hidden;
  width: 70%;
  margin: 0px auto;
  background: #FFFFFF;
  box-shadow: 0px 0px 10px 5px rgba(0, 0, 0, .2);
}

form {
  text-align: center;
  margin: 0 auto;
  width: 50%;
}
* {
  box-sizing: border-box;
}

input[type=text], select, input[type=date] {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 4px;
  resize: vertical;
}

label {
  padding: 12px 12px 12px 12px;
  display: inline-block;
}


.container {
  border-radius: 5px;
  padding: 20px;
}

.col-25 {
  float: left;
  width: 40%;
  margin-top: 6px;
  text-align: left;
}

.col-75 {
  float: left;
  width: 60%;
  margin-top: 6px;
  text-align: left;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Responsive layout - when the screen is less than 600px wide, make the two columns stack on top of each other instead of next to each other */
@media screen and (max-width: 1000px) {
  .col-25, .col-75, form, select, input[type=text], input[type=date] {
    width: 100%;
    margin-top: 0;

  }
}

</style>
