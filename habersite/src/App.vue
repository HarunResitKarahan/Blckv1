<template>
  <div class="Homepage">
    <!-- NAVBAR -->
    <b-navbar class="shadow-sm" toggleable="lg" variant="white">
      <!-- Hava Durumu -->
      <b-navbar-nav class="ml-auto">
        <b-nav-form>
          <b-form-input
            size="sm"
            class="shadow-sm mr-sm-0"
            placeholder="Search"
          ></b-form-input>
          <b-button size="sm" class="aramatusu shadow-sm my-2 my-sm-0 pr-3" type="submit"><i class="fa fa-search"></i></b-button>
        </b-nav-form>
        <b-nav-item-dropdown class="ml-3" right>
          <!-- Using 'button-content' slot -->
          <template #button-content>
            <img src="@/indir.png" width="25px" class="m-0"/>
          </template>
          <b-dropdown-item href="#">Profile</b-dropdown-item>
          <b-dropdown-item href="#">Sign Out</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-navbar>
    <!-- İÇERİK -->
    <b-container class="bv-example-row mt-4" fluid>
      <b-row>
        <!-- SOLMENU -->
        <b-col class="solgrid p-1 pt-5" cols="2">
          <!-- ROUTER -->
          <div class="Home">
            <router-link id="menu" class="shadow-sm" to="/home"
            >Home
            <i class="fa fa-caret-right"></i>
            <ul class="droprightmenu shadow-sm">
              <li>
                <a href="#"
                  ><img class="shadow katagoridownmenu" src="@/1.png" alt=""/></a>
              </li>
              <li>
                <a href="#"
                  ><img class="shadow katagoridownmenu" src="@/1.png" alt=""/></a>
              </li>
              <li>
                <a href="#"
                  ><img class="shadow katagoridownmenu" src="@/1.png" alt=""/></a>
              </li>
              <li>
                <a href="#"
                  ><img class="shadow katagoridownmenu" src="@/1.png" alt=""/></a>
              </li>
              <li>
                <a href="#"
                  ><img class="shadow katagoridownmenu" src="@/1.png" alt=""/></a>
              </li>
            </ul>
            </router-link>
          </div>
          <div class="About">
            <router-link id="menu" class="shadow-sm" to="/about"
            >About
            <i class="fa fa-caret-right"></i>
            <ul class="droprightmenu shadow-sm">
              <li>
                <a href="#"
                  ><img class="shadow katagoridownmenu" src="@/2.jpg" alt=""
                /></a>
              </li>
              <li>
                <a href="#"
                  ><img class="shadow katagoridownmenu" src="@/2.jpg" alt=""
                /></a>
              </li>
              <li>
                <a href="#"
                  ><img class="shadow katagoridownmenu" src="@/2.jpg" alt=""
                /></a>
              </li>
              <li>
                <a href="#"
                  ><img class="shadow katagoridownmenu" src="@/2.jpg" alt=""
                /></a>
              </li>
              <li>
                <a href="#"
                  ><img class="shadow katagoridownmenu" src="@/2.jpg" alt=""
                /></a>
              </li>
            </ul>
          </router-link>
          </div>
        </b-col>
        <!-- ORTAKISIM -->
        <b-col class="ortagrid" cols="8 p-0 pt-4" align="center">
          <!-- ÜSTKISIM -->
          <div class="ustkisim" align="left">
            <h4>SON DAKİKA</h4>
            <p id="p1">09:05</p>
            <p id="p2"> Bakan Koca, vaka sayıları artan ve azalan illeri açıkladı Bakan Koca, vaka sayıları artan ve azalan illeri açıkladı</p>
          </div>
          <!-- MANSET -->
        <div align="left" class="manset">
          <b-carousel
            id="carousel-1"
            class="pl-2"
            align= "center"
            v-model="slide"
            :interval="5000"
            controls
            indicators
            style="text-shadow: 1px 1px 2px #333;"
            @sliding-start="onSlideStart"
            @sliding-end="onSlideEnd"
          >
            <b-carousel-slide>
              <template #img>
                <img
                  class="d-block img-fluid w-100"
                  src="@/3.jpg"
                  alt="image slot"
                >
              </template>
              <p>
                 Bakan Koca, vaka sayıları artan ve azalan illeri açıkladı Bakan Koca, vaka sayıları artan ve azalan illeri açıkladı
              </p>
            </b-carousel-slide>
            <b-carousel-slide>
              <template #img>
                <img
                  class="d-block img-fluid w-100"
                  src="@/3.jpg"
                  alt="image slot"
                >
              </template>
              <p>
                 Bakan Koca, vaka sayıları artan ve azalan illeri açıkladı Bakan Koca, vaka sayıları artan ve azalan illeri açıkladı
              </p>
            </b-carousel-slide>
          </b-carousel>
          <div class="minimanset pt-2 pb-3" style="display: block" align="center">
            <a href="#">
              <img class="h-50" src="@/genzo.jpg" alt="">
              <span align="center">Bakan Koca, vaka sayıları artan ve azalan illeri açıkladı Bakan Koca, vaka sayıları artan ve azalan illeri açıkladı</span>
            </a>
            <div class="h-100">
              <a href="#">
                <img class="mt-2 h-50" src="@/genzo.jpg" alt="">
              </a>
            </div>
          </div>
        </div>
          <hr/>
          <div>
            <iframe class="doviz" src="https://www.genelpara.com/embed/?symbol=para-birimleri&pb=XU100,USD,EUR,BTC,GA,EUR/USD&stil=stil-4&renk=beyaz" frameborder="0"></iframe>
          </div>
          <!-- ORTARESİM -->
          <div class="row">
            <div class="resimler">
              <a href="#"><img class="shadow" src="@/2.jpg" alt=""><span align="center">Bakan Koca, vaka sayıları artan ve azalan illeri açıkladı Bakan Koca, vaka sayıları artan ve azalan illeri açıkladı</span></a>
              <a href="#"><img class="shadow" src="@/2.jpg" alt=""></a>
              <a href="#"><img class="shadow" src="@/2.jpg" alt=""></a>
              <a href="#"><img class="shadow" src="@/2.jpg" alt=""></a>
              <a href="#"><img class="shadow" src="@/2.jpg" alt=""></a>
              <a href="#"><img class="shadow" src="@/2.jpg" alt=""></a>
            </div>
          </div>
        </b-col>
        <b-col class="sagkisim" cols="2 mt-5" align="center">
          <iframe class="havadurumu" src="https://www.havadurumu15gunluk.xyz/sitene-ekle/2/havadurumu.php?il=istanbul&ilce=istanbul&bg=&title=00134a" frameborder="0" width="200" height="50" __idm_frm__="480"></iframe>
          <iframe class="havadurumu" src="https://www.havadurumu15gunluk.xyz/sitene-ekle/2/havadurumu.php?il=ankara&ilce=ankara&bg=&title=00134a" frameborder="0" width="200" height="50" __idm_frm__="480"></iframe>
          <iframe class="havadurumu" src="https://www.havadurumu15gunluk.xyz/sitene-ekle/2/havadurumu.php?il=izmir&ilce=izmir&bg=&title=00134a" frameborder="0" width="200" height="50" __idm_frm__="480"></iframe>
          <iframe class="havadurumu" src="https://www.havadurumu15gunluk.xyz/sitene-ekle/2/havadurumu.php?il=manisa&ilce=manisa&bg=&title=00134a" frameborder="0" width="200" height="50" __idm_frm__="480"></iframe>
          <iframe class="havadurumu" src="https://www.havadurumu15gunluk.xyz/sitene-ekle/2/havadurumu.php?il=bursa&ilce=bursa&bg=&title=00134a" frameborder="0" width="200" height="50" __idm_frm__="480"></iframe>
          <iframe class="havadurumu" src="https://www.havadurumu15gunluk.xyz/sitene-ekle/2/havadurumu.php?il=bilecik&ilce=bilecik&bg=&title=00134a" frameborder="0" width="200" height="50" __idm_frm__="480"></iframe>
          <iframe class="havadurumu" src="https://www.havadurumu15gunluk.xyz/sitene-ekle/2/havadurumu.php?il=antalya&ilce=antalya&bg=&title=00134a" frameborder="0" width="200" height="50" __idm_frm__="480"></iframe>
          <iframe class="havadurumu" src="https://www.havadurumu15gunluk.xyz/sitene-ekle/2/havadurumu.php?il=adana&ilce=adana&bg=&title=00134a" frameborder="0" width="200" height="50" __idm_frm__="480"></iframe>
        </b-col>
      </b-row>
    </b-container>
    <router-view />
  </div>
</template>

<style lang="scss">
body{
  background: rgb(226, 226, 226);
}
hr{
  background: white;
  width: 90%;
}
.doviz{
  width: 97.6%;
  height: 46px;
}
.havadurumu{
  background: white;
  min-width: 80%;
  margin-top: 10px;
  padding-top: 3px;
  border-radius: 15px;
}
@media only screen and (max-width: 1405px) {
}
//SOL MENU

#menu:hover {
  font-size: 17px;
  width: 104%;
  .fa {
    margin-left: 5px;
  }
  .droprightmenu {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    background: white;
  }
}

</style>
