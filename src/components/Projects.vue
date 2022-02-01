<template>
  <section id="Projects">
    <br><br><br>
      <div class="projectheading">Projects</div>
      <link href="https://fonts.googleapis.com/css?family=Lato|Montserrat" rel="stylesheet">

<div class="projectscontainer">
	<ul class="projectList">
		
		<li>
			<div class="projectWrap">
				<div class="inner">
					<div class="project">
						<div class="innerWrap">
							<div class="image" style="background-image:url(https://images.unsplash.com/photo-1456894332557-b03dc5cf60d5?ixlib=rb-0.3.5&q=80&fm=jpg&crop=entropy&s=29a9bb29bcbf19a5954d0110b19d5b51);"></div>
							<div class="metaWrap">
								<div class="meta">
									<h5>Calculator</h5>
									<p class="label">Web Design & Web development</p>
                  <a href="https://github.com/CraigBraaf/Cal-v2" target="_blank"><button id="da-btn" class="btn btn-secondary" type="button">Github</button></a>
                <a href="https://modest-jepsen-572175.netlify.app/" target="_blank"><button id="da-womb" class="btn btn-secondary" type="button">Netlify</button></a>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</li>
		
		<li>
			<div class="projectWrap">
				<div class="inner">
					<div class="project">
						<div class="innerWrap">
							<div class="image" style="background-image:url(../assets/pos.pngz);"></div>
							<div class="metaWrap">
								<div class="meta">
									<h5>POS Website</h5>
									<p class="label">Design & development</p>
									<div class="buttonalign">
                  <a href="https://github.com/CraigBraaf/POS-Project" target="_blank"><button id="da-btn" class="btn btn-secondary" type="button">Github</button></a>
                <a href="https://app.netlify.com/sites/posprojectcraigbraaf/overview" target="_blank"><button id="da-womb" class="btn btn-secondary" type="button">Netlify</button></a></div>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</li>
		
		<li>
			<div class="projectWrap">
				<div class="inner">
					<div class="project">
						<div class="innerWrap">
							<div class="image" style="background-image:url(https://images.unsplash.com/reserve/unsplash_52ce2b0530dab_1.JPG?ixlib=rb-0.3.5&q=80&fm=jpg&crop=entropy&s=fbc452cf6c1d6921779ef531f2e53c0d);"></div>
							<div class="metaWrap">
								<div class="meta">
									<h5>dsad</h5>
									<p class="label">Design & development</p>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</li>
		
		<li>
			<div class="projectWrap">
				<div class="inner">
					<div class="project">
						<div class="innerWrap">
							<div class="image" style="background-image:url(https://images.unsplash.com/photo-1463123081488-789f998ac9c4?ixlib=rb-0.3.5&q=80&fm=jpg&crop=entropy&s=6d1a6d1c5a7eb63d0c411b1d019f0b30);"></div>
							<div class="metaWrap">
								<div class="meta">
									<h5>Project name</h5>
									<p class="label">Design & development</p>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</li>
		
	</ul>
</div>
      </section>
</template>

<script>

</script>

<style>

 #Projects {
    background-color:  rgb(95, 93, 93);
    height: 100vh;
  }

body {
	margin:0;
	padding:0;
}

h1, h2, h3, h4, h5, h6 {
	font-family:'Montserrat', sans-serif;
}

h1, h2, h3, h4, h5, h6, p {
	margin:0;
	padding:0;
	float:left;
}

h5 {
	width:100%;
	text-align:center;
	font-size:15px;
	font-weight:400;
	line-height:20px;
  color: white;
}

p {
	font-size:13px;
	font-weight:500;
}

p.label {
	width:100%;
	text-align:center;
	color:#80919b;
	font-size:12px;
	line-height:20px;
}

.container {
	width:100%;
	max-width:1200px;
	float:left;
}

.projectList {
	width:100%;
	float:left;
	list-style:none;
	margin:0;
	padding:10px;
}

.projectList li {
	width:25%;
	float:left;
}

@media only screen and (max-width:1023px) {
	.projectList li {
		width:33.333%;
	}
}

@media only screen and (max-width:779px) {
	.projectList li {
		width:50%;
	}
}

@media only screen and (max-width:539px) {
	.projectList li {
		width:100%;
	}
}

.projectList li .projectWrap {
	width:100%;
	float:left;
	padding:100% 0 0 0;
	position:relative;
}

.projectList li .projectWrap .inner {
	width:100%;
	height:100%;
	position:absolute;
	top:0;
	left:0;
	padding:10px;
	overflow:hidden;
}

.projectList li .projectWrap .inner .project {
	width:100%;
	height:100%;
	float:left;
	background:#fff;
	border-radius:5px;
	box-shadow:0px 2px 4px 1px rgba(56,72,84,0.1);
	padding:10px;
	position:relative;
	overflow:hidden;
	cursor:pointer;
	
	transition:transform 0.3s ease, box-shadow 0.3s ease;
}

.projectList li .projectWrap .inner .project .innerWrap {
	width:100%;
	height:100%;
	float:left;
	position:relative;
	overflow:hidden;
	border-radius:1px;
	-webkit-mask-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAIAAACQd1PeAAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAA5JREFUeNpiYGBgAAgwAAAEAAGbA+oJAAAAAElFTkSuQmCC);
}

.projectList li .projectWrap .inner .project .innerWrap .image {
	width:100%;
	height:100%;
	float:left;
	position:relative;
	border-radius:1px;
	background-size:cover;
	background-position:center center;
	background-repeat:no-repeat;
	
	
	transition:transform 0.3s ease;
}

.projectList li .projectWrap .inner .project .innerWrap .image:before {
	content:'';
	width:100%;
	height:100%;
	position:absolute;
	border-radius:1px;
	top:0;
	left:0;
	z-index:1;
	background:rgba(56,72,84,0.5);
	opacity:0;
	
	transition:opacity 0.3s ease;
}

.projectList li .projectWrap .inner .project .innerWrap .metaWrap {
	width:100%;
	height:100px;
	position:absolute;
	bottom:0;
	left:0;
	z-index:2;
	padding:0 10px 10px;
	transform:translate3d(0px,20px,0px);
	opacity:0;
	
	transition:transform 0.3s ease, opacity 0.3s ease;
}

.projectList li .projectWrap .inner .project .innerWrap .meta {
	width:100%;
	height:100%;
	background:rgba(255,255,255,1.0);
	
	display:flex;
	flex-direction:column;
	justify-content:center;
}

.projectList li .projectWrap .inner .project:hover {
	transform:translate3d(0px,-5px,0px);
	box-shadow:0px 5px 8px 3px rgba(56,72,84,0.2);
}

.projectList li .projectWrap .inner .project:hover .image {
	transform:scale(1);
}

.projectList li .projectWrap .inner .project:hover .image:before {
	opacity:1;
}

.projectList li .projectWrap .inner .project:hover .metaWrap {
	transform:translate3d(0px,0px,0px);
	opacity:1;
}

.projectList li .projectWrap .inner .project:hover .meta h5 {
	transform:scale(1);
}

.projectheading {
  font-size: 50px;
  color: white;
  font-weight: 20px;
}

.buttonalign {
	display: flex;
	margin-left: 25%;
}
</style>