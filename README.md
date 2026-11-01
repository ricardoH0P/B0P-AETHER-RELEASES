# B0P AETHER — Atualizações oficiais

Repositório público de distribuição da **B0P AETHER**. Aqui ficam o manifesto `stable.json`, as notas de versão e os instaladores Windows disponibilizados em **GitHub Releases**.

## Canal stable — versão publicada

**Versão atualmente disponível para atualização automática:** `12.5.3`.

- [Descarregar o instalador estável 12.5.3](https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/v12.5.3)
- [Consultar o manifesto de atualização](stable.json)

A aplicação consulta `stable.json` por HTTPS. Só anuncia um update quando o instalador correspondente já está publicado, acessível e com o hash SHA-256 verificado.

## Próxima versão em preparação — 12.8.3

A B0P AETHER **12.8.3 — Topbar e Setup Fix** inclui, nas fontes de desenvolvimento, melhorias da barra superior, indicação da versão, alinhamento dos controlos e botão de fechar do instalador, preservando a identidade B0P e o Dashboard.

**Estado: ainda não publicada para download automático.** A entrega de desenvolvimento é um ZIP com código e scripts, não um `Setup.exe` compilado. A 12.8.3 só deverá aparecer na aplicação depois de o instalador Windows ter sido compilado, testado e publicado como asset no Release `v12.8.3`.

Ver [passos de publicação da 12.8.3](PUBLICAR_12_8_3.md).

## Regras de publicação

1. Compilar em Windows e testar o instalador `B0P_AETHER_Setup_12_8_3.exe`.
2. Criar um Release público `v12.8.3` com esse ficheiro anexado.
3. Calcular e confirmar o SHA-256 do instalador exato publicado.
4. Só então atualizar `stable.json` com `version`, `setup_url`, `sha256` e `notes`.
5. Confirmar na aplicação a deteção, descarregamento, verificação, confirmação e instalação.

**Segurança:** este repositório não deve incluir fontes privadas, credenciais, tokens, backups locais ou ficheiros de depuração. O SHA-256 verifica a integridade em relação ao manifesto, mas não substitui uma assinatura de código.
