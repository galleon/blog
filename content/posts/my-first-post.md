---
title: "My First Post"
date: 2019-11-01T11:21:27+01:00
draft: true
---

<!---
<link href="{{"mermaid/mermaid.css" | relURL}}{{ if not .Site.Params.disableAssetsBusting }}?{{ now.Unix }}{{ end }}" rel="stylesheet" />
<script src="{{"mermaid/mermaid.js" | relURL}}{{ if not .Site.Params.disableAssetsBusting }}?{{ now.Unix }}{{ end }}"></script>
<script>
	mermaid.initialize({ startOnLoad: true });
</script>
--->
Blah blah

{{< mermaid align="left" >}}
graph LR;
    A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
{{< /mermaid >}}

{{< mermaid align="right" >}}
graph LR;
    A[Bords droits] -->|Lien texte| B(Bords arondis)
    B --> C{Décision}
    C -->|Un| D[Résultat un]
    C -->|Deux| E[Résultat deux]
{{< /mermaid >}}

This is my first post with a chart
