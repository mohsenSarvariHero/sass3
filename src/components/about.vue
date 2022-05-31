<template>
    <div>
      <section class="sec1"><!--nav bar with css by ul,li -->
        <ul>
          <router-link to='/'><li ><a href="#">صفحه اصلی</a></li></router-link>
          <li ><a href="#LinkB"> درباره ما </a></li>
          <li ><a href="#LinkS"> مهارت ها </a></li>
          <li ><a href="#LinkC"> ارتباط با ما </a></li>
          <li class="left"><input type="text" name="inp1" style="text-align:right"></li>
          <a href="https://www.google.com/"><li class="left"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-search m-2" viewBox="0 0 16 16">
  <path d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"/>
</svg></li></a>
        </ul>
      </section>
      <section class="flexO">
        <article class="flexOF">
          <h2 class="wgh hover-4">Mohsen Sarvari</h2>
           <p>
          <b-calendar selected-variant="success" today-variant="info" nav-button-variant="primary"></b-calendar>
          </p>
           <h1>Digital Clock</h1>
  <div class="container">
    <div class="LCD">
      <div class="hours">{{ hours }}</div>
      <div class="divider">:</div>
      <div class="minutes">{{ minutes }}</div>
      <div class="divider">:</div>
      <div class="seconds">{{ seconds }}</div>
    </div>
  </div>
        </article>
        <article class="flexOS">
            <b-carousel
      id="carousel-fade"
      v-model="slide"
      :interval="4000"
      fade
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- Text slides with image -->
      <b-carousel-slide
        caption="First slide"
        text="Nulla vitae elit libero, a pharetra augue mollis interdum."
        img-src="https://picsum.photos/1024/480/?image=52"
      ></b-carousel-slide>

      <!-- Slides with custom text -->
      <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=54">
        <h1>Hello world!</h1>
      </b-carousel-slide>

      <!-- Slides with image only -->
      <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=58"></b-carousel-slide>

      <!-- Slides with img slot -->
      <!-- Note the classes .d-block and .img-fluid to prevent browser default image alignment -->
      <b-carousel-slide>
        <template #img>
          <img
            class="d-block img-fluid w-100"
            width="1024"
            height="480"
            src="https://picsum.photos/1024/480/?image=55"
            alt="image slot"
          >
        </template>
      </b-carousel-slide>

      <!-- Slide with blank fluid image to maintain slide aspect ratio -->
      <b-carousel-slide caption="Blank Image" img-blank img-alt="Blank image">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse eros felis, tincidunt
          a tincidunt eget, convallis vel est. Ut pellentesque ut lacus vel interdum.
        </p>
      </b-carousel-slide>
    </b-carousel>
        </article>
      </section>
<div id="LinkB">
      <section class="sec2" >
       <div class="sec2B" >
        <h2>به نام خدا</h2>
        <article class="bio1">
        <h3>سلام دوستان</h3>
        <h4>من محسن سروری</h4>
        <p>متولد 30 شهریور سال 1379 ساکن مشهد مقدس هستم. در خانواده ای بزرگ شدم که خیلی با تکنولوژی رابطه خوبی نداشتند و ا
          به همین دلیل به رشته کامپیوتر فکر نمیکردم بعد از گدراندن ابتدایی در مدرسه بنا خسروی و راهنمایی در مدرسه امام رضا و همچنین دبیرستان در مدرسه جباریان وارد دوران کنکور شدم و بعد از مشخص شدن نتایج با شرکت در همایش ها به رشته کامپیوتر رسدیم و با سوابق تحصیلی وارد دانشگاه خیام شدم و به خودم قول دادم که تلاشی که برای کنکور انجام ندادم جبران کنم و جزو نفرات برتر بشم و میدونستم کار سختی دارم. در کنار درس خواندن مشغول به یادگیری مهارت هم شدم و با طراحی سایت آشنا شدم و به طور خودآموز شروع به یادگیری کردم و خداروشگر نتایح خوبی هم گرفتم و جزو نفرات برتر دانشگاه در سایت شدم و هم چنین نفر دوم رشته کامپیوتر خیام در ورودی های خودم شدم و همه چیز عالی و درجه یک , چی بهتر از این و دوباره آماده برای شرکت در کنکور ارشد و استخدامی یا شروع بک استارت آپ تا خدا چی بخواد تا الان و چیزی که یاد گرفتم اول لطف خدا و بعد تلاش خودم.وامیدوارم همگی موفق و پیروزوسلامت در مسیر زندگی خودمان یاشیم چرا که ما بهترین زندگی داریم فقط باید بیشتر زندگی رو آسون بگیریم
        </p>💪❤
        </article>
        </div>
        <div class="sec2t">
        <img src="../assets/image/2.jpg" width="800" height="700">
        </div>
      </section>
