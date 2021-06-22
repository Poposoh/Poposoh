- 👋 Hi, I’m @Poposoh
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Poposoh/Poposoh is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>计数器案例</title>
		<script src="js/vue.js" type="text/javascript" charset="UTF-8"></script>
		<style>
			#app {
				width: 300px;
				height: 50px;
				margin: 100px auto;
			}
			.content {
				width: 100%;
				height: 100%;
				border: 1px solid #CCCCCC;
				border-radius: 8px;
				overflow: hidden;
			}
			button {
				float: left;
				width: 100px;
				height: 100%;
				background-color: #ccc;
				color: #ad2a27;
				font-size: 30px;
				cursor: pointer;
				outline: none;
				border: none;
			}
			span {
				display: block;
				float: left;
				width: 100px;
				height: 100%;
				line-height: 50px;
				text-align: center;
				font-size: 30px;
				background-color: #fff;
				padding: 0;
			}
		</style>
	</head>
	<body>
		<div id="app">
			<div class="content">
				<button @click="sub">-</button>
				<span>{{ num }}</span>
				<button @click="add">+</button>				
			</div>
		</div>
		<script>
			var app = new Vue({
				el: "#app",
				data: {
					num: 1
				},
				methods: {
					add: function() {
						if(this.num < 10) {
							this.num++;
						} else {
							alert("别点了，已经最大了！");
						}
					},
					sub: function() {
						if(this.num > 1) {
							this.num--;
						} else {
							alert("别点了，已经最小了！");
						}
					}
				}
			})
		</script>
	</body>
</html>
