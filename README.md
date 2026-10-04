# GO! | Pasta de marca

Logo escolhido: **A, Tipográfica**. Nome sempre escrito **GO!**, em Unbounded ExtraBold, com o "!" em verde.

Esta pasta junta o que já está pronto para usar e as regras para usar sempre do mesmo jeito.

## O que tem em cada pasta

| Pasta | Conteúdo |
|---|---|
| `01-logo` | Logos em SVG e a página `exportar-png-e-ico.html`, que gera os PNG e o favicon.ico |
| `02-tokens` | `go-tokens.css` (web) e `GoBrand.cs` (apps em C#) com cores e fontes |
| `03-aplicacoes` | Exemplos prontos: login do SGO, rodapé de tela, documento (ordem de serviço), assinatura de e-mail, cartão de visita, carimbo e avatar |
| `04-referencia` | Manual de uso visual, resumo das aplicações, a prancha do logo A e o registro em texto |
| `05-propostas-descartadas` | Propostas B e C, só para histórico |

Todos os arquivos `.html` abrem direto no navegador. Eles carregam a fonte do Google Fonts, então precisam de internet.

## Ver no navegador

O repo é publicado no GitHub Pages, então as páginas abrem sem clonar:

- [Manual de uso](https://gontechbr.github.io/go-marca/04-referencia/manual-de-uso.html)
- [Logo A escolhido](https://gontechbr.github.io/go-marca/04-referencia/logo-A-escolhido.html)
- [Resumo das aplicações](https://gontechbr.github.io/go-marca/04-referencia/aplicacoes-resumo.html)
- [Exportar PNG e ICO](https://gontechbr.github.io/go-marca/01-logo/exportar-png-e-ico.html)

O site da GO! (repo [gontechbr.github.io](https://github.com/gontechbr/gontechbr.github.io)) usa as cores e fontes daqui.

## Padrões

### Nome
- Escrita exata: **GO!** (G e O maiúsculos, com ponto de exclamação).
- Nunca "Go!", "go!" ou "GO !".

### Fonte
- Logo e títulos curtos: **Unbounded**, peso 800 (ExtraBold), espaçamento entre letras de -0,05 em, entrelinha 1.
- Texto de telas e documentos: **Hanken Grotesk** (400, 500 e 700). É uma sugestão e pode ser trocada sem afetar o logo.
- As duas são do Google Fonts, com licença SIL Open Font License (uso comercial livre).

### Cores

| Nome | Hex | Uso |
|---|---|---|
| Verde GO | `#0A9E64` | O "!" do logo e detalhes de destaque. Não usar em texto corrido |
| Grafite | `#0F1114` | Letras em fundo claro, texto, fundos escuros |
| Claro | `#F4F5F7` | Letras em fundo escuro e superfícies |
| Cinza de apoio | `#5B6270` | Textos secundários e legendas |

O laranja do SGO (`#ED653B`) fica no produto, não no logo da GO!.

### Versões do logo
1. Horizontal para usar sobre fundo claro (`go-logo-sobre-fundo-claro`): "GO" grafite, "!" verde.
2. Horizontal para usar sobre fundo escuro (`go-logo-sobre-fundo-escuro`): "GO" claro, "!" verde.
3. Uma cor preto, para carimbo e impressão simples.
4. Uma cor branco, sobre fundo escuro ou foto.
5. Ícone quadrado (cantos com raio de 22% do lado). O nome do arquivo diz a cor do próprio quadrado: `fundo-escuro` é o quadrado grafite com letras claras (use sobre fundo claro) e `fundo-claro` é o quadrado claro com letras grafite (use sobre fundo escuro).
6. Favicon de 16 px: variante "G!". De 32 px em diante, o ícone com "GO!".

### Tamanhos e respiro
- Assinatura "um produto GO!": o logo com 12 px de altura de letra, ao lado do texto "um produto" em cinza.
- Respiro mínimo ao redor do logo: a largura do "!".
- Impressão e carimbo: só a versão de uma cor.

### Não fazer
- Esticar, achatar, inclinar ou contornar o logo.
- Pintar o logo inteiro de verde ou trocar a cor do "!".
- Aplicar sombra, brilho ou gradiente.
- Escrever em minúsculas ou misturar maiúsculas e minúsculas.

## Como usar

**Na web**, importe o CSS e use o marcador:

```html
<link rel="stylesheet" href="go-tokens.css">
<span class="go-logo">GO<span class="go-bang">!</span></span>
```

Favicon e ícone de app:

```html
<link rel="icon" href="/favicon.ico" sizes="any">
<link rel="apple-touch-icon" href="/go-icone-fundo-escuro-180.png">
```

**Nos apps em C#**, adicione `GoBrand.cs` ao projeto e use as constantes (`GoBrand.Verde`, `GoBrand.GrafiteArgb` e as demais).

**Assinatura nas telas**: use o modelo de `03-aplicacoes/rodape-de-tela.html` e `login-sgo.html`.

**Documentos**: use `documento-ordem-de-servico.html` como base. Os textos entre colchetes são campos a preencher.

## Como gerar os PNG e o favicon.ico

1. Abra `01-logo/exportar-png-e-ico.html` no Chrome ou no Edge, com internet.
2. Clique em **Gerar arquivos**.
3. Baixe cada arquivo pelo link. O resultado inclui logos horizontais (sobre fundo claro, sobre fundo escuro, preto, branco), ícones de 512, 192, 180 e 64 px com quadrado escuro e com quadrado claro, avatar redondo, favicons de 16, 32 e 48 px e o `favicon.ico`.

## O que ainda falta

- **Logo em curvas (outline).** Os SVGs de `01-logo/svg` usam a fonte como texto e só aparecem corretamente com internet. Para gráfica, carimbo e entrega a terceiros, o ideal é converter para curvas. Isso precisa do arquivo da Unbounded ExtraBold (`.ttf`), que não consegui baixar no ambiente em que montei esta pasta.
- **Ajuste fino do "!".** Hoje é o "!" da fonte pintado de verde. Dá para desenhar um ponto próprio e acertar o espaçamento entre as letras depois de ver em tamanho grande.
- **Revisão em 16 px.** Confira o favicon "G!" na aba do navegador antes de fechar.
- **Dados de contato.** Cargo, telefone e e-mail estão como campos entre colchetes nos modelos.
