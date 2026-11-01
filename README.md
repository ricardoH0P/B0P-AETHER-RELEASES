# B0P AETHER — Atualizações oficiais

Este repositório público distribui os instaladores da **B0P AETHER** por GitHub Releases e o manifesto `stable.json`. O código-fonte mantém-se privado no repositório de desenvolvimento.

## Canal stable — B0P AETHER 12.8.3

<https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/12.8.3>

- **Versão:** `12.8.3` (revisão R2 de navegação e scroll)
- **Asset oficial:** `B0P_AETHER_Setup_12_8_3.exe`
- **Tag real do Release:** `12.8.3` (sem o prefixo `v`)
- **URL de download:** <https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/download/12.8.3/B0P_AETHER_Setup_12_8_3.exe>
- **SHA-256 apresentado pelo GitHub:** `071a9b00de315f7a56a58088f10fb57f42afb5d1fd9953f6265f7e6890a4df90`

A aplicação consulta [stable.json](stable.json) para ler a versão, o URL do instalador, o hash e as notas. O manifesto passou a anunciar a 12.8.3 após confirmar que o Release é público e tem o asset esperado.

## Alterações principais

- Refinamento do cabeçalho, da localização da versão e do botão de fechar do instalador.
- Revisão da navegação por categorias e do scroll para eliminar bloqueios prolongados.
- Preservação do Dashboard, da identidade B0P e dos módulos anteriores.

O GitHub confirma a presença e o SHA-256 do asset, mas isso **não substitui testes de instalação e regressão num computador Windows**. Se uma instalação falhar, suspender a divulgação da versão até resolver a causa.

[Consultar o registo de publicação 12.8.3](PUBLICAR_12_8_3.md).

## Regras de segurança

O repositório público contém instaladores, manifestos e notas, não código privado, credenciais, backups locais ou fontes completas. Confirmar o hash do ficheiro descarregado antes de executar o instalador. SHA-256 verifica a integridade em relação ao manifesto, não a assinatura digital do fabricante.
