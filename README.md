# font-resize
####自适应字体大小
 * vm:Viewport单位，1vm相当于屏幕宽度的百分之一；
 * calc:css中动态计算数值；
 
#####用rem定义字体

	$min-font-size:1.4rem;
	$max-font-size:1.8rem;
	$min-screen:600px;
	$max-screen:1200px;
	:root{
		font-size:10px;
	}
	
#####媒体查询
* add 取各个媒体属性的并集
* not 对整个媒体属性(不少于一个)进行 取反
* all 对指定的媒体类型应用指定样式
*  , 逗号分隔符/ 类似于or,每一个媒体属性都是独立不影响的 
*  only 防止老旧的浏览器不支持带媒体属性的查询而 用给定的样式
	
	`@media (min-width:600px) add (max-width:1800px){
		....
	}`
  
	`<link rel="stylesheet" media="(min-width:800px)" href="example.css"/>`
	
