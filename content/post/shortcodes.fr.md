+++
date = "2016-12-23T17:42:26"
title = "Hugo Shortcodes"
tags = ["exemples", "shortcodes"]
categories = ["exemples"]
slug = "hugo-shortcodes"
draft = false

+++

Dui purus curàé posuere blandît aptent donéc fringilla phaséllœs quis sed nètus conséquat, rhoncus porté mlius quam nûllam est ultricités habitasse mauris dïam dapidûs "sélecrum", dolor intègèr convallis litora enim nullam aliquàm congés. Nombre class classé justo mié egéstat, convallis metus condimentum. Adipiscing curàbitur arcû incéptos duèis vulputate mollis néc curabitur augueé inceptos eros, anonyma potentié ultricités est varius etiam donec nîbh mollis ïpsum dui, curabitur platéa integer séd lectus tincidûnt integer nulla rhoncus nisi, famès morbi aliquam çunc id malésdum quisquées vehicula convallis. Name interdum tempès commodoé ligula bibendum cubliâ portitorsé éuismod curabitur c'est hâc, aliquam 21 898€ adipiscing risius ût nisl adipiscing voluptà sempér interdum, eleifend anté lacinia convallis posuere cubilia maecenas bibendum maécènas luctus èst, ad nec ad ultrûcéas commodoé. 

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

Relref: [À propos]({{< ref "about.en.md" >}})

Twitter:

{{< tweet 666616452582129664 >}}

YouTube:

{{< youtube w7Ft2ymGmfc >}}

Vimeo:

{{< vimeo 146022717 >}}

GitHub gist:

{{< gist spf13 7896402 >}}

Speaker Deck:

{{< speakerdeck 4e8126e72d853c0060001f97 >}}

Instagram:

{{< instagram BMokmydjG-M >}}
