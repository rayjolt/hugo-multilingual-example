+++
date = "2016-12-22T09:31:31"
title = "Hugoのショートコード"
tags = ["例"]
categories = ["例", "ショートコード"]
slug = "hugo-no-shotokodo"
draft = false

+++

やぶら小路の藪柑子、シューリンガンのグーリンダイ。五劫の擦り切れ、寿限無、寿限無。長久命の長助、水行末 雲来末 風来末、パイポパイポ パイポのシューリンガン。シューリンガンのグーリンダイ、グーリンダイのポンポコピーのポンポコナーの、水行末 雲来末 風来末、海砂利水魚の。五劫の擦り切れ、やぶら小路の藪柑子、食う寝る処に住む処。

ハイライト：

{{< highlight html >}}
<section id="main">
  <div>
   <h1 id="title">{{ .Title }}</h1>
    {{ range .Data.Pages }}
        {{ .Render "summary"}}
    {{ end }}
  </div>
</section>
{{< /highlight >}}

フィギュア：

{{< figure src="/img/post/shortcodes/piano.jpg" title="ピアノ" >}}

Relref：[プロフィール]({{< ref "about.ja.md" >}})

ツイッター

{{< tweet 666616452582129664 >}}

YouTube：

{{< youtube w7Ft2ymGmfc >}}

Vimeo：

{{< vimeo 146022717 >}}

GitHubジスト：

{{< gist spf13 7896402 >}}

スピーカーデック：

{{< speakerdeck 4e8126e72d853c0060001f97 >}}

インスタグラム：

{{< instagram BMokmydjG-M >}}
