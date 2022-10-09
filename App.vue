<template>
<div>
<div class="www"><h1 class="number">{{count}} </h1></div>

<div class="clas"><a class="tasbeh" href="#" v-on:click="increment">{{count}}</a><a class="nollars" href="#" v-on:click="count = 0"><p class="harf">Reset</p></a></div>
<!-- <a class="minuss" href="#" v-on:click="count--"><p class="clik">kamaytiring</p></a> -->
<a href="https://t.me/ProgrammerEng" class="foter"> <p class="buyrtma">Buyurtmalar Uchun</p></a>
<!-- <table v-for="item of ismalar" :key="item" >
  <tbody> 
   <td > {{ item.name }}</td>
   <td> {{ item.age }}</td>
   <td> {{ item.job }}</td></tbody>
</table> -->
</div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
data(){
    return{
        //o'zgaruvcilar ,arraylar,object lar uchun joy

        count : 0,
        zero:0,
        ismalar:[
          {name:"Zilola ",
          age:12 ,
          job:"O'quvchi "},

          {name:"Lola ",
          age:25 ,
          job:"Medik "},

          {name:"Feruza",
          age:13,
          job:"Bekorchi"}
      ]
    }
},
methods:{
    //funksiyalar e'lon qilinadi
    increment(){
        this.count++;
    },
    nol(){
        if (this.zero){

        }
    }
    
},
}
</script>

<style>

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body{
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
}
.minuss{
    display: inline-block;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    width: 60px;
    height: 60px;
    border: 5px solid greenyellow;
    text-decoration: none;
    font-family: sans-serif;
transform: translate(99px,-70px);

}
.clik{
    text-decoration: none;
}
.nollars{
    display: inline-block;
    display: flex;
    justify-content: center;
    align-items: center;

    position: relative;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    /* background: #ccc; */
    display: flex;
    text-decoration: none;
    font-family: sans-serif;
    align-items: center;
    justify-content: center;
    color: #333;
    text-shadow: -2px -2px 5px rgb(183, 182, 182);
    filter: drop-shadow(4px 4px 10px #fff);
    box-shadow: inset 10px 10px 10px rgba(0, 0, 0, 0.2),
    10px 15px 10px rgba(0, 0, 0, 0.2),
    15px 20px 20px rgba(0, 0, 0, 0.2),
    inset -10px -10px 15px rgba(225,225,255,0.9);
    user-select: none;
transform: translate(99px,-70px);


}
.harf{
    color: black;
}
.tasbeh{
    margin-top: 200px;
    display: inline-block;
    width: 150px;
    height: 150px;
    border-radius: 50%;
    position: relative;
    text-decoration: none;
    font-size: 50px;
    width: 150px;
    height: 150px;
    border-radius: 50%;
    font-family: sans-serif;
    /* background: #ccc; */
    display: flex;
    align-items: center;
    justify-content: center;
    color: #333;
    text-shadow: -2px -2px 5px #fff;
    filter: drop-shadow(4px 4px 10px #fff);
    box-shadow: inset 10px 10px 10px rgba(0, 0, 0, 0.2),
    15px 25px 10px rgba(0, 0, 0, 0.2),
    15px 20px 20px rgba(0, 0, 0, 0.2),
    inset -10px -10px 15px rgba(225,225,255,0.9);
    user-select: none;

}
.tasbeh:active{
color: red
;}
.www{
    width: 300px;
    height: 70px;
    border: 5px solid rgb(162, 0, 255);
    display: flex;
    align-items: center;
    justify-content: center;
    margin-top: 50px;
    margin-left: -20px;
    color: rgb(34, 104, 255);
    text-shadow:0 0 10px 10px  red;

}
.number{
font-family: sans-serif;
font-size: 70px;
font-weight: lighter;
}


.clas{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
.p{
    margin-top: 50px;
    font-family: sans-serif;
}
.foter{
    background: #000;
    width: 100%;
    height: 70px;
    bottom: -150px;
    right: 0;
    position: absolute;
    display: flex;
   justify-content: center;
   align-items: center;
}
.buyrtma{
    color: white;
    text-decoration: none;
    font-family: sans-serif;
    font-size: 30px;
    text-align: center;
}
#app {


}
</style>
