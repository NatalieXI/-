# RegExp对象
1. 获取URL中值(index.htm?参数1=数值1&参数2=数值2&......)
```
		getvl : function(name) {
			var reg = new RegExp("(^|\\?|&)" + name + "=([^&]*)(\\s|&|$)", "i");
			if (reg.test(location.href)) {
				return unescape(RegExp.$2.replace(/\+/g, " "));
			} else {
				return "";
			}
		}
```		
|修饰符	 |   描述      |
|--------|-----------------------------|
|i       	|执行对大小写不敏感的匹配。|
|g       	|执行全局匹配（查找所有匹配而非在找到第一个匹配后停止）。|
|m        	|执行多行匹配。|

2. 总结：正则表达式的用途（校验、替换、定位搜索）。
