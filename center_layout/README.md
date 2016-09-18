## 5种未知元素宽高的水平垂直居中方法
*{
	margin: 0;
	padding: 0;
}
.parent{
	height: 500px;
	background-color: #999;
	width: 400px;
}
.child{
	background-color: #798;
	height: 100px;
	width: 100px;
}

/*假设是未知宽高的*/


/*方法一：position + margin*/
.case1_p{
	position: rela
	tive;
}
.case1_c{
	position: absolute;
	margin: auto;
	top: 0;
	left: 0;
	bottom: 0;
	right: 0;
}

/*方法二：display:table-cell*/
.case2_p{
	display: table-cell;
	vertical-align: middle;
	text-align: center;
}
.case2_c{
	display: inline-block;
}

/*方法三：position + transform*/
.case3_p{
	position: relative;
}
.case3_c{
	position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%,-50%);
}


/*方法四：flex*/
.case4_p{
	display: flex;
	justify-content: center;
	align-items: center;
}
.case4_c{
	
}


/*方法五： margin*/
.case5_p{
	overflow: hidden;
}
.case5_c{

	margin:50% auto; 
}
