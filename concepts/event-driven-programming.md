# ⚡ Programação Orientada a Eventos (Event-Driven Programming)

## 💡 O que é

Programação orientada a eventos é um paradigma em que o fluxo de execução do programa é
determinado por **eventos** — ações do usuário (cliques, toques), mensagens do sistema
(app iniciado, tela aberta) ou sinais externos. Em vez de o código executar em sequência
linear, ele fica "escutando" e reage quando algo acontece.

Esse paradigma é o modelo central de interfaces gráficas e apps mobile: o app fica em estado
de espera e só executa lógica quando o usuário interage. Cada elemento visual pode ter
múltiplos tipos de evento associados (clique, pressionamento longo, mudança de valor, etc.).

Em plataformas visuais como o Kodular, os eventos são representados como blocos com a
estrutura: **"Quando [componente].[evento] → faça [ações]"**.

## ⚙️ Como é usado neste projeto

Todo o comportamento do PedePizza é orientado a eventos. Cada interação do usuário
dispara um bloco de evento no Kodular que executa as ações correspondentes:

- **Clique em botão de categoria** → navega para a tela da sublista
- **Seleção em ListView** → armazena a escolha em variável global e atualiza o label do botão
- **Clique em FAZER PEDIDO** → navega para a tela de confirmação
- **Clique em Voltar** → retorna à tela principal

## 🔍 Exemplo do projeto

```
[ Evento: Screen1.Initialize ]
  → inicializar variáveis globais (saborSalgado, saborDoce, borda, bebida = "")

[ Evento: BotaoBebidas.Clique ]
  → abrir outra tela: "TelaBebidas"

[ Evento: ListaBebidas.AposSelecionar ]
  → definir variável global bebida = elemento selecionado
  → definir BotaoBebidas.Texto = variável global bebida
  → fechar tela atual
```
*(Representação textual dos blocos de evento do Kodular)*

## 📚 Recursos para aprofundamento

- [Event-Driven Programming — MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events) — conceito aplicado ao contexto web
- [Kodular Blocks — Event Handlers](https://docs.kodular.io/blocks/control/) — documentação dos blocos de controle e evento
- [Paradigmas de Programação — DevMedia](https://www.devmedia.com.br/paradigmas-de-programacao/33698) — visão geral em português
