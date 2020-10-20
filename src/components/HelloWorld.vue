<template>
  <div class="container">
      <side-bar />

      <div class="content">

          <div class="app-bar"> 
              <div>
                  <span class="mdi mdi-check-box-outline"></span> 
                  <span class="mdi mdi-message-outline "></span>  
                  <span class="mdi mdi-email-outline "></span>  
                  <span class="mdi mdi-calendar-blank-outline "></span>  
                  <span class="mdi mdi-star-outline "></span>  
              </div>
              <div class="app-user-bar">
                  <span class="app-lang">
                      english
                  </span>

                  <span class="mdi mdi-magnify"></span>  
                  <span class="mdi mdi-bell-outline"></span>  

                  <span class="app-user">
                      Jhon Doe<br/>
                      avaliable
                  </span>
                  <img 
                      src="../assets/Oval.png"
                  >

              </div>
 
          </div>

          <div class="bradcrumb"> breadcrumb
              Card Actions |eCommerce >> Eltronics 
          </div>

          <div class="list">

              <div class="filter"> 
                  <h4>filter</h4>
                  <div class="filter-box"> 
                      <h5>Multi Range</h5>
                      <div>
                          <input type="radio" id="scales" name="scales" checked>
                          <label for="scales">$10</label>
                      </div>
                      <div>
                          <input type="radio" id="scales" name="scales" checked>
                          <label for="scales">$10-$100</label>
                      </div>
                      <div>
                          <input type="radio" id="scales" name="scales" checked>
                          <label for="scales">$100-$500</label>
                      </div>
                      <div>
                          <input type="radio" id="scales" name="scales" checked>
                          <label for="scales">$500</label>
                      </div>
                      <div>
                          <input type="radio" id="scales" name="scales" checked>
                          <label for="scales">All</label>
                      </div>

                      <hr>

                      <h5>Slider</h5>

                      <hr>

                      <h5>Category</h5>
                      <div>
                          <input type="checkbox" id="scales" name="scales" checked>
                          <label for="scales">Cell Phones 1920</label>
                      </div>
                      <div>
                          <input type="checkbox" id="scales" name="scales" checked>
                          <label for="scales">Computer & Tablets 1820</label>
                      </div>

                      <hr>
                      <h5>Brand</h5>
                      <div>
                          <input type="checkbox" id="scales" name="scales" checked>
                          <label for="scales">Cell Phones 1920</label>
                      </div>
                      <div>
                          <input type="checkbox" id="scales" name="scales" checked>
                          <label for="scales">Computer & Tablets 1820</label>
                      </div>

                      <h5>Ratings</h5>
                      <div>
                          <input type="checkbox" id="scales" name="scales" checked>
                          <label for="scales">Cell Phones 1920</label>
                      </div>
                      <div>
                          <input type="checkbox" id="scales" name="scales" checked>
                          <label for="scales">Computer & Tablets 1820</label>
                      </div>
                      <button type="button">
                          Clear all filters
                      </button>
                  </div>
              </div>

              <div class="list-item">
                  <input placeholder="Search hear" class="search" type="text">
                  <div 
                      v-for="(item, index) in [1, 2, 3, 4, 5]"
                      class="card"
                      :key="index"
                  > 
                      <img 
                          class="card-img"
                          src="../assets/beats-headphones.png"
                      >
                      <div class="card-content">
                          <h3 class="card-title">
                              Apple Watch
                          </h3>
                          <h4 class="card-subtitle">
                              By Apple
                          </h4>
                          <p>
                              rem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of L
                          </p>
                      </div>
                      <div class="card-action">
                          <span>
                              star
                          </span>
                          <p>$399 <br>Free Shipping
                          </p>
                          <button class="btn">
                              wishlist
                          </button>
                          <button class="btn-reverse">
                             add to cart 
                          </button>
                      </div>
                  </div> 

              </div>
          </div>
      </div>
  </div>
</template>

<script>
import SideBar from './SideBar'
export default {
  name: 'HelloWorld',
  components:{
    SideBar
  },
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.container{
    display: grid;
    grid-template-columns: 280px auto;
}

.side-bar {

    background: #FFFFFF;
    box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.170509);
}

.content {
    display: grid;

    background: #F9F9F9;
    box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.0778245);
}

.app-bar {
    display: flex;
    justify-content: space-between;
    align-items: center;

    font-size: 22pt;

    min-height: 62px;

    background: #FFFFFF;
    box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
    border-radius: 8px;

    margin-left: 37px;
}

.app-icons {

}

.app-lang {
    font-family: Montserrat;
    font-style: normal;
    font-weight: normal;
    font-size: 14px;
    line-height: 17px;
    color: #2C2C2C;
}

.app-user {
    font-family: Montserrat;
    font-style: normal;
    font-weight: normal;
    font-size: 14px;
    line-height: 17px;
    color: #2C2C2C;
}

.app-user-bar {
    display:flex;
    justify-content: space-between;
    width: 300px;

}

.app-user-image {
  border-radius: 50%;
}

.bradcrumb{
    font-family: Montserrat;
    font-style: normal;
    font-weight: normal;
    font-size: 24px;
    line-height: 29px;
    text-align: left;
    margin-left: 37px;

    margin-top: 30px;
}

.filter {
    left: 14.43%;
    right: 0%;
    top: 0%;
    bottom: 0%;
    text-align: left;

    margin-left: 37px;

    background: #F9F9F9;
    box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.0778245);
}

.filter-box {
    width: 371px;

    background: #FFFFFF;
    box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
    border-radius: 8px;
}

.list {
    display: flex;
    margin-top: 51px;
}
.list-item{
    margin-left: 30px;
}

.search {
    background: #FFFFFF;
    box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
    border-radius: 8px;

    width: 100%;
    height: 62px;

    font-family: Montserrat;
    font-style: normal;
    font-weight: 300;
    font-size: 22px;
    line-height: 26px;
    color: #999999;
}

.card {
    display: flex;
    justify-content: space-between;
    padding: 20px;
    padding-right: 0px;
    padding-left: 10px;
    margin-top: 27px;

    height: 250px;
    width: 1170px;

    background: #FFFFFF;
    box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
    border-radius: 8px;
}

.card-img {

}

.card-content{
    padding-left: 23px;
    padding-right: 74px;
}

.card-title {
    height: 19px;

    font-family: Montserrat;
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
    line-height: 19px;

    /* identical to box height, or 119% */

    color: #2C2C2C;
}

.card-subtitle {
    height: 14px;
    left: 50%;
    right: 47.14%;
    top: calc(50% - 14px/2 - 581px);

    font-family: Montserrat;
    font-style: normal;
    font-weight: 300;
    font-size: 12px;
    line-height: 14px;

    /* identical to box height, or 117% */

    color: #7E7E7E;
}

.card-text {
    height: 93px;
    left: 50%;
    right: 17.6%;
    top: calc(50% - 93px/2 - 505.5px);

    font-family: Montserrat;
    font-style: normal;
    font-weight: 300;
    font-size: 14px;
    line-height: 23px;
    color: #2C2C2C;
}

.card-action {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 226px;
    padding: 20px; 
    border-left: 1px solid #DADADA;
}

.btn {
    width: 186px;
    height: 45px;
    left: 0%;
    right: 0%;
    top: 0%;
    bottom: 0%;

    background: #EDEDED;
    border-radius: 8px;
}

.btn-reverse {
    width: 185px;
    height: 45px;

    left: 0%;
    right: 0%;
    top: 0%;
    bottom: 0%;

    background: #686868;
    border-radius: 8px;
}
</style>
