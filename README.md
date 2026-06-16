# Manuais MeusCorreios

Repositório dedicado aos manuais das integrações do **MeusCorreios**.

## 📘 Manuais disponíveis

<!-- MANUAIS:INICIO -->
- [Integração JetCommerce x MeusCorreios](https://gernd90.github.io/manuais.github.io/integrJetcom/)
- [Integração Shopify x MeusCorreios](https://gernd90.github.io/manuais.github.io/integrShopifyG/)
- [Integração Tray x MeusCorreios](https://gernd90.github.io/manuais.github.io/integrTray/)
- [MeusCorreios Chatbot](https://gernd90.github.io/manuais.github.io/meusCorreiosChatbot/)
<!-- MANUAIS:FIM -->

## CI Pipeline

A cada push na `main`, um workflow (`.github/workflows/atualizar-readme.yml`) varre o repositório em busca de manuais HTML e atualiza a lista acima automaticamente.

- O bot commita o README atualizado com `[skip ci]` para evitar que um segundo deploy do Pages seja disparado e cancele o que foi iniciado pelo push humano.
- O workflow é ignorado quando o autor do push é `github-actions[bot]`, evitando loops.
- O GitHub Pages é publicado pelo workflow interno do GitHub, disparado apenas por commits humanos.
