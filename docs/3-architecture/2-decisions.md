# ⚖️ Decisões de Arquitetura (ADRs)

## 🏛️ ADR-001 — Uso do Kodular como plataforma de desenvolvimento

**📅 Data:** 2025
**🚦 Status:** ✅ Aceita

### 💡 Contexto
O projeto é de caráter acadêmico na disciplina de Fundamentos de Design de Sistemas.
Era necessária uma plataforma que permitisse criar um app Android funcional com curva de
aprendizado baixa, sem exigir conhecimento de linguagens nativas como Kotlin ou Java.

### 🚀 Decisão
Utilizar o **Kodular** — plataforma visual de desenvolvimento baseada em blocos — para
implementar toda a lógica e interface do aplicativo.

### 📈 Consequências

**✅ Vantagens:**
* Não requer escrita de código nativo — toda a lógica é construída em blocos visuais
* Compilação direta para APK Android sem configuração de ambiente local
* Ideal para projetos acadêmicos de curta duração com foco em produto funcional

**⚠️ Desvantagens/Riscos:**
* Sem código-fonte exportável — o projeto fica vinculado à plataforma Kodular
* Limitações de customização visual em relação a frameworks nativos
* Escalabilidade restrita para funcionalidades mais complexas

---

## 🏛️ ADR-002 — Prototipagem no Figma antes da implementação

**📅 Data:** 2025
**🚦 Status:** ✅ Aceita

### 💡 Contexto
Para garantir consistência visual e validar o fluxo de navegação antes de implementar
no Kodular, era necessário uma ferramenta de prototipagem de interface.

### 🚀 Decisão
Utilizar o **Figma** para projetar o protótipo de alta fidelidade do app antes da
implementação, seguindo o processo de Design → Protótipo → Implementação.

### 📈 Consequências

**✅ Vantagens:**
* Validação do fluxo de navegação sem precisar compilar o app
* Separação clara entre fase de design e fase de implementação
* Protótipo reutilizável como referência visual durante o desenvolvimento no Kodular

**⚠️ Desvantagens/Riscos:**
* Manutenção manual da sincronia entre Figma e Kodular (mudanças no design precisam ser replicadas)

---

## 🏛️ ADR-003 — Distribuição via APK direto no repositório

**📅 Data:** 2025
**🚦 Status:** ✅ Aceita

### 💡 Contexto
O app precisa ser compartilhado e avaliado sem necessidade de publicação em loja oficial.
A cada iteração de desenvolvimento uma nova versão do app era gerada.

### 🚀 Decisão
Distribuir o aplicativo como arquivos `.apk` commitados diretamente no repositório GitHub,
com nomenclatura versionada (`v1` → `v4`) para rastrear a evolução do projeto.

### 📈 Consequências

**✅ Vantagens:**
* Instalação imediata em qualquer dispositivo Android com "Fontes desconhecidas" ativado
* Versionamento claro no próprio repositório — cada APK representa uma iteração entregue
* Sem dependência de conta de desenvolvedor na Play Store

**⚠️ Desvantagens/Riscos:**
* Tamanho do repositório aumenta a cada APK adicionado
* Usuário precisa permitir instalação de fontes desconhecidas no dispositivo
