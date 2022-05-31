<template>
  <div class="hello">
    <router-link to="#"><a href="#kan">jump</a></router-link>
    <h1 class="icon-OK">fffff</h1><h2><span class="icon-ok"></span></h2>
    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-search" viewBox="0 0 16 16">
  <path d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"/>
</svg>
    <p>var</p>
    <p>https://www.w3schools.com/css/css3_variables.asp</p>
    <p>https://www.w3schools.com/cssref/playdemo.asp?filename=playcss_background-image</p>
    <p>https://developer.mozilla.org/en-US/docs/Web/CSS/background-clip</p>
   <h2 class="wgh hover-4">Mohsen Sarvari</h2>
  <h3>MOhsen</h3>
  -----
  <p>https://css-tricks.com/the-selectmenu-element/</p>
<selectmenu class="my-custom-select">
  <div slot="button">
    <button behavior="button">Open</button>
    <span class="label">Choose an option</span>
     <p class=" icon-menu" style="color:red;margin-right:7px;margin-top:-40px;"></p>
  </div>
  <option>Option 1</option>
  <option>Option 2</option>
  <option>Option 3</option>
</selectmenu>
<input type="text" >
--<p>https://css-tricks.com/css-hover-effects-background-masks-3d/</p>
<h3 class="hover-1">Hover Me</h3>
<h3 class="hover-2">Hover Me</h3>
<h3 class="hover-3">Hover Me</h3>
<h3 class="hover-4">Hover Me</h3>
--------------
<p>https://css-tricks.com/cool-hover-effects-using-background-properties/</p>

<h3 class="hover-11">1. Hover Me</h3>
<h3 class="hover-12">2. Hover Me</h3>
<h3 class="hover-13">3. Hover Me</h3>
<h3 class="hover-14">4. Hover Me</h3>
<h3 class="hover-5">4. Hover Me</h3>
<p class="icon-bell"></p>
  <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
            <ol class="carousel-indicators">
             <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
             <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
             <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
            </ol>
  <div class="carousel-inner" id="kan">
    <div class="carousel-item active">
      <img class="d-block w-100" src="../assets/image/1.jpg" alt="First slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="../assets/image/2.jpg" alt="Second slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="../assets/image/3.jpg" alt="Third slide">
    </div>
  </div>
  <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

