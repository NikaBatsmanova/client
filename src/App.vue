<template>
  <div id="wrapper">
    <div id="header-wrapper">
      <header>
        <div id="logo">

        </div>
        <menu>
          <ul>
            <li><a href="index.html">Тестовое задание на позицию Junior FrontEnd Developer.</a></li>
          </ul>
        </menu>
      </header>
    </div>

    <div id="page-wrapper">
      <section>
        <form id="app">
            <Surname msg="Фамилия"/>
            <Name msg="Имя"/>
            <Patronymic msg="Отчество"/>
            <DateOfBirth msg="Дата рождения"/>
            <Phone msg="Номер телефона"/>
            <Sex msg="Пол"/>
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
        </form>
      </section>
    </div>

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

export default {
  name: 'PersonalData',
  components: {
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
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0 auto;
  float:left
}
body {
  margin: 50px 0px 0px 0px;
  padding: 0;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 12px;
  color: #8F8F8F;
}

header {
  width: 100%;
  height: 10%;
  margin: 0 auto;
  padding: 0px 0px;
}

menu {
  float: right;
  width: 70%;
  height: 80px;
  padding: 20px 40px 0px 0px;
}

menu ul {
  width: 100%;
  float: right;
  margin: 0;
  padding: 40px 0px 0px 0px;
  list-style: none;
  line-height: normal;
}

menu li {
  width: 100%;
  float: left;
}

menu a {
  display: block;
  margin-left: 1px;
  padding: 7px 20px 7px 20px;
  letter-spacing: 1px;
  text-decoration: none;
  text-align: center;
  text-transform: uppercase;
  font-family: 'Oswald', sans-serif;
  font-size: 18px;
  font-weight: 300;
  color: #e8e2dc;
}

menu a:hover, menu .current_page_item a {
  text-decoration: none;
  background: #F08080;
  box-shadow: inset 0px 0px 10px 5px rgba(0, 0, 0, .1);
  border-radius: 5px;
  color: #36332E;
}

section {
  overflow: hidden;
  width: 90%;
  margin: 0px auto;
  padding: 50px 40px;
  color: #8F8F8F;
}

#wrapper {
  overflow: hidden;
  width: 70%;
  margin: 0px auto;
  background: #FFFFFF;
  box-shadow: 0px 0px 10px 5px rgba(0, 0, 0, .2);
}

#header-wrapper {
  overflow: hidden;
  height: 150px;
  background: #292521;
}
form {
  text-align: center;
  margin: 0 auto;
  width: 40%;
}
</style>
