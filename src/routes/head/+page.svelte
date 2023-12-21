<script>

</script>

<svelte:head>
	<title>Head</title>
</svelte:head>

<!-- De code voor het hoofd is eerlijk gejat can sanne van t hooft https://github.dev/shooft/your-tribe-profile-card -->
<main>
	<div class="grid" />
    <header class="head">
          
        <aside class="🌟">
          <em tabindex=0></em>
        </aside>
        
        <ul class="eyes">
            <li class="eye">
                <em class="⭐"></em>
            </li>
            <li class="eye">
                <em class="⭐"></em>
            </li>
        </ul>
        
        <strong class="nose"></strong>
        <output class="mouth"></output>
        <input class="ear" type="text">
        <input class="ear" type="text">
    </header>


</main>

<style>
    :root {

        /* hooft */
      --head-size:10em;
      --head-time-mood-change:1s;
      --head-bg:bisque;
      --head-bg-dark:#ffb699;
      --head-shadow:crimson;
  
      --head-light-x-default:.675;
      --head-light-y-default:.175;
  
      --head-glimmer-x-min:.17;
      --head-glimmer-x-max:calc(1 - var(--head-glimmer-x-min));
      --head-glimmer-y-min:.08;
      --head-glimmer-y-max:.225;
      --head-glimmer-time-rotate:10s;
      --head-glimmer-time-rotate-happy:.5s;
      --head-glimmer-time-filter:.3s;
      --head-glimmer-time-move:.15s;
      --head-glimmer-size:.2;
      --head-glimmer-clr:white;
  
      --head-balkje-time-mood-change:1s;
      --head-balkje-time-fcs:.3s;
      --head-balkje-time-correct:1s;
      --head-balkje-time-incorrect:.25s;
      --head-balkje-bg:black;
      --head-balkje-clr:salmon;
      --head-balkje-placeholder-clr:transparent;
      --head-balkje-placeholder-clr-hvr:#9996;
      --head-balkje-placeholder-clr-fcs:#999;
      --head-balkje-bg-correct:salmon;
  
      --head-oog-wit-bg:white;
      --head-oog-iris-bg: steelblue;
      --head-oog-iris-bg-boos:crimson;
      --head-oog-pupil-bg:black;
      --head-oog-shadow:burlywood;
  
      --head-wenkbrouw-bg:LemonChiffon;
  
      --head-highlight-x-limit:36%;
      --head-highlight-time-move:.15s;
      --head-highlight-time-rotate:10s;
      --head-highlight-time-flash:.5s;
      --head-highlight-time-spin:1s;
      --head-highlight-bg:white;
      --head-neus-bg:bisque;
      --head-neus-shadow:burlywood;
  
      --head-mond-bg:salmon;
      --head-mond-shadow:crimson;
  
      --head-oren-time-flap:.05s;
    }

	main {
		min-width: 100vw;
		height: 100vh;
		left: 0;
		top: 0;
		position: relative;
		display: flex;
		align-items: center;
		justify-content: center;
	}

	.grid {
	width: 5em;
	height: 5em;
	align-self: flex-start;
	justify-self: flex-start;
	background-color: hsl(180 100% 50%);
	box-shadow: 
	-30em 0 hsl(72 100% 50%),
	-30em 5em hsl(240 100% 50%),
	-30em 10em hsl(30 100% 50%),
	-30em 15em hsl(219 100% 50%),
	-30em 20em hsl(102 100% 50%),
	-30em 25em hsl(225 100% 50%),
	-30em 30em hsl(75 100% 50%),
	-30em 35em hsl(210 100% 50%),
	-25em 0 hsl(267 100% 50%),
	-25em 5em hsl(315 100% 50%),
	-25em 10em hsl(165 100% 50%),
	-25em 15em hsl(114 100% 50%),
	-25em 20em hsl(339 100% 50%),
	-25em 25em hsl(234 100% 50%),
	-25em 30em hsl(51 100% 50%),
	-25em 35em hsl(132 100% 50%),
	-20em 0 hsl(213 100% 50%),
	-20em 5em hsl(270 100% 50%),
	-20em 10em hsl(201 100% 50%),
	-20em 15em hsl(168 100% 50%),
	-20em 20em hsl(228 100% 50%),
	-20em 25em hsl(54 100% 50%),
	-20em 30em hsl(318 100% 50%),
	-20em 35em hsl(105 100% 50%),
	-15em 0 hsl(327 100% 50%),
	-15em 5em hsl(237 100% 50%),
	-15em 10em hsl(78 100% 50%),
	-15em 15em hsl(192 100% 50%),
	-15em 20em hsl(341 100% 50%),
	-15em 25em hsl(171 100% 50%),
	-15em 30em hsl(57 100% 50%),
	-15em 35em hsl(231 100% 50%),
	-10em 0 hsl(333 100% 50%),
	-10em 5em hsl(321 100% 50%),
	-10em 10em hsl(216 100% 50%),
	-10em 15em hsl(204 100% 50%),
	-10em 20em hsl(24 100% 50%),
	-10em 25em hsl(174 100% 50%),
	-10em 30em hsl(135 100% 50%),
	-10em 35em hsl(60 100% 50%),
	-5em 0 hsl(195 100% 50%),
	-5em 5em hsl(177 100% 50%),
	-5em 10em hsl(108 100% 50%),
	-5em 15em hsl(180 100% 50%),
	-5em 20em hsl(138 100% 50%),
	-5em 25em hsl(81 100% 50%),
	-5em 30em hsl(27 100% 50%),
	-5em 35em hsl(111 100% 50%),
	0 5em hsl( 123 100% 50%),
	0 10em hsl(324 100% 50%),
	0 15em hsl( 153 100% 50%),
	0 20em hsl(42 100% 50%),
	0 25em hsl(150 100% 50%),
	0 30em hsl(273 100% 50%),
	0 35em hsl(293 100% 50%),
	5em 0 hsl(345 100% 50%),
	5em 5em hsl(87 100% 50%),
	5em 10em hsl(358 100% 50%),
	5em 15em hsl(284 100% 50%),
	5em 20em hsl(351 100% 50%),
	5em 25em hsl(156 100% 50%),
	5em 30em hsl(309 100% 50%),
	5em 35em hsl(45 100% 50%),
	10em 0 hsl(287 100% 50%),
	10em 5em hsl(296 100% 50%),
	10em 10em hsl(276 100% 50%),
	10em 15em hsl(69 100% 50%),
	10em 20em hsl(348 100% 50%),
	10em 25em hsl(312 100% 50%),
	10em 30em hsl(159 100% 50%),
	10em 35em hsl(299 100% 50%),
	15em 0 hsl(279 100% 50%),
	15em 5em hsl(336 100% 50%),
	15em 10em hsl(3 100% 50%),
	15em 15em hsl(147 100% 50%),
	15em 20em hsl(63 100% 50%),
	15em 25em hsl(39 100% 50%),
	15em 30em hsl(99 100% 50%),
	15em 35em hsl(281 100% 50%),
	20em 0 hsl(84 100% 50%),
	20em 5em hsl(252 100% 50%),
	20em 10em hsl(66 100% 50%),
	20em 15em hsl(156 100% 50%),
	20em 20em hsl(183 100% 50%),
	20em 25em hsl(12 100% 50%),
	20em 30em hsl(249 100% 50%),
	20em 35em hsl(6 100% 50%),
	25em 0 hsl(302 100% 50%),
	25em 5em hsl(126 100% 50%),
	25em 10em hsl(96 100% 50%),
	25em 15em hsl(255 100% 50%),
	25em 20em hsl(36 100% 50%),
	25em 25em hsl(120 100% 50%),
	25em 30em hsl(144 100% 50%),
	25em 35em hsl(305 100% 50%),
	30em 0 hsl(258 100% 50%),
	30em 5em hsl(246 100% 50%),
	30em 10em hsl(330 100% 50%),
	30em 15em hsl(159 100% 50%),
	30em 20em hsl(9 100% 50%),
	30em 25em hsl(243 100% 50%),
	30em 30em hsl(48 100% 50%),
	30em 35em hsl(15 100% 50%),
	35em 0 hsl(186 100% 50%),
	35em 5em hsl(261 100% 50%),
	35em 10em hsl(33 100% 50%),
	35em 15em hsl(141 100% 50%),
	35em 20em hsl(90 100% 50%),
	35em 25em hsl(162 100% 50%),
	35em 30em hsl(18 100% 50%),
	35em 35em hsl(207 100% 50%),
	40em 0 hsl(290 100% 50%),
	40em 5em hsl(129 100% 50%),
	40em 10em hsl(117 100% 50%),
	40em 15em hsl(222 100% 50%),
	40em 20em hsl(198 100% 50%),
	40em 25em hsl(189 100% 50%),
	40em 30em hsl(21 100% 50%),
	40em 35em hsl(264 100% 50%);
	z-index: -1;
}


