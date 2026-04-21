# 📦 Distribuição de App Android (Mobile App Distribution)

## 💡 O que é

Distribuição de app mobile é o processo de disponibilizar um aplicativo para que usuários
possam instalá-lo em seus dispositivos. No ecossistema Android, existem duas formas principais:

**Distribuição oficial** via Google Play Store — requer conta de desenvolvedor, processo de
revisão e publicação pública. É o caminho padrão para apps destinados ao grande público.

**Distribuição direta (sideloading)** via arquivo APK — o Android Package Kit (APK) é o
formato de pacote instalável do Android. Qualquer app Android pode ser compilado como APK
e distribuído manualmente, sem passar pela Play Store. O usuário instala o arquivo
diretamente, desde que permita instalação de "fontes desconhecidas" nas configurações.

O sideloading é amplamente usado em contextos de desenvolvimento, testes, distribuição
corporativa e projetos acadêmicos, onde publicação em loja não é necessária.

## ⚙️ Como é usado neste projeto

O PedePizza é distribuído exclusivamente via APK direto no repositório GitHub. A cada
iteração do desenvolvimento, um novo APK foi compilado pelo Kodular e adicionado ao repo:

| Arquivo                   | Versão | Entrega |
| ------------------------- | ------ | ------- |
| `SotfwarePizzaria.apk`    | v1     | Iteração 1 — fluxo básico |
| `SotfwarePizzaria_v2.apk` | v2     | Iteração 2 — sabores doces |
| `SotfwarePizzaria_v3.apk` | v3     | Iteração 3 — bordas e bebidas |
| `SotfwarePizzaria_v4.apk` | v4     | Iteração 4 — confirmação completa |

## 🔍 Exemplo do projeto

```bash
# Estrutura de distribuição no repositório
app-pizzaria/
├── SotfwarePizzaria.apk      ← v1
├── SotfwarePizzaria_v2.apk   ← v2
├── SotfwarePizzaria_v3.apk   ← v3
└── SotfwarePizzaria_v4.apk   ← v4 (versão final recomendada)
```

Para instalar: baixar o APK → abrir no dispositivo Android → confirmar instalação.

## 📚 Recursos para aprofundamento

- [Android APK — Android Developers](https://developer.android.com/guide/components/fundamentals) — estrutura de um app Android
- [Sideloading APK — Android Authority](https://www.androidauthority.com/how-to-install-apks-31494/) — guia de instalação manual
- [Kodular — Export APK](https://docs.kodular.io/guides/export/) — como exportar o APK pelo Kodular
