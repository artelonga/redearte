---
title: Propriedades
description: documentação sobre propriedades são dados sobre o conteúdo em formato YAML
permalink: 
date: 2024-10-22
time: 12:14
type: garden
tags: 
draft: false
---

Propriedades são informações sobre o [[conteudo|conteúdo]], funcionando como uma [[YAML como dados|Base de Dados]]


> [!quote] [Obsidian Help](https://help.obsidian.md/Home)> Edição e formatação > [Propriedades](https://help.obsidian.md/Editing+and+formatting/Properties)
Propriedades contêm dados estruturados, como [texto](https://help.obsidian.md/Editing+and+formatting/Properties#^text-list), links, [datas](https://help.obsidian.md/Editing+and+formatting/Properties#^date-time), [verdadeiro ou falso](https://help.obsidian.md/Editing+and+formatting/Properties#:~:text=Number-,Checkbox,-Date), e [números](https://help.obsidian.md/Editing+and+formatting/Properties#^numbers)...</br>
Propriedades são armazenadas em formato [YAML](https://help.obsidian.md/Editing+and+formatting/Properties#:~:text=are%20stored%20in-,YAML,-format%20at%20the) (...), formato popular legível tanto por humanos quanto por computadores.


## Exemplos de propriedades

### Propriedades Nativas do Obsidian

As [propriedades](https://help.obsidian.md/Editing+and+formatting/Properties) (em inglês) do Obsidian são 

*  `tags` : palavras-chave ou tópicos (ver [Tags](https://help.obsidian.md/Editing+and+formatting/Tags))
* `cssclasses` informação sobre estilo usando [CSS](https://github.com/r-u-s-h-i-k-e-s-h/Obsidian-CSS-Snippets)
* `aliases` : nomes alternativos (ver [Aliases](https://help.obsidian.md/Linking+notes+and+files/Aliases))

Para links internos nas propriedades, é necessário usar aspas

```YAML
---
link: "[[Link]]"
linklist:
- "[[Link]]" 
- "[[Link2]]" 
---
```


### Propriedades Nativas do [[Quartz]]

Quartz é o componente responsável por renderizar o conteúdo na internet. Quartz também utiliza [propriedades](https://quartz.jzhao.xyz/authoring-content#syntax):


```YAML
---
title: 
description: 
permalink: 
aliases:
tags: 
draft: TRUE
---
```

- `title`: Titulo da página. Se não é providenciado, Quartz utiliza o nome do arquivo como título.
- `description`: Descrição da página utilizada em pré-visualizações do link.
- `permalink`: Uma URL customizada, constante mesmo que o caminho para o arquivo mude.
- `draft`: Se a página deve ser publicada ou não. Uma das formas de tornar  [páginas privadas](https://quartz.jzhao.xyz/features/private-pages)
- `date`:  Uma string representando a data em que a nota foi criada. Normalmente usa o formato `YYYY-MM-DD`.

## Propriedades [[content/redearte/jardim/plataforma/Rede Arte|Rede Arte]]

A Rede Arte utiliza a propriedade `type` para diferenciar entre conteúdo

```YAML
---
title: 
description: 
permalink: 
aliases:
tags: 
type: "reference"
draft: TRUE
```