/****************/
/****************/
/**            **/
/**  'T HOOFT  **/
/**            **/
/****************/
/****************/

.head {
 	position:relative;
	
	mix-blend-mode: difference;
	
	width:var(--head-size);
	aspect-ratio:4/5;
	flex-shrink:0;
	
	display:grid;
	align-content:end;
	justify-items:center;
	gap:4%;
	
	background-color:var(--head-bg);
	background-image:
		radial-gradient(
			farthest-side at center bottom,
			transparent 88%,
			var(--head-bg-dark) 98%
		);
	background-size: 400% 300%;
	background-position:50% 0%;
	border-radius:50%/ 50% 50% 25% 25%;
	box-shadow:0 0 1.5em var(--head-shadow);

	animation: breathing 4s infinite alternate;
}


/**************/
/* DE GLIMMER */
/**************/

.head .🌟 {
	position:absolute;
	inset:0;
	z-index:500;
	border-radius:inherit;

	-webkit-mask:
		linear-gradient(
			hsl(180 100% 50%),calc( (var(--head-glimmer-y-max) - var(--head-glimmer-size)/4) * 100%),
			transparent calc( (var(--head-glimmer-y-max) + var(--head-glimmer-size)/4) * 100%)
		);
	mask:
		linear-gradient(
			hsl(180 100% 50%),calc( (var(--head-glimmer-y-max) - var(--head-glimmer-size)/4) * 100%),
			transparent calc( (var(--head-glimmer-y-max) + var(--head-glimmer-size)/4) * 100%)
		);
}

