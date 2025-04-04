---
title: "Blog"
layout: gridlay
sitemap: false
permalink: /blogs/
---

## Blogs

<div class="jumbotron">
### On this webpage

<ul>
    {% for post in site.posts %}
    <li>
      <u>{{ post.date | date: "%b. %-d, %Y" }}</u>: <a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}" target="_blank">{{ post.title}}</a> <br>
      {{ post.abstract }}
    </li>
  {% endfor %}
</ul>
</div>



<div class="jumbotron">
### Beyond this webpage

<ul>
    <li><u> Nov. 17, 2024</u>:
        <a href="https://qiita.com/naoki_condensed_matter/private/494305ef78b58a37ca6a" target="_blank">
        物理系外部院試体験記
    </a>  <br>
    広島大学から外部の大学院を受けたので、その体験談を書きました。
    他の体験記に書いていないけど重要なことを書いたつもりなので、外部の大学院受験を考えている人は是非参考にしてください。
    </li>
    <li>
        <u>Apr. 2024</u>:
        <a href="https://www2.kek.jp/ksc/message.html" target="_blank">
        サマチャレ卒業生からのメッセージ
    </a>  <br>
    サマチャレ第17期生のOBとして、サマチャレに参加しようとする後輩へメッセージを書きました。
    もっと詳しいサマチャレ体験記を書こうとしてますが、進捗は全くありません。
    </li>
</ul>
</div>

