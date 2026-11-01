# B0P AETHER — Atualizações oficiais

Repositório público para distribuir versões **B0P AETHER** através de GitHub Releases e do manifesto `stable.json`. O código-fonte permanece privado.

## Versão disponível pelo atualizador

**Atualmente no canal stable: 12.5.3.**

- [Release 12.5.3](https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/v12.5.3)
- [Manifesto de atualização atual](stable.json)

O `stable.json` contém a versão disponível, URL do instalador, SHA-256 e notas. Só deve anunciar um instalador que esteja realmente acessível e verificado.

## B0P AETHER 12.8.3 R2 — publicação em preparação

**Título a usar no GitHub:** `B0P AETHER 12.8.3 R2 — Navegação sem Bloqueios`

**Tag:** `v12.8.3` • **Ficheiro:** `B0P_AETHER_Setup_12_8_3.exe`.

A versão R2 inclui as melhorias visuais da barra superior e do Setup e a correção da seleção de categorias e do scroll. O pacote de desenvolvimento e instalador foi preparado para revisão, mas esta versão **ainda não está anunciada no canal stable**.

[Consultar passos para publicar a 12.8.3 R2](PUBLICAR_12_8_3.md)

## Ordem correta de publicação

1. Compilar e testar o Setup da versão nova no Windows.
2. Publicar o Release público e anexar o instalador.
3. Confirmar URL e SHA-256 do executável publicado.
4. Atualizar `stable.json` apenas com valores reais.
5. Testar a atualização pela própria app.

Não colocar fontes privadas, credenciais, tokens, backups locais ou ficheiros temporários no repositório público. A integridade por SHA-256 não substitui assinatura de código.
