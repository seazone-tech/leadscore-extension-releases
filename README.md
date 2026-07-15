# leadscore-extension-releases

Distribuicao self-hosted da extensao Chrome **Leadscore Marketplace** (pre-venda do funil 37).

- **Extension ID:** `obhpjmidkcpnehhmbaljedlibeaomjfj`
- **Update URL:** `https://leadscore-ext.seazone.properties/update.xml`
- **Pacote:** `https://leadscore-ext.seazone.properties/leadscore-marketplace.crx`
- **Codigo-fonte:** [seazone-tech/leadscore-marketplace](https://github.com/seazone-tech/leadscore-marketplace) (pasta `extension/`)

## Distribuicao (Google Admin Console)

Admin Console > Dispositivos > Chrome > Apps e extensoes > Usuarios e navegadores >
Adicionar > **Adicionar pelo ID da extensao (fora da Chrome Web Store)**:

- ID: `obhpjmidkcpnehhmbaljedlibeaomjfj`
- URL de instalacao (update URL): `https://leadscore-ext.seazone.properties/update.xml`
- Politica: instalacao forcada

## Publicar nova versao

1. Bump `version` no `manifest.json` da extensao (repo leadscore-marketplace).
2. Empacotar o `.crx` assinado com a chave persistente (`leadscore-ext.pem`, guardada fora do repo — NUNCA commitar).
3. Substituir `leadscore-marketplace.crx` aqui e atualizar `version` no `update.xml`.
4. Commit + push na `main` — o Coolify redeploya a app estatica e o Chrome atualiza sozinho (checagem periodica).
