##CN
<article class="markdown-body entry-content" itemprop="text"><p><trans data-src="Highcharts JS is a JavaScript charting library based on SVG, with fallbacks to VML and canvas for old browsers." data-dst="Highcharts JS是一个JavaScript图表库基于SVG，VML和帆布的回退到旧的浏览器。">Highcharts JS是一个JavaScript图表库基于SVG，VML和帆布的回退到旧的浏览器。</trans></p>

<p><em><trans data-src="For NPM users, please note that this module replaces the previous " data-dst="对于新用户，请注意，这个模块取代了以前的">对于新用户，请注意，这个模块取代了以前的</trans><a href="https://www.npmjs.com/package/highcharts-server"><trans data-src="Highcharts Server" data-dst="开发服务器">开发服务器</trans></a><trans data-src=" module." data-dst="模块">模块</trans></em></p>

<ul>
<li><trans data-src="Official website:  " data-dst="官方网站：">官方网站：</trans><a href="http://www.highcharts.com"><trans data-src="www.highcharts.com" data-dst="www.highcharts.com"><trans data-src="www.highcharts.com" data-dst="www.highcharts.com">www.highcharts.com</trans></trans></a></li>
<li><trans data-src="Download page: " data-dst="下载页面：">下载页面：</trans><a href="http://www.highcharts.com/download"><trans data-src="www.highcharts.com/download" data-dst="www.highcharts.com /下载">www.highcharts.com /下载</trans></a></li>
<li><trans data-src="Licensing: " data-dst="许可证贸易">许可证贸易</trans><a href="http://www.highcharts.com/license"><trans data-src="www.highcharts.com/license" data-dst="www.highcharts.com /许可证">www.highcharts.com /许可证</trans></a></li>
<li><trans data-src="Support: " data-dst="支持">支持</trans><a href="http://www.highcharts.com/support"><trans data-src="www.highcharts.com/support" data-dst="www.highcharts.com/support"><trans data-src="www.highcharts.com/support" data-dst="www.highcharts.com/support">www.highcharts.com/support</trans></trans></a></li>
<li><trans data-src="Issues " data-dst="问题">问题</trans><a href="/2947721120/highcharts/blob/master/repo-guidelines.md"><trans data-src="Repo guidelines" data-dst="回购指引" style="background: transparent;">回购指引</trans></a></li>
</ul>

<h2><a id="user-content-example-usage-in-nodebrowserifywebpack" class="anchor" href="#example-usage-in-nodebrowserifywebpack" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a><trans data-src="Example Usage in Node/Browserify/Webpack" data-dst="在节点/ browserify / WebPACK使用示例">在节点/ browserify / WebPACK使用示例</trans></h2>

<p><trans data-src="Please note that there are several ways to use Highcharts. For general installation instructions, see " data-dst="请注意，有使用HighCharts的几种方法。对于一般的安装说明，看" style="background: transparent;">请注意，有使用HighCharts的几种方法。对于一般的安装说明，看</trans><a href="http://www.highcharts.com/docs/getting-started/installation"><trans data-src="the docs" data-dst="文档" style="background: transparent;">文档</trans></a><trans data-src="." data-dst="。">。</trans></p>

<pre><code><trans data-src="npm install highcharts
" data-dst="NPM安装开发">NPM安装开发</trans></code></pre>

<div class="highlight highlight-source-js"><pre><span class="pl-c"><trans data-src="// Load Highcharts" data-dst="highcharts /负载">highcharts /负载</trans></span>
<span class="pl-k"><trans data-src="var" data-dst="VaR">VaR</trans></span><trans data-src=" Highcharts " data-dst="Highcharts">Highcharts</trans><span class="pl-k">=</span> <span class="pl-c1"><trans data-src="require" data-dst="要求">要求</trans></span><trans data-src="(" data-dst="（">（</trans><span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="highcharts" data-dst="Highcharts">Highcharts</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src=");

" data-dst="）；">）；</trans><span class="pl-c"><trans data-src="// Alternatively, this is how to load Highstock. Highmaps is similar." data-dst="/ /或者，这是如何加载highstock。highmaps相似。">/ /或者，这是如何加载highstock。highmaps相似。</trans></span>
<span class="pl-c">// var Highcharts = require('highcharts/highstock');</span>

<span class="pl-c"><trans data-src="// This is how a module is loaded. Pass in Highcharts as a parameter." data-dst="/这是怎样的一个模块加载。通过开发一个参数。">/这是怎样的一个模块加载。通过开发一个参数。</trans></span>
<span class="pl-c1"><trans data-src="require" data-dst="要求">要求</trans></span><trans data-src="(" data-dst="（">（</trans><span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="highcharts/modules/exporting" data-dst="Highcharts /模块/输出">Highcharts /模块/输出</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src=")(Highcharts);

" data-dst="）（highcharts）；">）（highcharts）；</trans><span class="pl-c"><trans data-src="// Generate the chart" data-dst="//生成图表">//生成图表</trans></span>
<span class="pl-smi"><trans data-src="Highcharts" data-dst="Highcharts"><trans data-src="Highcharts" data-dst="Highcharts">Highcharts</trans></trans></span><trans data-src="." data-dst="。">。</trans><span class="pl-en"><trans data-src="chart" data-dst="图表"><trans data-src="图表" data-dst="图表">图表</trans></trans></span><trans data-src="(" data-dst="（">（</trans><span class="pl-s"><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span><trans data-src="container" data-dst="容器">容器</trans><span class="pl-pds"><trans data-src="'" data-dst="'"><trans data-src="'" data-dst="'">'</trans></trans></span></span><trans data-src=", {
  " data-dst="，{">，{</trans><span class="pl-c"><trans data-src="// options - see http://api.highcharts.com/highcharts" data-dst="湖/选项/ highcharts api.highcharts.com http：／／">湖/选项/ highcharts api.highcharts.com http：／／</trans></span><trans data-src="
});" data-dst="}）；">}）；</trans></pre></div>
</article>
##EN
Highcharts JS is a JavaScript charting library based on SVG, with fallbacks to VML and canvas for old browsers.

_For NPM users, please note that this module replaces the previous [Highcharts Server](https://www.npmjs.com/package/highcharts-server) module._

* Official website:  [www.highcharts.com](http://www.highcharts.com)
* Download page: [www.highcharts.com/download](http://www.highcharts.com/download)
* Licensing: [www.highcharts.com/license](http://www.highcharts.com/license)
* Support: [www.highcharts.com/support](http://www.highcharts.com/support)
* Issues [Repo guidelines](repo-guidelines.md)

## Example Usage in Node/Browserify/Webpack
Please note that there are several ways to use Highcharts. For general installation instructions, see [the docs](http://www.highcharts.com/docs/getting-started/installation).

```
npm install highcharts
```

```js
// Load Highcharts
var Highcharts = require('highcharts');

// Alternatively, this is how to load Highstock. Highmaps is similar.
// var Highcharts = require('highcharts/highstock');

// This is how a module is loaded. Pass in Highcharts as a parameter.
require('highcharts/modules/exporting')(Highcharts);

// Generate the chart
Highcharts.chart('container', {
  // options - see http://api.highcharts.com/highcharts
});
```

