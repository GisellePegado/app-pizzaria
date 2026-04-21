# 🔁 Desenvolvimento Iterativo (Iterative Development)

## 💡 O que é

Desenvolvimento iterativo é uma abordagem de construção de software em que o produto é
entregue em **ciclos curtos e incrementais** — cada iteração adiciona novas funcionalidades
sobre o que já existe e foi validado. Em vez de construir tudo de uma vez e entregar ao
final, a equipe entrega versões funcionais progressivamente.

Essa abordagem reduz o risco de retrabalho (erros são detectados cedo), facilita o
feedback do cliente (cada versão pode ser testada) e mantém o projeto sempre em um
estado "entregável". É um dos princípios centrais de metodologias ágeis como Scrum e XP.

O desenvolvimento iterativo se diferencia do incremental puro pelo fato de que cada
iteração pode também **refinar** o que foi feito anteriormente, não apenas adicionar.

## ⚙️ Como é usado neste projeto

O PedePizza evoluiu em **4 iterações**, cada uma representada por um APK versionado no
repositório. Cada versão entregou uma parte funcional do fluxo de pedido:

| Iteração | Versão | Funcionalidade entregue               |
| -------- | ------ | ------------------------------------- |
| 1ª       | v1     | Tela principal + seleção de salgado   |
| 2ª       | v2     | + Seleção de sabor doce               |
| 3ª       | v3     | + Seleção de borda e bebida           |
| 4ª       | v4     | + Tela de confirmação com resumo      |

A versão v4 representa o produto completo — mas cada versão anterior já era um app
funcional e instalável, mesmo com o fluxo ainda incompleto.

## 🔍 Exemplo do projeto

```
v1: [Menu: Sabores Salgados | Sabores Doces | Bordas | Bebidas] → apenas Salgados funcional

v2: [Menu: Marguerita | Sabores Doces | Bordas | Bebidas] → Salgados + Doces funcionais

v3: [Menu: Marguerita | Banana Nevada | Bordas | Bebidas] → + Bordas + Bebidas

v4: [Menu: Marguerita | Banana Nevada | Catupiry | Guaraná] → FAZER PEDIDO → Confirmação ✅
```

## 📚 Recursos para aprofundamento

- [Iterative and Incremental Development — Wikipedia](https://en.wikipedia.org/wiki/Iterative_and_incremental_development) — visão histórica e conceitual
- [Scrum Guide](https://scrumguides.org/scrum-guide.html) — metodologia ágil que formaliza o desenvolvimento iterativo
- [Desenvolvimento Ágil — Agile Manifesto](https://agilemanifesto.org/iso/ptbr/manifesto.html) — manifesto em português
