# 📖 Histórias de Usuário

> Disciplina: Fundamentos de Design de Sistemas — UNINTER

---

## 📑 HU-01 — Montar e enviar um pedido de pizza

**Como** cliente da pizzaria,
**quero** escolher sabor salgado, sabor doce, tipo de borda e bebida em etapas separadas,
**para que** eu possa montar meu pedido de forma guiada e confirmar antes de finalizar.

### ✅ Critérios de Aceitação

- [ ] O app exibe as categorias de pedido (Sabores Salgados, Sabores Doces, Bordas, Bebidas)
- [ ] Cada categoria abre uma sublista com as opções disponíveis
- [ ] Ao selecionar uma opção, o placeholder da categoria é substituído pela escolha feita
- [ ] O botão "FAZER PEDIDO" só leva à tela de confirmação após todas as seleções
- [ ] A tela de confirmação exibe um resumo com todas as escolhas realizadas
- [ ] O botão "Voltar" na tela de confirmação retorna ao menu de pedido

---

## 📑 HU-02 — Visualizar opções disponíveis por categoria

**Como** cliente da pizzaria,
**quero** ver a lista completa de opções ao tocar em cada categoria,
**para que** eu possa escolher com base nos itens disponíveis no momento.

### ✅ Critérios de Aceitação

- [ ] Sabores Salgados exibe: Calabresa, Marguerita, Portuguesa
- [ ] Sabores Doces exibe: Prestígio, Banana Nevada, Oreo
- [ ] Bordas exibe: Catupiry, Cheddar, Doce de leite
- [ ] Bebidas exibe: Guaraná, Coca-Cola, Água, Suco
- [ ] A navegação de volta à tela principal funciona após a seleção

---

## 🌐 Contexto

O **PedePizza** é um aplicativo mobile Android desenvolvido com a plataforma Kodular,
com interface projetada no Figma. Ele simula o fluxo de pedido de uma pizzaria,
guiando o cliente por quatro categorias de escolha — sabor salgado, sabor doce,
borda e bebida — até a confirmação final do pedido.