</div>
<div class="hsec3" id="LinkS">
<section class="sec3">
  <article>
 <h5 >HTML</h5>
    <b-progress :value="value" :max="max" :precision="2" show-progress class="mb-3 w-70"></b-progress>
 <h5 >CSS</h5>
    <b-progress :value="value1" :max="max" :precision="2" show-progress class="mb-3 w-70"></b-progress>
 <h5 >SCSS</h5>
    <b-progress :value="value2" :max="max" :precision="2" show-progress class="mb-3 w-70"></b-progress>
 <h5 >BOOTSTRAP</h5>
    <b-progress :value="value3" :max="max" :precision="2" show-progress class="mb-3 w-70"></b-progress>
 <h5 >JS</h5>
    <b-progress :value="value4" :max="max" :precision="2" show-progress class="mb-3 w-70"></b-progress>
 <h5 >VUE.JS</h5>
    <b-progress :value="value5" :max="max" :precision="2" show-progress class="mb-3 w-70"></b-progress>
 <h5 >NODE.JS</h5>
    <b-progress :value="value6" :max="max" :precision="2" show-progress class="mb-3 w-70"></b-progress>
 <h5 >EXPRESS.JS</h5>
    <b-progress :value="value6" :max="max" :precision="2" show-progress class="mb-3 w-70"></b-progress>
 <h5 >MONGODB</h5>
    <b-progress :value="value7" :max="max" :precision="2" show-progress class="mb-3 w-70"></b-progress>
 <h5 >GIT</h5>
    <b-progress :value="value8" :max="max" :precision="2" show-progress class="mb-3 w-70"></b-progress>
  </article>
</section>
</div>
<section class="sec4" id="LinkC">
  <form>
    <fieldset>
      <legend>Contact us</legend>
      <div class="Contact">
      <article class="c1">
      <label>First Name</label><br>
      <input type="text" name="fN" size="50"><br>
      <br>
      <br>
      <label>Email</label><br>
      <input type="email" name="LN" size="50">
      </article>
      <article class="c2">
      <label>Last Name</label><br>
      <input type="text" name="LN" size="50">
      <br>
      <br>
      <br>
      <label>Phone</label><br>
      <input type="text" name="Ph" size="50">
      </article>
      </div>
      <br>
      <label>comment</label><br>
      <textarea cols="80" rows="10"></textarea><br>
      <button type="submit"> submit </button>
    </fieldset>
    <div>
      <h3 class="hover-2">mohsen sarvari</h3>
      <h4  class="hover-2">phone: +989152094629</h4>
      <h4  class="hover-2">e-mail: mohsen_sarvari2000@yahoo.com</h4>
    </div>
  </form>
</section>
    </div>
