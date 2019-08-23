<template>
  <div class="app">
    <div class="header row">
      <div class="menu-button row middle-xs center-xs">
        <div>
          <i class="fa fa-lg fa-bars" style="color:white"></i>
        </div>
      </div>
      <div class="tabs col-xs row bottom-xs">
        <div class="tab open row middle-xs center-xs">
          <div>John Wick</div>
        </div>
        <div class="tab row middle-xs center-xs">
          <div>
            <i class="fa fa fa-plus"></i>
          </div>
        </div>
      </div>
    </div>
    <div class="main row">
      <div class="menu">
        <div class="menu-item">
          <i class="fa fa-lg fa-search"></i>
        </div>
        <div class="menu-item">
          <i class="fa fa-lg fa-black-tie"></i>
        </div>
        <div class="menu-item">
          <i class="fa fa-lg fa-envelope"></i>
        </div>
        <div class="menu-item">
          <i class="fa fa-lg fa-question-circle"></i>
        </div>
      </div>
      <div class="order col-xs">
        <div class="search row">
          <div class="search-block col-xs">
            <input type="text" style="width:80%; height:20px;" />&nbsp;
            <i class="fa fa-lg fa-search"></i>
            <br />
            <br />John Wick
            <br />(404) 555-5555
          </div>
          <div class="search-block col-xs">
            <input type="text" style="width:80%; height:20px;" />&nbsp;
            <i class="fa fa-lg fa-search"></i>
            <br />
            <br />FIL 1515
            <br />NAPA Filter Gold
          </div>
          <div class="search-block col-xs"></div>
        </div>
        <div class="cart">
          <table width="100%">
            <tr class="table-header">
              <td>Item</td>
              <td>Price</td>
              <td>Qty</td>
              <td>Unit</td>
              <td>Total</td>
            </tr>
            <tr>
              <td colspan="5">
                <hr />
              </td>
            </tr>
            <tr>
              <td>FIL 1515</td>
              <td>$10.99</td>
              <td>10</td>
              <td>ea</td>
              <td>$109.90</td>
            </tr>
            <tr>
              <td>BRK 342223</td>
              <td>$104.99</td>
              <td>1</td>
              <td>ea</td>
              <td>$104.99</td>
            </tr>
            <tr>
              <td>FIL 1515</td>
              <td>$10.99</td>
              <td>10</td>
              <td>ea</td>
              <td>$109.90</td>
            </tr>
          </table>
        </div>
      </div>
      <div class="aux"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BaseComponent",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div {
  padding: 0px;
  margin: 0px;
  border: 0;
}
.header {
  width: 100%;
  height: 50px;
  background-color: darkgray;
}

.menu-button {
  flex-basis: 50px;
  height: 100%;
  background-color: #444;
}

.tabs {
  height: 100%;
}

.tab {
  width: 40px;
  height: 35px;
  margin-left: 5px;
  font-weight: bold;
  background-color: white;
  border-radius: 10px 10px 0px 0px;
  border-bottom: 1px solid lightgray;
}

.tab.open {
  margin-left: 25px;
  width: 200px;
  border-bottom: none;
}

.main {
  width: 100%;
  height: calc(100% - 50px);
  background-color: magenta;
}

.menu {
  flex-basis: 50px;
  padding-top: 20px;
  /* height: 100%; */
  background-color: gray;
}

.menu-item {
  width: 22px;
  height: 35px;
  color: white;
  padding: 14px;
  cursor: pointer;
}

.order {
  /* height: 100%; */
}

.search {
  height: 180px;
  width: 100%;
  background-color: white;
}

.search-block {
  height: calc(100%-40px);
  border-left: 1px solid lightgray;
  padding: 10px;
  margin-right: 5px;
  margin-top: 10px;
  margin-bottom: 10px;
}

.cart {
  height: calc(100% - 200px);
  width: calc(100% - 20px);
  padding: 10px;
  background-color: whitesmoke;
}

.table-header {
  font-weight: bold;
}

.aux {
  width: 30%;
  height: 100%;
  background-color: #ccc;
  float: left;
}
</style>
