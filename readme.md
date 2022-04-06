滚动：

1、回到顶部
//平滑滚动到哪里 
window.scrollTo({ 
    top: 100, 
    left: 0, 
    behavior: 'smooth'  //平滑滚动
 })
 
 //平滑滚动多少
window.scrollBy({ 
    top: window.innerHeight, 
    left: 0, 
    behavior: 'smooth' 
})

2、FullPage滚动（全屏滚动，不用鼠标 用上下键滚动）

window.onkeydown = function(e) {console.log(e)  //先定义执行摁下键盘键
e.preventDefault()  //因为上下键本身自带含义，先需要取消上下键的默认属性，再才按照设定的滚动方式来实行
