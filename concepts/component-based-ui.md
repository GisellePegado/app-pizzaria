# 🧩 UI Baseada em Componentes (Component-Based UI)

## 💡 O que é

UI baseada em componentes é uma abordagem de construção de interfaces em que a tela é
composta por blocos reutilizáveis e independentes — cada um com seu próprio visual,
comportamento e estado. Em vez de construir cada tela do zero, o desenvolvedor monta
a interface combinando componentes pré-definidos (botões, listas, barras de navegação, etc.).

Essa abordagem facilita a consistência visual (todos os botões da mesma categoria têm a
mesma aparência), a manutenção (alterar o componente reflete em todos os usos) e a
produtividade (componentes são reutilizados em vez de recriados).

Em plataformas como o Kodular, os componentes são os blocos de UI disponíveis no editor
visual — cada um com propriedades configuráveis e eventos associados.

## ⚙️ Como é usado neste projeto

O PedePizza usa os seguintes componentes do Kodular de forma consistente em todas as telas:

| Componente   | Uso no projeto                                                  |
| ------------ | --------------------------------------------------------------- |
| `Button`     | Botões de categoria (laranja) e botão de ação principal (CTA)   |
| `ListView`   | Listas de opções em cada tela de sublista (salgados, doces, etc.) |
| `Label`      | Títulos das telas e textos informativos                         |
| `Screen`     | Cada tela do app é uma Screen independente                      |
| `HorizontalArrangement` / `VerticalArrangement` | Organização do layout |

O padrão visual é replicado de forma consistente: AppBar azul, fundo rosa claro, botões
em laranja — graças à reutilização dos mesmos componentes com as mesmas propriedades.

## 🔍 Exemplo do projeto

```
Screen: TelaSaboresSalgados
  ├── TitleBar: "SoftwarePedePizza" [azul]
  └── ListView
        ├── item: "Calabresa"
        ├── item: "Marguerita"
        └── item: "Portuguesa"

Screen: TelaSaboresDoces
  ├── TitleBar: "SoftwarePedePizza" [azul]  ← mesmo componente, mesma config
  └── ListView
        ├── item: "Prestígio"
        ├── item: "Banana Nevada"
        └── item: "Oreo"
```

## 📚 Recursos para aprofundamento

- [Component-Based Architecture — freeCodeCamp](https://www.freecodecamp.org/news/how-to-use-component-based-architecture-in-react/) — conceito aplicado ao React
- [Kodular Components Overview](https://docs.kodular.io/components/) — lista completa de componentes disponíveis
- [Design Systems — Nielsen Norman Group](https://www.nngroup.com/articles/design-systems-101/) — sistemas de design e componentização