$color:red;
$bjk:blue;
.wgh{
  background-image: conic-gradient(red,blue,green);
  color:white;
  line-height: 200%;
  width:30%;
  border-bottom-left-radius: 50px;
  border-top-right-radius: 50px;
}
.hover-1 {
  --c: #1095c1; /* the color */
  --s: .15em;
  line-height:1.1em;
  padding-bottom: calc(2.1*var(--s));
  background:conic-gradient(from 135deg at top,var(--c) 90deg,#0000 0)
      left 0 bottom var(--s)/calc(2*var(--s)) var(--s) repeat-x,
    conic-gradient(from -45deg at bottom,var(--c) 90deg,#0000 0)
      left var(--s) bottom 0/calc(2*var(--s)) var(--s) repeat-x;
  -webkit-mask:
  linear-gradient(#000 0 0) content-box,
  linear-gradient(#000 0 0) 0/var(--_p,0%) padding-box no-repeat;
  transition: .5s;
}
.hover-1:hover {
  --_p: 100%;
  color: var(--c);
}

.hover-2 {
  --c: #1095c1; /* the color */
  --b: .1em;    /* border length*/
  --d: 20px;    /* the cube depth */
  --_s: calc(var(--d) + var(--b));
  color: var(--c);
  border: solid #0000;
  border-width: var(--b) var(--b) var(--_s) var(--_s);
  background:
      conic-gradient(at left var(--d)  bottom var(--d),#0000 90deg,rgba(197, 81, 81, 0.3) 0 225deg,rgba(204, 31, 31, 0.6) 0) border-box,
    conic-gradient(at left var(--_s) bottom var(--_s),
      #0000 90deg,var(--c) 0) 0 100%/calc(100% - var(--b)) calc(100% - var(--b))  border-box;
  transform: translate(calc(var(--d)/-1),var(--d));
  clip-path:
    polygon(
     var(--d) 0%,
     var(--d) 0%,
     100% 0%,
     100% calc(100% - var(--d)),
     100% calc(100% - var(--d)),
     var(--d) calc(100% - var(--d))
    );
  transition: 0.5s;
}
.hover-2:hover {
  transform: translate(0,0);
  clip-path:
    polygon(
     0% var(--d),
     var(--d) 0%,
     100% 0%,
     100% calc(100% - var(--d)),
     calc(100% - var(--d)) 100%,
     0% 100%
   );
}
.hover-3 {
  --b: 0.1em;   /* the thickness of the line */
  --c: #1095c1; /* the color */
  color: #0000;
  padding-block: var(--b);
  background: linear-gradient(var(--c) 50%,#000 0) 0% calc(100% - var(--_p,0%))/100% 200%,
    linear-gradient(var(--c) 0 0) 0% var(--_p,0%)/var(--_p,0%) var(--b) no-repeat;
  -webkit-background-clip: text,padding-box;
          background-clip: text,padding-box;
  transition: .3s var(--_s,0s) linear,background-size .3s calc(.3s - var(--_s,0s));
}
.hover-3:hover {
  --_p: 100%;
  --_s: .3s;
}
.hover-4 {
  border: 8px solid;
  border-image: repeating-linear-gradient(135deg,#F8CA00 0 10px,#E97F02 0 20px,#BD1550 0 30px) 8;
  -webkit-mask:
    conic-gradient(from 180deg at top 8px right 8px, #0000 90deg,#000 0)
     var(--_i,200%) 0  /200% var(--_i,8px) border-box no-repeat,
    conic-gradient(at bottom 8px left  8px,  #0000 90deg,#000 0)
     0   var(--_i,200%)/var(--_i,8px) 200% border-box no-repeat,
    linear-gradient(#000 0 0) padding-box no-repeat;
  transition: .3s, -webkit-mask-position .3s .3s;
}
.hover-4:hover {
  --_i: 100%;
  color: #CC333F;
  transition: .3s, -webkit-mask-size .3s .3s;
}

body {
  height: 100vh;
  margin: 0;
  display: grid;
  grid-template-columns: auto auto;
  gap: 20px 50px;
  place-content: center;
  align-items: end;
}
h3 {
  font-family: system-ui, sans-serif;
  font-size: 4rem;
  margin:0 auto;
  cursor: pointer;
  padding: 0 .1em;
}
  .my-custom-select [slot='button'] {
    display: flex;
    align-content: center;
  }
  .my-custom-select button {
    padding: 5px;
    border: none;
    background: #f06;
    border-radius: 5px 0 0 5px;
    color: white;
    font-weight: bold;
  }
  .my-custom-select .label {
    padding: 5px;
    border: 1px solid #f06;
    border-radius: 0 5px 5px 0;
  }

// h3 {
//   color:antiquewhite;
//   margin: 40px 0 0;
//   background-color: $bjk;
// }
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
 .my-select-menu::part(button) {
    color: white;
    background-color: #f00;
    padding: 5px;
    border-radius: 5px;
  }

  .my-select-menu::part(listbox) {
    padding: 10px;
    margin-top: 5px;
    border: 1px solid red;
    border-radius: 5px;
  }
  .hover-11 {
  background: linear-gradient(#1095c1 0 0) var(--p,0)/var(--p,0) no-repeat;
  transition: .4s,background-position 0s;
}
.hover-11:hover {
  --p: 100%;
  color: #fff;
}
.hover-12 {
  background:
    linear-gradient(#1095c1 0 0) no-repeat
     calc(200% - var(--p,0%)) 100% / 200% var(--p,.08em);
  transition: .3s var(--t,0s), background-position .3s calc(.3s - var(--t,0s));
}
.hover-12:hover {
  --p: 100%;
  --t: .3s;
  color: #fff;
}
.hover-13 {
  --c: no-repeat linear-gradient(#1095c1 0 0);
  background:
    var(--c)  calc(-101% + var(--p,0%)) 100%,
    var(--c)  calc( 201% - var(--p,0%)) 0;
  background-size: 50.1% var(--p,.08em);
  transition: .3s var(--t,0s), background-position .3s calc(.3s - var(--t,0s));
}
.hover-13:hover {
  --p: 101%;
  --t: 0.3s;
  color: #fff;
}
.hover-14 {
  --c: #1095c1;
  line-height: 1.2em;
  background:
    conic-gradient(from -135deg at 100%  50%,var(--c) 90deg,#0000 0) 0    var(--p,0%),
    conic-gradient(from -135deg at 1.2em 50%,#0000 90deg,var(--c) 0) 100% var(--p,0%);
  background-size: var(--s,0%) 200%;
  background-repeat: no-repeat;
  transition: .4s ease-in, background-position 0s;
}
.hover-14:hover {
  --p: 100%;
  --s: calc(50% + .61em); /* it should be 0.6em(1.2em/2) but we use a litte bigger */
  color: #fff;
}
.hover-5 {
  background-image: linear-gradient(#a1d2e2,#10b4eb) ;
  background-size: 0 100%;
  background-repeat: no-repeat;
  transition: .4s;
}
.hover-5:hover {
  background-size: 100% 100%;
  background-position: right;
  color:white;
}
</style>
