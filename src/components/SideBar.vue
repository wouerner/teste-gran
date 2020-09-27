<template>
    <div class="side-bar">

        <div class="logo">
            <img 
                class="logo-img"
                src="../assets/logo_gran.png"
            >
        </div>

        <ul class="list">
            <li>
                <span class="mdi mdi-email-outline"></span> Dashboard 
            </li>
            <li>
                <span class="mdi mdi-email-outline"></span> eCommerce 
            </li>
        </ul> 

        <h4 class="list-title">Apps</h4>
        <ul class="list">
            <li>
                <span class="mdi mdi-email-outline"></span> E-mail
            </li>
            <li>
                <span class="mdi mdi-email-outline"></span> Chat 
            </li>
            <li>
                <span class="mdi mdi-email-outline"></span> Todo 
            </li>
            <li>
                <span class="mdi mdi-email-outline"></span> Calendar 
            </li>
        </ul> 

        <h4 class="list-title">UI Elements</h4>
        <ul class="list">
            <li>
                <span class="mdi mdi-email-outline"></span> E-mail
            </li>
            <li>
                <span class="mdi mdi-email-outline"></span> Chat 
            </li>
            <li>
                <span class="mdi mdi-email-outline"></span> Todo 
            </li>
            <li>
                <span class="mdi mdi-email-outline"></span> Calendar 
            </li>
        </ul> 

        <h4 class="list-title">Forms</h4>
        <ul class="list">
            <li>
                <span class="mdi mdi-email-outline"></span> Form Elements
            </li>
            <li>
                <span class="mdi mdi-email-outline"></span> Form Layouts 
            </li>
            <li>
                <span class="mdi mdi-email-outline"></span> Form Wizard 
            </li>
            <li>
                <span class="mdi mdi-email-outline"></span> Form Validation 
            </li>
        </ul> 
    </div>
</template>

<script>

export default {
  name: 'SideBar',
  props: {
    msg: String
  }
}
</script>

<style scoped>
.logo {
    display: block;
    width:100%;
    height: 23px; 
    padding-top: 31px;
    padding-left: 40px;
}

.logo-img {
    float: left;
}

.list {
    list-style-type: none;
    text-align: left;
}

.list-title {
    font-family: Montserrat;
    font-style: normal;
    font-weight: normal;
    font-size: 14px;
    line-height: 36px;

    padding-left: 40px;

    color: #999999;

    text-align: left;
}
</style>
