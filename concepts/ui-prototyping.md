# 🎨 Prototipagem de Interface (UI Prototyping)

## 💡 O que é

Prototipagem de interface é o processo de criar uma representação visual e interativa de um
produto digital **antes** de sua implementação real. O objetivo é validar o fluxo de
navegação, a disposição dos elementos e a experiência do usuário sem precisar escrever
código ou compilar um app.

Protótipos podem ter diferentes níveis de fidelidade: esboços em papel (baixa fidelidade)
ou simulações navegáveis com design final (alta fidelidade). Ferramentas como o **Figma**
permitem criar protótipos de alta fidelidade com animações de transição, componentes
reutilizáveis e conexões entre telas — o que possibilita testes de usabilidade reais
antes da linha de código existir.

A prototipagem reduz o retrabalho, alinha expectativas entre designer e desenvolvedor,
e documenta as decisões de interface de forma que toda a equipe pode consultar.

## ⚙️ Como é usado neste projeto

O PedePizza foi prototipado no **Figma** antes de ser implementado no Kodular. O protótipo
serviu como referência visual para o design das telas: cores (azul para a AppBar, laranja
para os botões de ação), tipografia, disposição dos elementos e fluxo de navegação.

O processo seguiu a sequência: **Figma (design) → Kodular (implementação) → APK (distribuição)**.

## 🔍 Exemplo do projeto

As telas do app implementado seguem fielmente o design prototipado:

- AppBar azul com título do app
- Fundo rosa claro (`#FFF0F0` aproximado)
- Botões de categoria em laranja suave
- Botão de ação principal (FAZER PEDIDO / Voltar) em laranja escuro

```
Figma Frame: "Tela Principal"
  ├── AppBar [azul] → texto: "PedePizza1.0"
  ├── Título: "OPÇÕES DE PEDIDO"
  ├── Botão Categoria 1 [laranja] → navega para "Salgados"
  ├── Botão Categoria 2 [laranja] → navega para "Doces"
  ├── Botão Categoria 3 [laranja] → navega para "Bordas"
  ├── Botão Categoria 4 [laranja] → navega para "Bebidas"
  └── Botão CTA [laranja escuro] → navega para "Confirmação"
```

## 📚 Recursos para aprofundamento

- [Figma — Get Started](https://help.figma.com/hc/en-us/categories/360002051613) — documentação oficial do Figma
- [Prototipagem no Figma — Alura](https://www.alura.com.br/artigos/prototipagem-figma) — artigo introdutório em português
- [UX Design Fundamentals — Nielsen Norman Group](https://www.nngroup.com/articles/ux-prototype/) — conceitos de fidelidade de protótipo
