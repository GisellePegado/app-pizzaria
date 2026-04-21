# 🔀 Fluxo de Navegação entre Telas (Navigation Flow)

## 💡 O que é

Fluxo de navegação é a sequência de transições entre telas (ou estados) que um usuário
percorre para completar uma tarefa em um aplicativo. Definir esse fluxo é uma das decisões
centrais de design de UX, pois determina quantas interações são necessárias, em que ordem
o usuário toma decisões e como ele pode desfazer ou corrigir escolhas anteriores.

Em apps mobile, os padrões mais comuns de navegação são: navegação linear (tela A → B → C),
navegação por abas (acesso direto a qualquer seção) e navegação hierárquica (menu → sublista
→ detalhe). O PedePizza adota o modelo **hierárquico linear** — cada categoria é acessada
a partir do menu principal e retorna a ele após a seleção.

## ⚙️ Como é usado neste projeto

O app implementa um fluxo de 6 telas com navegação hierárquica:

```
Tela Principal (menu)
  ├── → Tela Sabores Salgados → volta ao menu com seleção registrada
  ├── → Tela Sabores Doces    → volta ao menu com seleção registrada
  ├── → Tela Bordas           → volta ao menu com seleção registrada
  ├── → Tela Bebidas          → volta ao menu com seleção registrada
  └── → Tela Confirmação      → botão Voltar retorna ao menu
```

O estado é mantido entre navegações por meio de variáveis globais, garantindo que as
seleções anteriores não sejam perdidas ao navegar para outra categoria.

## 🔍 Exemplo do projeto

Fluxo real observado nas telas do app (frames numerados):

```
[1] Menu inicial: Sabores Salgados | Sabores Doces | Bordas | Bebidas
 ↓ toca "Sabores Salgados"
[2] Lista: Calabresa / Marguerita / Portuguesa → seleciona "Marguerita"
 ↓ retorna ao menu
[3] Menu: "Marguerita" | Sabores Doces | Bordas | Bebidas
 ↓ toca "Sabores Doces" → seleciona "Banana Nevada"
[5] Menu: "Marguerita" | "Banana Nevada" | Bordas | Bebidas
 ↓ ...
[9] Menu completo: Marguerita | Banana Nevada | Catupiry | Guaraná
 ↓ toca "FAZER PEDIDO"
[10] Confirmação: resumo dos 4 itens + botão Voltar
```

## 📚 Recursos para aprofundamento

- [Navigation Design Patterns — UX Planet](https://uxplanet.org/navigation-design-almost-everything-you-need-to-know-about-navigation-for-mobile-ui-9ce3f96c4f59) — padrões de navegação mobile
- [Fluxo de Usuário — NNg](https://www.nngroup.com/articles/user-journeys-vs-user-flows/) — diferença entre user journey e user flow
- [Kodular — Multiple Screens](https://docs.kodular.io/guides/multiple-screens/) — navegação entre telas no Kodular