.head .🌟 em {
	position:absolute;
	left:calc( 
			( 
				clamp(
					var(--head-glimmer-x-min), 
					var(--head-light-x, var(--head-light-x-default)), 
					var(--head-glimmer-x-max)
				) 
				- var(--head-glimmer-size) / 2 
			) * 100%
		);
	top:calc( 
			( 
				clamp(
					var(--head-glimmer-y-min), 
					var(--head-light-y, var(--head-light-y-default)), 
					var(--head-glimmer-y-max)
				)
				- var(--head-glimmer-size) / 2 
			) * 100%
		);

	width:calc(var(--head-glimmer-size) * 100%);
	aspect-ratio:1/1;

	filter:blur(2px);
	-webkit-mask:radial-gradient(closest-side circle, #f00c 25%,#f003);
	mask:radial-gradient(closest-side circle, #f00c 25%,#f003);

	cursor:grab;

	transition: filter var(--head-glimmer-time-filter);
	animation:🌟 var(--head-glimmer-time-rotate) linear infinite;
}

.head .🌟 em:focus-visible {
	outline:none;
	filter:none;
}

.head.moving .🌟 em {
	transition:var(--head-glimmer-time-move);
}

.head .🌟 em::before,
.head .🌟 em::after {
	content:"";
	position:absolute;
	inset:0;
	background-color:var(--head-glimmer-clr);
	transform:rotate(var(--ry, 0deg)) skew(25deg, 25deg) scale(.5);
}

.head .🌟 em::after {
	--ry:90deg;
}

/***********/
/* DE OGEN */
/***********/

.head .eyes {
	margin:0; padding:0;
	list-style:none;
	
	grid-area:1 / 1;
	justify-self:stretch;
	align-self:end;
	margin-bottom:20%;
	z-index:200;
	
	display:flex;
	justify-content:center;
	gap:4%;
		
	transition:var(--head-time-mood-change);
}

/* EEN OOG */
.head .eye {
	position:relative;
	width:33%;
	aspect-ratio:2/1;

	background-color:var(--head-oog-wit-bg);
	background-image:radial-gradient(
		circle, 
		var(--head-oog-pupil-bg) calc(25% - .5px), 
		var(--clr-eye, var(--head-oog-iris-bg)) calc(25% + .5px) calc(55% - .5px), 
		transparent calc(25% + .5px)
	);
	background-size:80% 160%;
	background-position:center 80%;
	background-repeat:no-repeat;

	border-radius:50% / 20% 20% 80% 80%;
	box-shadow:0 .375em 0 var(--head-oog-shadow);

	transform:scaleX(var(--sc, 1)) rotate(var(--r, -5deg));
	transition:var(--head-time-mood-change);
}

.head .eye + .eye {
	--sc:-1;
}


/* DE WENKBRAUWEN */
.head .eye::before {
	content:"";
	position:absolute;
	left:0; top:0;
	width:75%;
	aspect-ratio:15/4;
	
	background-color:var(--head-wenkbrouw-bg);
	border-radius:100% 0 20% 20% / 100% 50% 50% 0;
	transform:translate(var(--tx, 10%), var(--ty, -175%)) rotate(var(--r, -5deg));
	transition:var(--head-time-mood-change);
}

.head .eye + .eye::before {
	background-color: rgba(255 255 204 /.75);
}


/* DE HIGHLIGHTS */
/* container */
.head .⭐ {
	--maat:20%;
	--top:0%;

	--left:calc(var(--head-highlight-x-limit) + (100% - var(--head-highlight-x-limit) * 2) * var(--head-light-x, var(--head-light-x-default)));
	
	position:absolute;
	left:calc(var(--left) - var(--maat) / 2);
	top:var(--top);
	
	display:block;
	width:var(--maat);
	aspect-ratio:1/1;
	
	transition:
		top var(--head-time-mood-change), 
		transform var(--head-time-mood-change), 
		width var(--head-time-mood-change);
}

.head .eye + .eye .⭐ {
	left:calc(100% - var(--left) - var(--maat) / 2);
}

/* de actual highlight */
.head .⭐::after {
	content:"";
	position:absolute;
	inset:0;
	background-color:var(--head-highlight-bg);
	clip-path:polygon(50% 0, 61.2% 34.5%, 97.6% 34.5%, 68.2% 55.9%, 79.4% 90.4%, 50% 69%, 20.6% 90.4%, 31.8% 55.9%, 2.4% 34.5%, 38.8% 34.5%); /* ⭐ */
	animation:⭐ var(--head-highlight-time-rotate) infinite linear;
	transition:var(--head-time-mood-change);
}

.head .eye + .eye .⭐::after {
	animation-direction:reverse;
}


/***********/
/* DE NEUS */
/***********/

.head .nose {
	z-index:300;
	grid-area:1 / 1;
	transform:
		translateX(-5%)
		rotate(10deg)
		skew(-15deg, -5deg);

	width:25%;
	aspect-ratio:1/2;
	
	background-image:
		linear-gradient(
			67.5deg, 
			var(--head-neus-bg) calc(50% + .15em),
			transparent 0%
		);

	border-radius:10% 0 10% 50% / 50%;
	box-shadow:inset .25em -.25em 0 var(--head-neus-shadow);
}


/***********/
/* DE MOND */
/***********/

.head .mouth {
	z-index:700;

	width:10%;
	aspect-ratio:2/1;
	margin-bottom:1em;

	background-color:var(--head-mond-bg);
	border-radius:20% 80% 80% 20% / 40% 50% 50% 40%;
	
	transition:var(--head-time-mood-change);
}

/***********/
/* DE OREN */
/***********/

.head .ear {
	position: absolute;
	top:43%;
	
	width:8%;
	aspect-ratio:1/4;
	
	transform-origin:right center;
	transform:rotateZ(var(--r, -7.5deg)) scalex(1);
	
	appearance:none;
	background-color:inherit;
	border:none;
	border-radius:1em;
	outline:none;
	
	text-align:center;
}

.head .ear {
	right:98%;
}

.head .ear + .ear {
	--r:7.5deg;
	left:98%;
	transform-origin:left center;
}

@keyframes breathing {
	from {
		transform: scale(1);
	}

	to {
		transform: scale(1.5);
	}
}

</style>