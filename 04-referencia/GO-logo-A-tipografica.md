# GO! | Logo A (Tipográfica)

Registro da direção escolhida. Versão de trabalho, ainda não é o manual final da marca.

## Ideia

Só o nome, em letra larga e arredondada, com cara de painel de máquina. O "GO" fica apertado e vira um bloco só. O "!" em verde é o único destaque, como uma luz acesa.

A GO! é a marca acima dos produtos. O primeiro é o SGO (Sistema de Gestão Operacional). Ela aparece pequena como assinatura ("um produto GO!") e também sozinha, como ícone de app, avatar e cabeçalho de documento.

## Fonte

- Família: **Unbounded**, peso **ExtraBold (800)**
- Origem: Google Fonts (licença SIL Open Font License, uso comercial livre)
- Escrita exata: **GO!** (G e O maiúsculos, com ponto de exclamação)
- Espaçamento entre letras: **-0,05 em** (apertado)
- Altura da entrelinha: 1
- "GO" na cor principal do contexto, "!" em verde

CSS de referência:

```css
.go-logo {
  font-family: 'Unbounded', sans-serif;
  font-weight: 800;
  letter-spacing: -0.05em;
  line-height: 1;
  color: #0F1114;
}
.go-logo .bang { color: #0A9E64; }
```

```html
<span class="go-logo">GO<span class="bang">!</span></span>
```

Carregamento: `https://fonts.googleapis.com/css2?family=Unbounded:wght@800&display=swap`

Para material impresso, carimbo e arquivo final, a fonte deve ser convertida em curvas (outline) antes de sair da mão do designer.

## Cores

| Nome | Hex | Uso |
|---|---|---|
| Verde GO | `#0A9E64` | O "!" e nenhum outro elemento do logo |
| Grafite | `#0F1114` | Letras em fundo claro, fundo do ícone, fundo escuro de referência |
| Claro | `#F4F5F7` | Letras em fundo escuro, fundo do ícone em fundo escuro |

O verde tem contraste de cerca de 3,4:1 sobre branco e 5,4:1 sobre o grafite. Serve para o "!" (elemento gráfico grande), mas não deve ser usado para texto corrido.

O laranja do SGO (`#ED653B`) não entra no logo da GO!. A GO! tem cor própria e convive com ele.

## Versões

1. **Horizontal**, em fundo claro: "GO" grafite, "!" verde.
2. **Horizontal**, em fundo escuro (`#0F1114`): "GO" claro, "!" verde.
3. **Uma cor, preto**: tudo grafite, para carimbo e impressão simples.
4. **Uma cor, branco**: tudo branco, sobre fundo escuro ou foto.
5. **Ícone quadrado**: quadrado de cantos arredondados (raio de 22% do lado) com "GO!" centralizado.
   - Em fundo claro: quadrado grafite, letras claras, "!" verde.
   - Em fundo escuro: quadrado claro, letras grafite, "!" verde.
   - Uma cor: quadrado cheio, letras vazadas.
6. **Assinatura "um produto GO!"**: texto "um produto" em cinza neutro, seguido do logo com 12 px de altura (altura da letra).

## Regras de uso

- Escrever sempre **GO!**, nunca "Go!", "go!" ou "GO !".
- Não inclinar, esticar, contornar ou aplicar sombra, gradiente ou brilho.
- Não trocar a cor do "!" por outra que não seja o verde da marca (ou a cor única da versão monocromática).
- Área de respiro mínima ao redor do logo: a largura do "!".
- Não usar o verde em outras letras do logo.

## Pontos em aberto (o que ainda pode melhorar)

- **Ícone de 16 px**: a Unbounded é muito larga, então o "GO!" em 16 px fica pequeno e apertado. Vale testar uma variante só para favicon (por exemplo "G!" maior, ou o "GO" em duas linhas).
- **Ajuste fino de espaçamento (kerning)**: o par G e O, e o O com o "!", podem ser acertados à mão depois de ver em tamanho grande.
- **Detalhe próprio no "!"**: hoje é o "!" da fonte, só pintado de verde. Dá para desenhar um ponto circular maior ou levemente separado, para o logo ficar menos "fonte digitada".
- **Conversão em curvas** e entrega em SVG, PNG e PDF.

## Assets possíveis a partir daqui

- Favicon e ícones de app (16, 32, 48, 180, 192, 512 px, mais `.ico` e SVG)
- Avatar de perfil
- Tela de login com a assinatura "um produto GO!"
- Cabeçalho e rodapé de documento (relatório, ordem de serviço, proposta)
- Assinatura de e-mail
- Modelo de apresentação
- Cartão de visita
- Carimbo (versão uma cor)
- Lockups por produto: "SGO | um produto GO!" e os apps de fábrica (aperto, rastreabilidade, integração com MES)
- Tokens de cor e tipografia em CSS, para uso direto nas telas
- Folha de estilo curta com tudo isso (manual da marca em uma página)
