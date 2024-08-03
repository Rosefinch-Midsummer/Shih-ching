# 中文排版 heti

[赫蹏](https://sivan.github.io/heti/)

古代称用以书写的小幅绢帛。后亦以借指纸。《汉书·外戚传下·孝成赵皇后》：「武（籍武）发篋中，有裹药二枚，赫蹏书。」颜师古注：「邓展曰：『赫音兄弟鬩墙之鬩。』应劭曰：『赫蹏，薄小纸也。』」宋赵彦卫 《云麓漫钞》卷七：「《赵后传》所谓『赫蹏』者，注云『薄小纸』，然其寔亦縑帛。」


赫蹏（hètí）是专为中文网页内容设计的排版样式增强。它基于通行的中文排版规范，可为网站的读者带来更好的内容阅读体验。它的主要特性有：

<ul>
        <li>贴合网格的排版；</li>
        <li>全标签样式美化；</li>
        <li>预置古文、诗词样式；</li>
        <li>预置多种排版样式（行间注、多栏、竖排等）；</li>
        <li>多种预设字体族（仅限桌面端）；</li>
        <li>简/繁体中文支持；</li>
        <li>自适应黑暗模式；</li>
        <li>中西文混排美化，不再手敲空格（基于JavaScript脚本）；</li>
        <li>标点挤压（基于JavaScript脚本）；</li>
        <li>兼容<i>normalize.css</i>、<i>CSS Reset<sup><a id="ref-01" href="#fn-01">[1]</a></sup></i>等常见样式重置；</li>
        <li>移动端支持；</li>
        <li>……</li>
      </ul>
      <p>总之，用上就会变好看。</p>

注：赫蹏是正文区域的样式增强，不是normalize.css或CSS Reset的替代。因此不建议将它作用在根标签（如<body>或<div class="container">）上。

## 效果示例

本页面全页应用了赫蹏样式，所见即所得。下面是内置的多种排版效果演示。

### 古文

为容器元素`<div class="heti">`添加名为heti--ancient的class即可实现古文版式：

```html
<div class="heti heti--ancient">...</div>
```

### 诗词

诗词：为容器元素`<div class="heti">`添加名为heti--poetry的class实现诗词版式：

```html
<div class="heti heti--poetry">
  <h2>九月九日忆山东兄弟<span class="heti-meta heti-small">[唐]<abbr title="号摩诘居士">王维</abbr></span></h2>
  <p class="heti-x-large">
    独在异乡为异客<span class="heti-hang">，</span><br>
    每逢佳节倍思亲<span class="heti-hang">。</span><br>
    遥知兄弟登高处<span class="heti-hang">，</span><br>
    遍插茱萸少一人<span class="heti-hang">。</span>
  </p>
</div>
```

诗节：在古文版式`<div class="heti heti--ancient">`中，为诗句添加名为heti-verse的class可以将其居中显示：

```html
<div class="heti heti--ancient">
  <h2>一剪梅·红藕香残玉簟秋<span class="heti-meta heti-small">[宋]<abbr title="号易安居士">李清照</abbr></span></h2>
  <p class="heti-verse heti-x-large">
    红藕香残玉簟秋。轻解罗裳，独上兰舟<span class="heti-hang">。</span><br>
    云中谁寄锦书来，雁字回时，月满西楼<span class="heti-hang">。</span><br>
    花自飘零水自流。一种相思，两处闲愁<span class="heti-hang">。</span><br>
    此情无计可消除，才下眉头，却上心头<span class="heti-hang">。</span>
  </p>
</div>
```

搭配使用标点悬挂<span class="heti-hang">、元信息<span class="heti-meta heti-small">来丰富展示效果。

### 行间注

为容器元素`<div class="heti">`添加名为heti--annotation的class后，搭配`<ruby>`元素即可实现整齐的行间注效果：

```html
<div class="heti heti--annotation">...</div>
```

### 多栏排版

赫蹏预置了多种多栏布局类，可以按栏数或每栏行宽进行设置。

为容器元素`<div class="heti">`添加名为heti--columns-2的class即可实现双栏排版：

```html
<div class="heti heti--columns-2">...</div>
```

### 竖排排版

赫蹏预置了传统的竖排（直排）方向排版，同样贴合栅格。

为容器元素`<div class="heti">`添加名为heti--vertical的class即可实现竖排布局：

```html
<div class="heti heti--vertical">...</div>
```

 <h3 id="tags">标签示例表<a class="anchor" href="#tags"></a></h3>
      <details open>
        <summary>查看标签示例表</summary>
        <section class="section">
          <table>
            <caption>常用标签样式示例表</caption>
            <tr>
              <th style="width: 72px;">类型</th>
              <th style="width: 320px;">标签</th>
              <th style="width: 240px;">效果</th>
            </tr>
            <tr>
              <td>链接</td>
              <td><code>&lt;a href=&quot;https://github.com/sivan/heti&quot; title=&quot;赫蹏&quot;&gt;heti.css&lt;/a&gt;</code></td>
              <td><a href="https://github.com/sivan/heti" title="赫蹏">heti.css</a></td>
            </tr>
            <tr>
              <td>缩写</td>
              <td><code>&lt;abbr title=&quot;Cascading Style Sheets&quot;&gt;CSS&lt;/abbr&gt;</code></td>
              <td><abbr title="Cascading Style Sheets">CSS</abbr></td>
            </tr>
            <tr>
              <td>代码</td>
              <td><code>&lt;code&gt;.heti { star: 5; }&lt;/code&gt;</code></td>
              <td><code>.heti { star: 5; }</code></td>
            </tr>
            <tr>
              <td>专名号</td>
              <td><code>此时来自&lt;u title=&quot;位于山东省聊城市阳谷县城东&quot;&gt;景阳冈&lt;/u&gt;的&lt;u&gt;武松&lt;/u&gt;大喝一声：&lt;q&gt;纳命来！&lt;/q&gt;</code></td>
              <td>此时来自<u title="位于山东省聊城市阳谷县城东">景阳冈</u>的<u>武松</u>大喝一声：<q>纳命来！</q></td>
            </tr>
            <tr>
              <td>文本变动</td>
              <td><code>这次考试，我考了&lt;del datetime=&quot;17:00:00&quot;&gt;58&lt;/del&gt;&lt;ins datetime=&quot;18:15:00&quot;&gt;98&lt;/ins&gt;分呢！</code></td>
              <td>这次考试，我考了<del datetime="17:00:00">58</del><ins datetime="18:15:00">98</ins>分呢！</td>
            </tr>
            <tr>
              <td>文本更新</td>
              <td><code>因为谁也不认识，所以最后我们决定念&lt;s&gt;d&iacute;&lt;/s&gt;t&iacute;。</code></td>
              <td>因为谁也不认识，所以最后我们决定念<s>dí</s>tí。</td>
            </tr>
            <tr>
              <td>引号</td>
              <td><code>窃&middot;格瓦拉曾经说过：&lt;q&gt;打工是不可能打工的。&lt;/q&gt;</code></td>
              <td>窃·格瓦拉曾经说过：<q>打工是不可能打工的。</q></td>
            </tr>
            <tr>
              <td>术语</td>
              <td><code>&lt;dfn&gt;窃&middot;格瓦拉&lt;/dfn&gt;，中国大陆网络红人、罪犯。被奉为百度「戒赌吧」400万会员的「精神领袖」。</code></td>
              <td><dfn>窃·格瓦拉</dfn>，中国大陆网络红人、罪犯。被奉为百度「戒赌吧」400万会员的「精神领袖」。</td>
            </tr>
            <tr>
              <td>标记</td>
              <td><code>这道题&lt;mark&gt;必考&lt;/mark&gt;，你们爱记不记。</code></td>
              <td>这道题<mark>必考</mark>，你们爱记不记。</td>
            </tr>
            <tr>
              <td>强调</td>
              <td><code>稳住，&lt;em&gt;我们能赢&lt;/em&gt;！</code></td>
              <td>稳住，<em>我们能赢</em>！</td>
            </tr>
            <tr>
              <td>着重号</td>
              <td><code>我们&lt;span class=&quot;heti-em&quot;&gt;必将&lt;/span&gt;战胜这场疫情。</code></td>
              <td>我们<span class="heti-em">必将</span>战胜这场疫情。</td>
            </tr>
          </table>
        </section>
      </details>



# mdbook-template

添加目录块:

```toml
<!-- toc -->
```

# MdBook Github Action with Plugin Support

Coverage Security Rating Maintainability Rating Vulnerabilities GitHub license GitHub issues

## Introduction

This is an github action to set up the rust-lang/mdBook with some supported plugins.

This action runs only on linux and is well tested on github latest ubuntu runner and compatible with Node v14, v16 and v18. Windows and MacOS are currently not supported.

## Supported Plugins

Michael-F-Bryan/mdbook-linkcheck  
badboy/mdbook-mermaid  
badboy/mdbook-toc  
badboy/mdbook-open-on-gh  
tommilligan/mdbook-admonish  
lzanini/mdbook-katex  

## Fast Setup

The following example installs mdbook with all currently supported plugins with the latest version. Keep in mind that this build could break if mdbook or one of the plugins release new versions with breaking changes. Therefore it is highly recommended to specify a version. See "Advanced Setup" for more information.

```bash
name: Setup mdBook with plugins (latest)
on:
  push:
    branches:
      - main
jobs:
  run:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: jontze/action-mdbook@v2
        with:
          token: ${{secrets.GITHUB_TOKEN}}
          # Optional Plugins have to be enabled
          use-linkcheck: true
          use-mermaid: true
          use-toc: true
          use-opengh: true
          use-admonish: true
          use-katex: true
      - name: Show mdbook version
        run: mdbook --version
      - name: Show linkchecker version
        run: mdbook-linkcheck --version
      - name: Show mermaid version
        run: mdbook-mermaid --version
      - name: Show toc version
        run: mdbook-toc --version
      - name: Show open-on-gh version
        run: mdbook-open-on-gh --version
      - name: Show admonish version
        run: mdbook-admonish --version
      - name: Show katex version
        run: mdbook-katex --version
```

## Advanced Setup

```bash
name: Setup mdBook wth plugins (version)
on:
  push:
    branches:
      - main
jobs:
  run:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: jontze/action-mdbook@v2
        with:
          token: ${{secrets.GITHUB_TOKEN}}
          # Optional Plugins have to be enabled with a version
          mdbook-version: "~0.3.0" # Use a semver compatible string
          use-linkcheck: true
          linkcheck-version: "~0.7.0"
          use-mermaid: true
          mermaid-version: "~0.8.0"
          use-toc: true
          toc-version: "~0.7.0"
          use-opengh: true
          opengh-version: "~2.0.0"
          use-admonish: true
          admonish-version: "~1.8.0"
          use-katex: true
          katex-version: "~0.2.17"
      - name: Show mdbook version
        run: mdbook --version
      - name: Show linkchecker version
        run: mdbook-linkcheck --version
      - name: Show mermaid version
        run: mdbook-mermaid --version
      - name: Show toc version
        run: mdbook-toc --version
      - name: Show open-on-gh version
        run: mdbook-open-on-gh --version
      - name: Show admonish version
        run: mdbook-admonish --version
      - name: Show katex version
        run: mdbook-katex --version
```

