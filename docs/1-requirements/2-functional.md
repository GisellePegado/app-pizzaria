# 🛠️ Requisitos Funcionais

> Derivados das Histórias de Usuário HU-01 e HU-02.

Os requisitos funcionais descrevem **o que o sistema deve fazer**.

| ID   | Nome                        | Descrição                                                                                 |
| ---- | --------------------------- | ----------------------------------------------------------------------------------------- |
| RF01 | Exibir menu de pedido       | O app exibe as quatro categorias de pedido na tela principal (tela "OPÇÕES DE PEDIDO")    |
| RF02 | Navegar para sublista       | Ao tocar em uma categoria, o app navega para a tela com as opções daquela categoria       |
| RF03 | Selecionar item             | O usuário seleciona um item da sublista e o app registra a escolha                        |
| RF04 | Atualizar tela principal    | Após a seleção, o placeholder da categoria é substituído pelo nome do item escolhido      |
| RF05 | Confirmar pedido            | O botão "FAZER PEDIDO" leva à tela de resumo com todas as escolhas realizadas             |
| RF06 | Voltar ao menu              | O botão "Voltar" na tela de confirmação retorna o usuário ao menu de pedido               |

---

## 🔗 Rastreabilidade: RF × Histórias de Usuário

| Requisito              | HU-01 | HU-02 |
| ---------------------- | :---: | :---: |
| RF01 — Exibir menu     |  ✅   |  ✅   |
| RF02 — Navegar sublista|  ✅   |  ✅   |
| RF03 — Selecionar item |  ✅   |  ✅   |
| RF04 — Atualizar tela  |  ✅   |   —   |
| RF05 — Confirmar pedido|  ✅   |   —   |
| RF06 — Voltar ao menu  |  ✅   |   —   |

---

## 💻 Implementação no App

| Requisito | Implementação no Kodular                                        |
| --------- | --------------------------------------------------------------- |
| RF01      | Tela principal com 4 botões de categoria + botão FAZER PEDIDO   |
| RF02      | Evento de clique em botão → navegar para Screen da categoria    |
| RF03      | ListView com os itens da categoria; clique registra seleção     |
| RF04      | Variável global armazena escolha; label do botão é atualizado   |
| RF05      | Tela de confirmação exibe as 4 variáveis globais em labels      |
| RF06      | Botão "Voltar" chama bloco de navegação para Screen principal   |
