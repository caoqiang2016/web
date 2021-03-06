参考网址：http://www.runoob.com/regexp/regexp-metachar.html

###模式
1. g:global-全局
2. i:case-insenstive-不区分大小写
3. m:multiline-多行

###方括号
1. [abc]	查找方括号之间的任何字符
1. [^abc]	查找任何不在方括号之间的字符
1. [0-9]	查找任何从 0 至 9 的数字
1. [a-z]	查找任何从小写 a 到小写 z 的字符
1. [A-Z]	查找任何从大写 A 到大写 Z 的字符
1. [A-z]	查找任何从大写 A 到小写 z 的字符
1. [adgk]	查找给定集合内的任何字符
1. [^adgk]	查找给定集合外的任何字符
1. (red|blue|green)	查找任何指定的选项

###量词
1. n+	匹配任何包含至少一个 n 的字符串
1. n*	匹配任何包含零个或多个 n 的字符串
1. n?	匹配任何包含零个或一个 n 的字符串
1. n{X}	匹配包含 X 个 n 的序列的字符串
1. n{X,Y}	匹配包含 X 或 Y 个 n 的序列的字符串
1. n{X,}	匹配包含至少 X 个 n 的序列的字符串
1. n$	匹配任何结尾为 n 的字符串
1. ^n	匹配任何开头为 n 的字符串
1. ?=n	匹配任何其后紧接指定字符串 n 的字符串
1. ?!n	匹配任何其后没有紧接指定字符串 n 的字符串

###构造函数属性
1. input
2. lastMatch
3. lastParen
4. lastContext
5. multiline
6. rightContext

###实例方法
1. compile	编译正则表达式
2. exec	检索字符串中指定的值返回找到的值，并确定其位置
3. test	检索字符串中指定的值返回 true 或 false

###实例属性
1. global:全局
2. ignoreCase:不区分大小写
3. lastIndex:搜索下一个匹配项的字符位置
4. multiline:是否设置多行
5. source:正则表达式字符串，如/\[bc\]at/为'\\[bc\\]at'

###字符串方法
1. search:检索与正则表达式相匹配的值
2. match:找到一个或多个正则表达式的匹配
3. replace:替换与正则表达式匹配的子串
4. split:把字符串分割为字符串数组

###match与exec区别
1. exec:返回[返回第一次匹配字符串,匹配组,匹配位置,全部字符串]
2. match:返回所有匹配结果,可以返回捕获和匹配组结果,如果是全局查找，
不会返回匹配组结果