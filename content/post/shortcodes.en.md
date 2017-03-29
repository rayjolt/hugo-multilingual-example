+++
date = "2016-12-22T09:31:31"
title = "Hugo Shortcodes"
tags = ["examples", "shortcodes"]
categories = ["examples"]
slug = "hugo-shortcodes"
draft = false

+++

Ex nostrum deterruisset usu, ea nam constituam efficiantur, in sed stet libris accumsan. Odio ubique oblique vis an, eu falli bonorum adversarium eum. Nec eu indoctum consulatu incorrupte, reque ridens oblique nam at, scripta expetenda usu an. His dicit doming in, eu pro partem abhorreant, possit tincidunt ius ne. Ne nam saperet ornatus eloquentiam, an modus delectus mei.

Highlight:

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

Figure:

{{< figure src="/img/post/shortcodes/piano.jpg" title="A piano" >}}

Relref: [About]({{< ref "about.en.md" >}})

Twitter:

{{< tweet 666616452582129664 >}}

YouTube:

{{< youtube w7Ft2ymGmfc >}}

Vimeo:

{{< vimeo 146022717 >}}

GitHub gists:

{{< gist spf13 7896402 >}}

Speaker Deck:

{{< speakerdeck 4e8126e72d853c0060001f97 >}}

Instagram:

{{< instagram BMokmydjG-M >}}
