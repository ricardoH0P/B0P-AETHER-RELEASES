# B0P AETHER — Atualizações oficiais

Este é o **repositório público de distribuição** da B0P AETHER. Aqui são publicados apenas manifestos de atualização, instaladores e notas de versão. O código-fonte permanece num repositório privado separado.

## Canal stable

A aplicação consulta [stable.json](stable.json) através de HTTPS para descobrir se existe uma nova versão.

**Estado inicial:** versão `12.4`. Este primeiro manifesto testa apenas a ligação; **não existe qualquer instalador anunciado** e a aplicação não deverá oferecer download nesta fase.

## Publicação de versões futuras

1. Compilar e testar o instalador no Windows.
2. Criar um GitHub Release público com o instalador `.exe`.
3. Verificar o SHA-256 do ficheiro publicado.
4. Atualizar `stable.json` com a versão superior, o URL exato do asset e o SHA-256.
5. Confirmar na app a deteção, o consentimento, a transferência e a instalação.

O SHA-256 verifica integridade relativamente ao manifesto, mas não equivale a uma assinatura de código. Nunca publicar fontes privadas, credenciais, tokens ou backups locais neste repositório.
