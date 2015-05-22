# moment.js

---

一个轻量级的Javascript日期处理类库,不依赖任何第三方库,更多有关moment.js的介绍，请访问项目官网：http://momentjs.com/

---

## 格式化日期

当前时间：
 
	moment().format('YYYY-MM-DD HH:mm:ss'); //2014-09-24 23:36:09 

今天是星期几：

	moment().format('d'); //3 

转换当前时间的Unix时间戳：

	moment().format('X'); 

##相对时间

2015-05-22 22:34:10相对当前日期是
 
	moment("2015-05-22 22:34:10").fromNow(); 

7天后的日期：

	moment().add('days',7).format('YYYY年MM月DD日'); //2014年10月01日 

9小时后的时间：

	moment().add('hours',9).format('HH:mm:ss'); 


moment.js提供了丰富的说明文档，使用它还可以创建日历项目等复杂的日期时间应用。我们日常开发中最常用的是格式化时间，下面我把常用的格式制作成表格说明供有需要的朋友查看：

<table class="main_table" border="0" cellspacing="0" cellpadding="0" width="100%">
    <tbody>
        <tr class="table_title">
            <td width="15%">格式代码</td>
            <td>说明</td>
            <td width="35%">返回值例子</td>
        </tr>
        <tr>
            <td align="center">M</td>
            <td>数字表示的月份，没有前导零</td>
            <td>1到12</td>
        </tr>
        <tr>
            <td align="center">MM</td>
            <td>数字表示的月份，有前导零</td>
            <td>01到12</td>
        </tr>
        <tr>
            <td align="center">MMM</td>
            <td>三个字母缩写表示的月份</td>
            <td>Jan到Dec</td>
        </tr>
        <tr>
            <td align="center">MMMM</td>
            <td>月份，完整的文本格式</td>
            <td>January到December</td>
        </tr>
        <tr>
            <td align="center">Q</td>
            <td>季度</td>
            <td>1到4</td>
        </tr>
        <tr>
            <td align="center">D</td>
            <td>月份中的第几天，没有前导零</td>
            <td>1到31</td>
        </tr>
        <tr>
            <td align="center">DD</td>
            <td>月份中的第几天，有前导零</td>
            <td>01到31</td>
        </tr>
        <tr>
            <td align="center">d</td>
            <td>星期中的第几天，数字表示</td>
            <td>0到6，0表示周日，6表示周六</td>
        </tr>
        <tr>
            <td align="center">ddd</td>
            <td>三个字母表示星期中的第几天</td>
            <td>Sun到Sat</td>
        </tr>
        <tr>
            <td align="center">dddd</td>
            <td>星期几，完整的星期文本</td>
            <td>从Sunday到Saturday</td>
        </tr>
        <tr>
            <td align="center">w</td>
            <td>年份中的第几周</td>
            <td>如42：表示第42周</td>
        </tr>
        <tr>
            <td align="center">YYYY</td>
            <td>四位数字完整表示的年份</td>
            <td>如：2014 或 2000</td>
        </tr>
        <tr>
            <td align="center">YY</td>
            <td>两位数字表示的年份</td>
            <td>如：14 或 98</td>
        </tr>
        <tr>
            <td align="center">A</td>
            <td>大写的AM PM</td>
            <td>AM PM</td>
        </tr>
        <tr>
            <td align="center">a</td>
            <td>小写的am pm</td>
            <td>am pm</td>
        </tr>
        <tr>
            <td align="center">HH</td>
            <td>小时，24小时制，有前导零</td>
            <td>00到23</td>
        </tr>
        <tr>
            <td align="center">H</td>
            <td>小时，24小时制，无前导零</td>
            <td>0到23</td>
        </tr>
        <tr>
            <td align="center">hh</td>
            <td>小时，12小时制，有前导零</td>
            <td>00到12</td>
        </tr>
        <tr>
            <td align="center">h</td>
            <td>小时，12小时制，无前导零</td>
            <td>0到12</td>
        </tr>
        <tr>
            <td align="center">m</td>
            <td>没有前导零的分钟数</td>
            <td>0到59</td>
        </tr>
        <tr>
            <td align="center">mm</td>
            <td>有前导零的分钟数</td>
            <td>00到59</td>
        </tr>
        <tr>
            <td align="center">s</td>
            <td>没有前导零的秒数</td>
            <td>1到59</td>
        </tr>
        <tr>
            <td align="center">ss</td>
            <td>有前导零的描述</td>
            <td>01到59</td>
        </tr>
        <tr>
            <td align="center">X</td>
            <td>Unix时间戳</td>
            <td>1411572969</td>
        </tr>
	</tbody>
</table>