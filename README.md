# jquery-tableLottery
这是一个九宫格抽奖插件。自己造的轮子，贴出源代码跟大家交流一下。
配置参数：
~~~javascript
 self.def={
        html:'',    // 抽奖效果，添加HTML标签
        hoverClass:'',  // 抽奖效果，在TD添加样式
        startTime:50,  //起始延迟时间
        onlyTime:2,     //延迟时间间隔
        endTime:500,    //最后出结果的延迟时间
        id:'',          //抽奖按钮ID，JQ选择器语法
        way:'click',    //按钮绑定的事件，默认点击事件
        cycle:3,        //九宫格循环次数
        start:5,        //九宫格起始位置
        arr:[0,1,2,5,8,7,6,3],  //九宫格循环方向，默认顺时针
        runBefor:function(){    //抽奖之前的函数，返回中奖位置，默认为第一格，返回false结束抽奖
            return 0;
        },
        callBack:function(i){   //抽奖之后的回调函数
//                alert(i);
        }
    };
~~~
## html配置
因为每个活动的UI效果都不一样，所以只要求是3*3的table九宫格就行，[点击这里看DEMO][1]。

[1]: [https://codepen.io/FreadChen/pen/WZrQOG]