</template>
<script>
export default {
  name: 'about',
  data () {
    return {
      value: 90,
      value1: 90,
      value2: 90,
      value3: 90,
      value4: 80,
      value5: 80,
      value6: 60,
      value7: 70,
      value8: 75,
      max: 100,
      slide: 0,
      sliding: null,
      hours: 0,
      minutes: 0,
      seconds: 0
    }
  },
  mounted () {
    setInterval(() => this.setTime(), 1000)
  },
  methods: {
    setTime () {
      const date = new Date()
      let hours = date.getHours()
      let minutes = date.getMinutes()
      let seconds = date.getSeconds()
      hours = hours <= 9 ? `${hours}`.padStart(2, 0) : hours
      minutes = minutes <= 9 ? `${minutes}`.padStart(2, 0) : minutes
      seconds = seconds <= 9 ? `${seconds}`.padStart(2, 0) : seconds
      this.hours = hours
      this.minutes = minutes
      this.seconds = seconds
    },
    onSlideStart (slide) {
      this.sliding = true
    },
    onSlideEnd (slide) {
      this.sliding = false
    }
  }
}
</script>
<style scoped lang="scss">
.sec1{
  position: sticky;
  top:5px;
  z-index: 3;
}
.sec1 .left input{
  height: 10%;
}
.sec1 .left{
  float:left;
  width:0%;
}
.sec1 ul{
  list-style: none;
  background-color: rgb(56, 55, 58);
  overflow: hidden;
}
.sec1 ul li {
  float: right;
  width: 10%;
  line-height: 3.5rem;
}
.sec1 ul li:hover{
  background-color: rgba(155, 227, 236, 0.664);
}
.sec1 ul li a{
  text-decoration: none;
   --c: #1095c1;
  background:
    conic-gradient(from -135deg at 100%  50%,var(--c) 90deg,#0000 0) 0    var(--p,0%),
    conic-gradient(from -135deg at 1.2em 50%,#0000 90deg,var(--c) 0) 100% var(--p,0%);
  background-size: var(--s,0%) 200%;
  background-repeat: no-repeat;
  transition: .4s ease-in, background-position 0s;
  display: block;/*test with inline-block */
    color: rgb(225, 226, 126);
    font-size: 18px;
}
.sec1 ul li a:hover{
  color: white;
    --p: 100%;
  --s: calc(70% + .61em); /* it should be 0.6em(1.2em/2) but we use a litte bigger */
}
.wgh{
  background-image: conic-gradient(red,blue,green);
  color:white;
  line-height: 200%;
  width:30%;
  border-bottom-left-radius: 50px;
  border-top-right-radius: 50px;
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
.flexO{
  display: flex;
  width:100%;
}
.flexO article:first-child h2{
  width: 100%;
}
.flexO article:first-child{
  flex:10%;
  background-color: blue;
  padding: 10px;
}
.flexO article:last-child{
  flex:90%;
  background-color: rgb(36, 201, 137);
}
.LCD {
  display: flex;
  margin-left:70px;
}
.LCD > div {
  font-family: "alarm clock";
  font-size: x-large;
}
.sec2{
  background: url('../assets/image/3.jpg');
  background-repeat: no-repeat;
  height: 850px;
  background-size:cover;
  background-position: center;
  display: flex;
  flex-direction: row-reverse;
  padding: 20px 20px 0px 20px;
  background-attachment: fixed;
}
.sec2 .bio1 {
  text-align: justify;
  direction: rtl;
  padding: 20px;
  font-size: 1.5rem;
  background-color: #f8cb006e;
  text-shadow: 1px 1px rgb(110, 110, 219);
  box-shadow: 1px 1px rgb(226, 226, 231);
}
.sec2 .sec2t{
  padding: 90px 10px;
}
.hsec3{
  background-image: url('../assets/image/1.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
}
.sec3{
  background: url('../assets/image/Skill.jpg'),url('../assets/image/skill2.jpg');
  background-position: left,right;
  background-size: 400px 680px, 400px 600px;
  background-repeat: no-repeat;
  height: 700px;
}
.sec3 article{
  padding: 2% 30%;
}
.sec4{
  background-color: rgb(46, 46, 48);
  color: white;
}

.Contact{
  display: flex;
}
.Contact .c1{
  flex: 30;
}
.Contact .c2{
  flex: 30;
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
   color: #F8CA00;
}
input{
  border: 1px solid gray;
}
input:focus{
  border: 3px solid blue !important;
}
</style>
