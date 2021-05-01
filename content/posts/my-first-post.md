---
title: "Embedding a chart in your posts"
date: 2019-11-01T11:21:27+01:00
draft: false
---

<!---
<link href="{{"mermaid/mermaid.css" | relURL}}{{ if not .Site.Params.disableAssetsBusting }}?{{ now.Unix }}{{ end }}" rel="stylesheet" />
<script src="{{"mermaid/mermaid.js" | relURL}}{{ if not .Site.Params.disableAssetsBusting }}?{{ now.Unix }}{{ end }}"></script>
<script>
	mermaid.initialize({ startOnLoad: true });
</script>
--->
Just in case you want to add some kind of schema in your blog like this one

```
{{< mermaid align="left" >}}
graph LR;
    A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
{{< /mermaid >}}
```

Just do:

```
{{</*  mermaid align="left" */>}}
graph LR;
    A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
{{</* /mermaid */>}}
```
