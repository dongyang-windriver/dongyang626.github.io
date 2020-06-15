---


---

<hr>
<p>layout: post<br>
title: 1s 提升Git clone Github 速度<br>
subtitle: 简单、快速<br>
date: 2020-06-15<br>
author: Dongyang<br>
header-img: img/post-bg-cook.jpg<br>
catalog: true<br>
tags:</p>
<ul>
<li>Git</li>
</ul>
<hr>
<p>这类操作性质的文章网上很多，本来不想重复造轮子的。<br>
奈何很多方法，1费时间，2可能还不好用。<br>
所以还是写一下亲测简单又好用的方法（该方法来自知乎，文末会附链接）。</p>
<p>该方法只需一步：<br>
将clone地址中的 <a href="http://github.com">github.com</a> 替换为github的Mirror: <a href="http://github.com.cnpmjs.org">github.com.cnpmjs.org</a> 即可<br>
（该方法同样适用于对github网站的访问）<br>
Eg：你本来打算clone</p>
<blockquote>
<p>git clone <a href="https://github.com/dongyang626/dongyang626.github.io.git">https://github.com/dongyang626/dongyang626.github.io.git</a></p>
</blockquote>
<p>只需将地址改为：</p>
<blockquote>
<p>git clone <a href="https://github.com.cnpmjs.org/dongyang626/dongyang626.github.io.git">https://github.com.cnpmjs.org/dongyang626/dongyang626.github.io.git</a></p>
</blockquote>
<p>速度即可成倍提升 :)</p>
<p>注意：<br>
很多Git仓库，更偏向支持SSH方式clone， 像BitBucket已经不再支持HTTP的方式了，<br>
所以有些情况下使用HTTP可能会报错，网速没问题的尽量使用SSH方式。另，我对SSH中的github.com进行替换，发现会导致time<br>
out 无法clone（没有进一步调查该问题）。</p>
<p>知乎原文作者：Don.hub<br>
原文链接：<a href="https://www.zhihu.com/question/27159393/answer/1117219745">https://www.zhihu.com/question/27159393/answer/1117219745</a></p>
