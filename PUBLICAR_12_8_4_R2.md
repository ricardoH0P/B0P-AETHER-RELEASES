# Publicação oficial — B0P AETHER 12.8.4 R2

**Data de publicação:** 2026-11-02 (UTC)

## Release verificada

- **Tag:** `12.8.4.2`
- **Título:** `B0P AETHER 12.8.4 R2`
- **Asset:** `B0P_AETHER_Setup_12_8_4_R2.exe`
- **Tamanho do asset:** 552028350 bytes
- **SHA-256 (digest apresentado pela API do GitHub):** `2e7fc6c18d202f330e7bbe37cf7242fe96d52b6f3e3c4bae501fa471bb252534`
- **Release:** https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/12.8.4.2
- **Download:** https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/download/12.8.4.2/B0P_AETHER_Setup_12_8_4_R2.exe

A Release foi confirmada como pública (`draft=false`, `prerelease=false`) e o asset constava como `uploaded` no GitHub.

## Alterações anunciadas

- Laboratório de benchmarks recuperado na navegação da B0P AI.
- Monitorização de utilização GPU no Dashboard a partir de telemetria NVIDIA, quando disponível.
- Menu Rede consolidado: teste de Velocidade (download/upload e medições de latência) e lista única de Adaptadores.
- Mantido o motor de benchmarks existente e o comportamento sem injeção em jogos.

## Manifesto e documentação

Depois de verificar a Release e o digest, os ficheiros `stable.json` e `README.md` foram atualizados para `12.8.4.2`.

Para verificar a integridade do EXE descarregado em Windows PowerShell:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath "$env:USERPROFILE\Downloads\B0P_AETHER_Setup_12_8_4_R2.exe"
```

O valor apresentado deve ser `2e7fc6c18d202f330e7bbe37cf7242fe96d52b6f3e3c4bae501fa471bb252534`. Ajusta o caminho se guardaste o instalador numa subpasta.

**Limitação:** a confirmação do asset/hash não significa que esta publicação tenha sido testada numa instalação Windows limpa; validar instalação, atualizador, benchmark UE5 e regressões de navegação antes de uma divulgação ampla.

## Segurança

O repositório de Releases publica apenas instaladores e documentação. O código-fonte privado, ficheiros locais de configuração e dados do utilizador não devem ser carregados para este repositório.
