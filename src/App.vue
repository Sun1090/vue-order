<template>
	<div id="app">
		<SideBar></SideBar>

		<div id="content">

			<div>
				
				<router-view></router-view>
          <ul class="boxList">
          <Menu-List>
            <img src="https://s1.ax1x.com/2018/12/10/FGhm2F.jpg" alt="" slot="imgsrc">
            <span slot="tilte">可乐鸡翅</span>
            <strong slot="price">22/份</strong>
          </Menu-List>
          <Menu-List>
            <img src="https://s1.ax1x.com/2018/12/10/FGhKKJ.jpg" alt="" slot="imgsrc">
            <span slot="tilte">红烧排骨</span>
            <strong slot="price">48/份</strong>
          </Menu-List>
          <Menu-List>
            <img src="https://s1.ax1x.com/2018/12/10/FGhnv4.jpg" alt="" slot="imgsrc">
            <span slot="tilte">糖醋里脊</span>
            <strong slot="price">48/份</strong>
          </Menu-List>
           <Menu-List>
            <img src="https://s1.ax1x.com/2018/12/10/FGhMr9.jpg" alt="" slot="imgsrc">
            <span slot="tilte">水煮鱼</span>
            <strong slot="price">48/份</strong>
          </Menu-List>
        </ul>
			</div>
		</div>
	</div>
</template>
/* {name:'可乐鸡翅',price:'22',classify:'热菜',img:'https://s1.ax1x.com/2018/12/10/FGhm2F.jpg'},
	{name:'红烧排骨',price:'48',classify:'热菜',img:'https://s1.ax1x.com/2018/12/10/FGhKKJ.jpg'},
	{name:'糖醋里脊',price:'30',classify:'热菜',img:'https://s1.ax1x.com/2018/12/10/FGhnv4.jpg'},
	{name:'水煮鱼',price:'39',classify:'热菜',img:'https://s1.ax1x.com/2018/12/10/FGhMr9.jpg'},
	{name:'蕨根粉',price:'15',classify:'凉菜',img:'https://s1.ax1x.com/2018/12/10/FGhQbR.jpg'},
	{name:'手撕鸡',price:'22',classify:'凉菜',img:'https://s1.ax1x.com/2018/12/10/FGh1V1.jpg'},
	{name:'蓝莓山药',price:'18',classify:'凉菜',img:'https://s1.ax1x.com/2018/12/10/FGhe8U.jpg'},
	{name:'可口可乐',price:'5',classify:'饮料',img:'https://s1.ax1x.com/2018/12/14/FUpzfx.jpg'},
	{name:'酸辣汤',price:'14',classify:'汤',img:'https://s1.ax1x.com/2018/12/14/FUpH6U.jpg'},
	{name:'啤酒',price:'12',classify:'其它',img:'https://s1.ax1x.com/2018/12/14/FUpTpV.jpg'}, */
<script>
	import SideBar from './components/SideBar'
import MenuList from './components/MenuList'
	export default {
		components:{	//导入进来的组件要放到components里面
			SideBar,MenuList
		}
	}
</script>

<style>
body,p{
	margin: 0;
}
body{
	background: url(./assets/images/bg.jpg) center top no-repeat;
}
ul{
	margin: 0;
	padding: 0;
	list-style: none;
}
a{
	text-decoration: none;
}

#app{
	display: flex;
	width: 100%;
}
.logo{
	height: 120px;
}
#content{
	width: 100%;
	position: relative;
}
</style>
