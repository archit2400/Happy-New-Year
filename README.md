<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy New Year 2023</title>
    <style>
      @import url('https://fonts.googleapis.com/css?family=Montserrat:700|Pacifico');

*, *:after, *:before{
  box-sizing:border-box;
  margin:0;
  padding:0;
  -webkit-transition: all 100ms ease-in;
  transition: all 100ms ease-in;
}
html{
	background: #222048;
}
.feliz{
  width: 100%;
  font-family: 'Pacifico', cursive;
  font-size: 100px;
  font-weight: 700;
  color: #f48fb1;
  text-align: center;
  position: absolute;
  top: 50%;
  opacity: 0;
  animation: vem_feliz 2s ease-in-out 7s forwards;
}
.ano_novo{
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  overflow: hidden;
  padding: 200px 100px 0px 0px;
}
.ano_novo>span{
  font-family: 'Montserrat', sans-serif;
  font-size: 175px;
  font-weight: 700;
  color: #7a8fe8;
}
span.seis{
  position: absolute;
  top: 50%;
  right: 50%;
  margin-right: -200px;
  animation: vai_2016 5s ease-in-out 5s forwards;
}
span.sete{
  position: absolute;
  right: 0%;
  margin-right: -200px;
  animation: vem_2017 6s ease-in-out forwards;
}
span.sete:before{
  content: '';
  width: 0px;
  height: 6px;
  display: block;
  border-radius: 3px;
  background: #7a8fe8;
  transform: rotate(0deg);
  transform-origin: left top;
  position: absolute;
  top: 55px;
  left: 10px;
  z-index: -1;
  animation: entrega_balao 1s ease-in-out 4s;
}
.balao{
  width: 100px;
  height: 100px;
  display: block;
  background: #e8d57a;
  border-radius: 50%;
  position: absolute;
  top: 50%;
  margin-top: -165px;
  right: 0%;
  margin-right: -200px;
  animation: vem_e_vai_balao 10s ease-in-out forwards;
}
.balao:before{
  content: '';
  width: 0;
  height: 0;
  border-style: solid;
  border-width: 0 10px 20px 10px;
  border-color: transparent transparent #b19b32 transparent;
  position: absolute;
  left: 50%;
  margin-left: -10px;
  bottom: -10px;
  z-index: -1;
}
.balao:after{
  content: '';
  width: 4px;
  height: 100px;
  display: block;
  background: #fff;
  border-radius: 0px 0px 3px 3px;
  position: absolute;
  left: 50%;
  margin-left: -2px;
  bottom: -110px;
}
.fogos{
  width: 100%;
  height: 100%;
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  overflow: hidden;
}
.fogos>div{
  border: 2px solid #fff;
  position: absolute;
  opacity: 0;
  animation: solta_fogos 1.5s ease-in-out 8s forwards;
}
.fogos>div.f1{
  left: 20%;
  top: 40%;
}
.fogos>div.f2{
  left: 15%;
  top: 70%;
}
.fogos>div.f3{
  right: 20%;
  top: 40%;
}
.fogos>div.f4{
  right: 15%;
  top: 70%;
}
.fogos>div span{
  width: 6px;
  height: 6px;
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  opacity: 0;
  animation: estoura_fogos 0.5s ease-in-out 9s forwards;
}
.fogos>div span:nth-child(1){
  transform: rotate(0deg);
}
.fogos>div span:nth-child(2){
  transform: rotate(120deg);
}
.fogos>div span:nth-child(3){
  transform: rotate(240deg);
}
.fogos>div span:before{
  content: '';
  width: 2px;
  height: 50px;
  display: block;
  background: #f5cc06;
  position: absolute;
  top: -60px;
  left: 2px;
}
.fogos>div span:after{
  content: '';
  width: 2px;
  height: 50px;
  display: block;
  background: #f5cc06;
  position: absolute;
  bottom: -60px;
  left: 2px;
}
.fogos>div span i:before{
  content: '';
  width: 3px;
  height: 3px;
  display: block;
  border-radius: 50%;
  background: #fff;
  position: absolute;
  top: -15px;
  left: 10px;
}
.fogos>div span i:after{
  content: '';
  width: 3px;
  height: 3px;
  display: block;
  border-radius: 50%;
  background: #fff;
  position: absolute;
  top: -15px;
  right: 10px;
}
a.author{
  font-size: 12px;
  text-decoration: none;
  color: #f47c7c;
  position: fixed;
  bottom: 10px;
  right: 10px;
}

