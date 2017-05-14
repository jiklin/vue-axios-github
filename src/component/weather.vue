<template>
	<div class="weather">
		<div id="tp-weather-widget"></div>
	</div>
</template>

<script>
	export default {
		mounted() {
			(function(T,h,i,n,k,P,a,g,e){g=function(){P=h.createElement(i);a=h.getElementsByTagName(i)[0];P.src=k;P.charset="utf-8";P.async=1;a.parentNode.insertBefore(P,a)};T["ThinkPageWeatherWidgetObject"]=n;T[n]||(T[n]=function(){(T[n].q=T[n].q||[]).push(arguments)});T[n].l=+new Date();if(T.attachEvent){T.attachEvent("onload",g)}else{T.addEventListener("load",g,false)}}(window,document,"script","tpwidget","//widget.seniverse.com/widget/chameleon.js"));
			tpwidget("init", {
			    "flavor": "slim",
			    "location": "WS10730EM8EV",
			    "geolocation": "enabled",
			    "language": "zh-chs",
			    "unit": "c",
			    "theme": "chameleon",
			    "container": "tp-weather-widget",
			    "bubble": "disabled",
			    "alarmType": "badge",
			    "color": "#FFFFFF",
			    "uid": "U93A7BFC3C",
			    "hash": "6900053376b919b8f95930499a420794"
			});
			tpwidget("show");
		}
	};
</script>

<style lang="sass">
	.weather { display: inline-block; margin-left: 200px }
</style>