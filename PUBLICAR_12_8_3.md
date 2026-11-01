# B0P AETHER 12.8.3 R2 — Publicação

## Estado de publicação

- **GitHub Release:** [12.8.3](https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/12.8.3)
- **Tag efetiva:** `12.8.3` (não `v12.8.3`)
- **Publicado:** 2026-11-01 23:54:45 UTC
- **Asset:** `B0P_AETHER_Setup_12_8_3.exe`
- **Tamanho:** 552 016 058 bytes
- **Download:** <https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/download/12.8.3/B0P_AETHER_Setup_12_8_3.exe>
- **SHA-256 apresentado pelo GitHub:** `071a9b00de315f7a56a58088f10fb57f42afb5d1fd9953f6265f7e6890a4df90`
- **Manifesto:** [stable.json](stable.json), atualizado para a 12.8.3.

O asset está marcado como `uploaded`, e o Release não é rascunho nem pré-lançamento.

## Verificação local recomendada

No PowerShell, após descarregar o Setup.exe:

```powershell
$setup = Join-Path $env:USERPROFILE "Downloads\B0P_AETHER_Setup_12_8_3.exe"
if (!(Test-Path -LiteralPath $setup)) { throw "Instalador nao encontrado: $setup" }
$esperado = "071a9b00de315f7a56a58088f10fb57f42afb5d1fd9953f6265f7e6890a4df90"
$real = (Get-FileHash -LiteralPath $setup -Algorithm SHA256).Hash.ToLowerInvariant()
if ($real -ne $esperado) { throw "SHA-256 nao corresponde ao release!" }
Write-Host "Instalador verificado por SHA-256" -ForegroundColor Green
```

## Checklist de regressão após instalar

1. Confirmar que a aplicação instalada indica 12.8.3.
2. Verificar botão X do Setup e cabeçalho com o ícone B0P original.
3. Testar scroll e cliques rápidos em Segurança e Personalizado e outras categorias.
4. Validar Dashboard, jogos, limpeza, arranque e ferramentas anteriormente funcionais.
5. Testar o fluxo `Procurar atualizações` → `Descarregar` → `Instalar` numa versão anterior.

**Nota:** a presença do asset e o hash do GitHub confirmam a distribuição do ficheiro, não que a instalação tenha sido testada independentemente.
