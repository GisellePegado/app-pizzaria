# 🧱 Desenvolvimento Low-Code (Low-Code Development)

## 💡 O que é

Desenvolvimento low-code é uma abordagem de criação de software em que a maior parte da
lógica e da interface é construída por meio de ferramentas visuais — como editores gráficos,
blocos de programação e componentes arrastáveis — em vez de código escrito manualmente linha
por linha.

Plataformas low-code reduzem significativamente a barreira de entrada para o desenvolvimento
de aplicações, permitindo que pessoas com pouco ou nenhum conhecimento de programação
tradicional criem produtos funcionais. Isso é especialmente valioso em contextos acadêmicos,
prototipagem rápida e projetos de pequeno porte.

O conceito se diferencia de "no-code" pelo fato de ainda permitir — e muitas vezes exigir —
algum nível de lógica estruturada, mesmo que visual.

## ⚙️ Como é usado neste projeto

O PedePizza foi construído inteiramente no **Kodular Creator**, uma plataforma low-code
derivada do MIT App Inventor. Toda a lógica do app — navegação entre telas, atualização
de estado, resposta a eventos de clique — foi implementada por meio de blocos visuais,
sem escrita de código Kotlin, Java ou qualquer linguagem nativa.

O resultado final é compilado pela plataforma e exportado diretamente como um APK Android.

## 🔍 Exemplo do projeto

```
[ Quando: BotaoSaborSalgado.Clique ]
  → abrir outra tela: "TelaSaboresSalgados"

[ Quando: ListaSalgados.AposSelecionar ]
  → definir variável global saborSalgado = elemento selecionado
  → definir BotaoSaborSalgado.Texto = variável global saborSalgado
  → abrir outra tela: "TelaPrincipal"
```
*(Representação textual da lógica de blocos do Kodular)*

<details>
<summary>🧱 Blocos Kodular</summary>

<img width="1277" height="867" alt="SotfwarePizzaria-kodular-blocks" src="https://github.com/user-attachments/assets/39007895-0e43-42d8-845a-6a019edef11b" />

</details>

## 📚 Recursos para aprofundamento

- [Kodular Documentation](https://docs.kodular.io) — documentação oficial da plataforma
- [MIT App Inventor](https://appinventor.mit.edu) — plataforma original da qual o Kodular deriva
- [What is Low-Code? — Mendix](https://www.mendix.com/low-code-guide/) — introdução ao paradigma low-code