@keyframes vem_2017 {
  0% {
    right: 0%;
  }
  66.6666% {
    right: 50%;
    margin-right: -300px;
  }
  90% {
    right: 50%;
    margin-right: -300px;
  }
  100% {
    right: 50%;
  }
}
@keyframes vem_e_vai_balao {
  0% {
    right: 0%;
  }
  40% {
    right: 50%;
    margin-right: -300px;
  }
  50% {
    right: 50%;
    margin-right: -200px;
    top: 50%;
  }
  100% {
    top: -100%;
    right: 50%;
  }
}
@keyframes entrega_balao {
  0% {
    transform: rotate(-30deg);
    width: 40px;
  }
  100% {
    transform: rotate(-150deg);
    width: 70px;
  }
}
@keyframes vai_2016 {
  0% {
    top: 50%;
  }
  100% {
    top: -100%;
  }
}
@keyframes vem_feliz {
  0% {
    margin-top: 0px;
    opacity: 0;
  }
  100% {
    margin-top: -200px;;
    opacity: 1;
  }
}
@keyframes solta_fogos {
  0% {
    margin-top: 100%;
    opacity: 0;
    width: 2px;
    height: 30px;
    display: block;
    border-radius: 50%;
  }
  75% {
    margin-top: 0%;
    opacity: 1;
    width: 2px;
    height: 30px;
    display: block;
    border-radius: 50%;
  }
  80%{
    margin-top: 0px;
    margin-left: 0px;
    opacity: 1;
    width: 10px;
    height: 10px;
    display: block;
    border-radius: 50%;
    transform: scale(0.2);
  }
  100%{
    opacity: 1;
    width: 10px;
    height: 10px;
    display: block;
    border-radius: 50%;
    transform: scale(1);
  }
}
@keyframes estoura_fogos {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
    </style>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="feliz">Happy new year</div>
<div class="ano_novo">
  <span>202</span>
  <span class="seis">3</span>
  <span class="sete">4</span>
  <div class="balao"></div>
</div>
<div class="fogos">
  <div class="f1">
    <span><i></i></span>
    <span><i></i></span>
    <span><i></i></span>
  </div>
  <div class="f2">
    <span><i></i></span>
    <span><i></i></span>
    <span><i></i></span>
  </div>
  <div class="f3">
    <span><i></i></span>
    <span><i></i></span>
    <span><i></i></span>
  </div>
  <div class="f4">
    <span><i></i></span>
    <span><i></i></span>
    <span><i></i></span>
  </div>
</div>
<script>
  MorphSVGPlugin.convertToPath('polygon');
var xmlns = "http://www.w3.org/2000/svg",
  xlinkns = "http://www.w3.org/1999/xlink",
select = function(s) {
    return document.querySelector(s);
  },
  selectAll = function(s) {
    return document.querySelectorAll(s);
  },
  pContainer = select('.pContainer'),
  mainSVG = select('.mainSVG'),
  star = select('#star'),
  sparkle = select('.sparkle'),
  tree = select('#tree'),
  showParticle = true,
  particleColorArray = ['#E8F6F8', '#ACE8F8', '#F6FBFE','#A2CBDC','#B74551', '#5DBA72', '#910B28', '#910B28', '#446D39'],
  particleTypeArray = ['#star','#circ','#cross','#heart'],
 // particleTypeArray = ['#star'],
  particlePool = [],
  particleCount = 0,
  numParticles = 201


gsap.set('svg', {
  visibility: 'visible'
})

gsap.set(sparkle, {
    transformOrigin:'50% 50%',
    y:-100
})

let getSVGPoints = (path) => {
    
    let arr = []
    var rawPath = MotionPathPlugin.getRawPath(path)[0];
    rawPath.forEach((el, value) => {
        let obj = {}
        obj.x = rawPath[value * 2]
        obj.y = rawPath[(value * 2) + 1]
        if(value % 2) {
            arr.push(obj)
        }
        //console.log(value)
    })
    
    return arr;
}
let treePath = getSVGPoints('.treePath'),
    treeBottomPath = getSVGPoints('.treeBottomPath'),
    mainTl = gsap.timeline({delay:0, repeat:0}),
    starTl;

function flicker(p){

  gsap.killTweensOf(p, {opacity:true});
  gsap.fromTo(p, {
    opacity:1
  }, {
        duration: 0.07,
    opacity:Math.random(),
    repeat:-1
  })
}

function createParticles() {
  
  var i = numParticles, p, particleTl, step = numParticles/treePath.length, pos;
  while (--i > -1) {
    
    p = select(particleTypeArray[i%particleTypeArray.length]).cloneNode(true);
    mainSVG.appendChild(p);
    p.setAttribute('fill', particleColorArray[i % particleColorArray.length]);
    p.setAttribute('class', "particle");   
    particlePool.push(p);
    //hide them initially
    gsap.set(p, {
                 x:-100, 
                 y:-100,
   transformOrigin:'50% 50%'
                 })
    
    

  }

}

var getScale = gsap.utils.random(0.5, 3, 0.001, true);

function playParticle(p){
  if(!showParticle){return};
  var p = particlePool[particleCount]
 gsap.set(p, {
     x: gsap.getProperty('.pContainer', 'x'),
     y: gsap.getProperty('.pContainer', 'y'),
     scale:getScale()
    }
    );
var tl = gsap.timeline();
  tl.to(p, {
        duration: gsap.utils.random(0.61,6),
      physics2D: {
        velocity: gsap.utils.random(-23, 23),
        angle:gsap.utils.random(-180, 180),
        gravity:gsap.utils.random(-6, 50)
      },
      scale:0,
      rotation:gsap.utils.random(-123,360),
      ease: 'power1',
      onStart:flicker,
      onStartParams:[p],
      onRepeat: (p) => {
        gsap.set(p, {         
            scale:getScale()
        })
      },
      onRepeatParams: [p]

    });
  

  particleCount++;
  particleCount = (particleCount >=numParticles) ? 0 : particleCount
  
}

function drawStar(){
  
  starTl = gsap.timeline({onUpdate:playParticle})
  starTl.to('.pContainer, .sparkle', {
        duration: 6,
        motionPath :{
            path: '.treePath',
      autoRotate: false
        },
    ease: 'linear'
  })  
  .to('.pContainer, .sparkle', {
        duration: 1,
    onStart:function(){showParticle = false},
    x:treeBottomPath[0].x,
    y:treeBottomPath[0].y
  })
  .to('.pContainer, .sparkle',  {
        duration: 2,
    onStart:function(){showParticle = true},
        motionPath :{
            path: '.treeBottomPath',
      autoRotate: false
        },
    ease: 'linear'    
  },'-=0')
.from('.treeBottomMask', {
        duration: 2,
  drawSVG:'0% 0%',
  stroke:'#FFF',
  ease:'linear'
},'-=2')  
   
}


createParticles();
drawStar();

mainTl.from(['.treePathMask','.treePotMask'],{
    duration: 6,
  drawSVG:'0% 0%',
  stroke:'#FFF',
    stagger: {
        each: 6
    },
  duration: gsap.utils.wrap([6, 1,2]),
  ease:'linear'
})
.from('.treeStar', {
    duration: 3,
  scaleY:0,
  scaleX:0.15,
  transformOrigin:'50% 50%',
  ease: 'elastic(1,0.5)'
},'-=4')

 .to('.sparkle', {
    duration: 3,
    opacity:0,
    ease:"rough({strength: 2, points: 100, template: linear, taper: both, randomize: true, clamp: false})"
  },'-=0')
  .to('.treeStarOutline', {
    duration: 1,
    opacity:1,
    ease:"rough({strength: 2, points: 16, template: linear, taper: none, randomize: true, clamp: false})"
  },'+=1')

mainTl.add(starTl, 0)
gsap.globalTimeline.timeScale(1.5);

</script>
</body>
</html>
