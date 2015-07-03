## string类型
#1,charCodeAt方法，返回一个整数，代表制定位置字符的Unicode编码
example：
    var str="ABC";
    str.charCodeAt(0);
    ==>65

# 2,formCharCode方法，从一些unicode字符串中返回一个字符串
    string.formCharCode(code,code2...)
example:
    string.formCharCode(65,66,112);
    ==>ABp

# 3,charAt方法返回指定位置处的字符，如果超出范围返回空字符串
    objObject.charAt(index)
example:
    var str="ABC";
    str.charAt(1);
    ==>B

# 4,slice方法,返回字符串片段
    strObj.slice(start[,end])
说明：
start下标从0开始的strObj指定部分其实索引。
如果start为负，将它作为length+start处理，此处length为字符串的长度。
end小标从0开始的strObj指定部分结束索引。
如果end为负，将它作为length+end处理，此处length为字符串的长度。
example:
    var str="abcdefghijk";
    str.slice(2,4);
    ==>cd
    str.slice(-5,8);//此处起始位置为:-5+11=6
    ==>gh

# 5,substring方法,返回string对象中指定位置的字符串
    strObj.string(start,end)
说明:
start指明字符串起始位置，索引从0开始计算
end指明字符串结束位置，索引从0开始计算
substring方法使用start,end数值较小的作为子字符串的起始位置,
如果start或者end为NAN或者负数,那么将其替换为0
example:
    var str="abcdefghijk";
    str.substring(2,4);
    ==>cd
    str.substring(4,2);
    ==>cd

# 6,substr方法,返回一个从指定位置开始的指定长度的字符串
    strObj.substr(start,[length])
说明:
start为子字符串起始的位置,索引从0开始，如果start为负数,则从length-1开始往回数
lenght在返回的子字符串中应包括的字符个数

example:
    var str="abcdefghijk";
    str.substr(0,2);
    ==>ab
    str.substr(-2,2);
    ==>jk

# 7,indexOf方法返回字符在string对象中中第一次出现子字符串的位置
如果没有找到子字符串，则返回-1;
    strObj.indexOf(subStr,[,startIndex])
说明:
subStr是要在string对象中查找的子字符串
startIndex整数值指出在string对象内开始查询的索引，如果忽略，则从字符串开始处开始查找
example:
    var str="abcdefghijk";
    str.indexOf("abc");
    ==>0
    str.indexOf("abc",5);
    ==>-1


# 8,lastIndexOf方法返回string对象中子字符串最后出现的位置
如果没有匹配到子字符串，则返回-1
    strObj.lastIndexOf(subStr[,startIndex])
说明:
subStr是要在string对象中查找的子字符串
startIndex整数值指出在string对象内开始查询的索引，如果忽略，则从字符串开始处末尾查找
example:
    var str="aabbccddeeff";
    srt.lastIndexOf("a");
    ==>1


# 9,search()方法返回与正则表达式查找内容匹配的第一个字符串的位置
    strObj.search(reExp)
说明：
reExp包含正则表达式模式和可用标志的正则表达式对象。
example:
    var str = "ABCDECDF";
    str.search("CD"); // 或 str.search(/CD/i);
    ==>2

# 10,concat方法返回字符串值，该值包好了两个或多个提供的字符串的链接
    str.concat(string1,string2.....)
说明：
string1，string2要和所有其他指定的字符串进行连接的String对象或文字。
example：
    var str = "ABCDEF";
    str.concat("ABCDEF","ABC");
    ==>ABCDEFABCDEFABC

# 11,split方法，将一个字符串分割为子字符串，然后将结果作为字符串数组返回
    strObj.split([separator[,limit]])
说明：
separator字符串或 正则表达式 对象，它标识了分隔字符串时使用的是一个还是多个字符。如果忽略该选项，返回包含整个字符串的单一元素数组。
limit该值用来限制返回数组中的元素个数。
example：
    var str = "AA BB CC DD EE FF";
    str.split(" ",3);
    ==>AA,BB,CC

# 12,toLowerCase方法返回一个字符串，该字符串中的字母被转换成小写。
example：
    var str = "ABCabc";
    str.toLowerCase();
    ==>abcabc
# 13,toUpperCase方法返回一个字符串，该字符串中的所有字母都被转换为大写字母。
example：
    var str = "ABCabc";
    str.toUpperCase();
    ==>ABCABC








