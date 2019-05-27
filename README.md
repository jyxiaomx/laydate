# laydate
laydate  自定义小时、分钟范围  
有项目需求，需要定义小时范围，如早上8点到晚上21点；定义分钟范围，5的倍数  
网上查阅，发现都是些不彻底解决的方法，故重写LAYDATE源码，彻底解决  
使用说明：  
只需在初始化LAYDATE时，传入hourArray、minuteArray变量即可  
部分代码片段：  
laydate.render({  
      &nbsp;&nbsp;&nbsp;&nbsp;type: 'time',  
      &nbsp;&nbsp;&nbsp;&nbsp;btns: ['confirm'],  
      &nbsp;&nbsp;&nbsp;&nbsp;range: '~',  
      &nbsp;&nbsp;&nbsp;&nbsp;format: 'HH:mm',  
      &nbsp;&nbsp;&nbsp;&nbsp;hourArray:[8,9,10,11,12,13,14,15,16,17,18,19,20,21,22],  
      &nbsp;&nbsp;&nbsp;&nbsp;minuteArray:[0,30]  
});  
