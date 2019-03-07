---
layout: post
title:  "Markdowm learning notes"
date:   2019-03-06
categories: markdown
tags: markdown
excerpt: Markdown的学习笔记
---

* content
{:toc}
# 基本语法  
- - -
**标题**  
>markdown支持两种形式的标题，setext和atx.  
>setext:  只有两级标题(任意个 = 和 - )  
>     This is H1      
>     =======  
>	 This is H2  
>     ------------  
>	 atx: 可分六级标题  
>	 # This is H1  
>	 ## This is H2  
>	 ###### This is H6   

- - -    
**换行**    
>markdown中的换行方式有多种：
> 两个及以上的空格 + 回车   
> &lt;br&gt; 标签  

- - -  
**转义**   
<table border = "-1" width = "100%">
	<caption> Markdown 特殊字符转义 </caption>
	<thead>
		<tr>
			<th> 字符 </th>
			<th> 描述 </th>
			<th> 实体名称 </th>
			<th> 实体编号 </th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>  </td>
			<td> 空格 </td>
			<td> &amp;nbsp; </td>
			<td> &amp;#160; </td>
		</tr>
		<tr>
			<td> &lt; </td>
			<td> 左尖括号 </td>
			<td> &amp;lt; </td>
			<td> &amp;#60; </td>
		</tr>
		<tr>
			<td> &gt; </td>
			<td> 右尖括号 </td>
			<td> &amp;gt; </td>
			<td> &amp;#62; </td>
		</tr>
		<tr>
			<td> &amp; </td>
			<td>   </td>
			<td> &amp;amp; </td>
			<td> &amp;#38; </td>
		</tr>
		<tr>
			<td> &quot; </td>
			<td> 双引号 </td>
			<td> &amp;quot; </td>
			<td> &amp;#34; </td>
		</tr>
		<tr>
			<td> &apos; </td>
			<td> 单引号 </td>
			<td> &amp;apos; </td>
			<td> &amp;#39; </td>
		</tr>
	</tbody>
	<thead align = "middle">
		<tr>
			<th colspan = "4"> 反斜杠"\"转义 </th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td> \ </td>
			<td> backslash </td>
			<td>  </td>
			<td>   </td>
		</tr>
		<tr>
			<td> ` </td>
			<td> backtick </td>
			<td>   </td>
			<td>   </td>
		</tr>
		<tr>
			<td> * </td>
			<td> asterisk </td>
			<td>   </td>
			<td>   </td>
		</tr>
		<tr>
			<td> _ </td>
			<td> underscore </td>
			<td>   </td>
			<td>   </td>
		</tr>
		<tr>
			<td> {} </td>
			<td> curly braces </td>
			<td>   </td>
			<td>   </td>
		</tr>
		<tr>
			<td> [] </td>
			<td> square brackets </td>
			<td>   </td>
			<td>   </td>
		</tr>
		<tr>
			<td> () </td>
			<td> parentheses </td>
			<td>   </td>
			<td>   </td>
		</tr>
		<tr>
			<td> # </td>
			<td> hash mark </td>
			<td>   </td>
			<td>   </td>
		</tr>
		<tr>
			<td> + </td>
			<td> plus sign </td>
			<td>   </td>
			<td>   </td>
		</tr>
		<tr>
			<td> - </td>
			<td> minus sign (hyphen) </td>
			<td>   </td>
			<td>   </td>
		</tr>
		<tr>
			<td> . </td>
			<td> dot </td>
			<td>   </td>
			<td>   </td>
		</tr>
		<tr>
			<td> ! </td>
			<td> exclamation mark </td>
			<td>   </td>
			<td>   </td>
		</tr>
	</tbody> 
</table>
 
- - -
**水平线**  
> 三个以上连续的星号（*）、连字符（-）或下划线（_) 会在当前位置生成一个&lt;hr /&gt;标签，即一根水平线    

- - -
**链接&引用**    
> 内联链接：  
> 　　`This is [an example](http://example.com/ "Title") inline link.`>  
> 　　中括号内为显示的链接信息，后接的圆括号内为链接地址，双引号（或单引号或圆括号）内的为可选链接标题。  
> 自动链接：  
> 　　Markdown 支持一种 "自动" 创建 URL 和 email 地址链接的简短形式: 只需用尖括号包围 URL 或 email 地址即可，如：  
> 　　`<https://www.google.com.hk/>`  
> 引用：　  
> 　　`[Google]: https://www.google.com.hk/ "google"`  
>  　　在文档的任意位置，可以像上面一样定义链接标签，需要单独占一行。其中中括号内为链接标识符；后接一个冒号；跟着是链接URL（URL可用<>包围）；最后是可选的链接标题，可用单引号、双引号或圆括号包围。  
>  　  引用时的写法：[接标签]`[Google]`或[链接文本][链接标签]`[Gooooooogle][Google]`
  
- - -          
**强调**     
<table width = "100%">  
	<thead>
		<tr>
			<th> markdown </th>
			<th> html </th>
			<th> 效果 </th>
		</tr>
	</thead>
	<tbody align = "middle">
		<tr>
			<td> *single asterisks* </td>
			<td> &lt;em&gt; single asterisks &lt;/em&gt; </td>
			<td> <em> single asterisks </em> </td>
		</tr>
		<tr>
			<td> _single underscores_ </td>
			<td> &lt;em&gt;signal underscores&lt;/em&gt; </td>
			<td> <em> single underscores </em> </td>
		</tr>
		<tr>
			<td> **single underscores** </td>
			<td> &lt;strong&gt;double underscores&lt;/strong&gt; </td>
			<td> <strong> single underscores </strong> </td>
		</tr>
		<tr>
			<td> __double underscores__ </td>
			<td> &lt;strong&gt;signal underscores&lt;/strong&gt; </td>
			<td> <strong> single underscores </strong> </td>
		</tr>
	</tbody>
</table>  
- - -   

**图片**  
>Markdown 采用类似链接的语法来插入图片，包含两种形式： **内联** 和 **引用**  
>    
> 内联图片语法如下：  
> 　　`![Alt text](path/to/img.jpg)`    
> 即：
> <ol>
> <li> 一个感叹号 </li>
> <li> 紧跟着一个方括号，方括号内为图片的Alt属性 </li>
> <li> 紧跟着一对圆括号, 包含了图片的 URL 或者路径, 以及一个可选的用单引号或双引号包裹的 title 属性. </li>
> </ol>
> 引用图片的语法如下：  
> 　　`![Alt text][id]`  
> "id" 是图片引用的名称. 图片引用使用链接定义的相同语法:  
>　　`[id]: url/to/img.jpg "Optional title attribute"`  
> ![Hot Air Balloon](/../image/1.jpg "Hot Air Balloon") ![hot air balloon][2]     
>Tip: 以这种方式仅仅只能在页面中插入图片，不能设置图片的更多属性，若要为图片设置更多属性，需要使用html中的标签。  

[2]: /../image/2.png "Hot Air Balloon"


 
参考网页：
[Markdown 文档](https://markdown-zh.readthedocs.io/en/latest/ (Markdown 中文文档))
              
           
                   
  
