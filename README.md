# B0P AETHER — Atualizações oficiais

Este repositório público distribui os instaladores da **B0P AETHER** por GitHub Releases e anuncia atualizações através de [stable.json](stable.json). O código-fonte de desenvolvimento e os dados pessoais não são distribuídos neste repositório.

## Atualização atual — B0P AETHER 13.2.8.6 / Gaming R8.2 Full

- **Versão do atualizador:** `13.2.8.6`
- **Tag real da release:** `13_2_8_6`
- **Instalador:** `B0P_AETHER_Setup_13_2_8_6_FULL.exe`
- **Tamanho do asset no GitHub:** 346755965 bytes (330,7 MiB)
- **SHA-256 do asset (GitHub):** `61a41502f8cebbc81e58f5b39ec1070226f16b358823e6ec7ee3daffe35f8b0e`
- **Release:** https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/13_2_8_6
- **Download:** https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/download/13_2_8_6/B0P_AETHER_Setup_13_2_8_6_FULL.exe

A tag da release difere da versão numérica por uma questão de nomenclatura. O atualizador compara a versão do `stable.json` com a versão instalada, e valida o SHA-256 do Setup descarregado antes da instalação.

### O que mudou

- Menu **HUD/FPS** reorganizado para distinguir a sobreposição WPF, a apresentação de FPS e o estado do fornecedor RTSS.
- Removido o bloco redundante de identificação da versão em **Definições → Geral**, mantendo a versão no topo e no rodapé.
- Mantida a leitura real de **PING** (ICMP externo; não equivale à latência do servidor do jogo).
- Mantida a melhoria de leitura de temperatura CPU com o motor de sensores atualizado.
- Setup Full preparado para instalar o benchmark UE5 e os seus recursos juntamente com a B0P, sem downloads manuais depois da instalação.
- Preservados o Dashboard, os restantes módulos e a identidade visual.

### Como testar a atualização

Na B0P AETHER instalada: **Definições → Atualizações → Procurar atualização**. Uma instalação reconhecida com versão inferior a `13.2.8.6` deverá apresentar esta atualização. A instalação exige confirmação do utilizador.

O instalador também pode ser descarregado manualmente pela ligação acima.

### Verificação SHA-256 no PowerShell

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath "$env:USERPROFILE\Downloads\B0P_AETHER_Setup_13_2_8_6_FULL.exe"
```

O hash deve corresponder ao SHA-256 listado acima.

**Limitações de validação:** a presença da release e a integridade do asset estão confirmadas no GitHub, mas o sucesso da atualização pela aplicação, a execução do benchmark UE5 e a compatibilidade com jogos/anti-cheats precisam de testes no Windows. O modo ecrã inteiro exclusivo pode impedir a apresentação de overlays WPF.

## Releases anteriores

- [13.2.8.4 — Full HUD Fix](https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/13_2_8_R2)
- [13.2.8.2](https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/13.2.8)
- [12.8.4 R2](https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/12.8.4.2)

## Segurança e privacidade

Não publicar fontes privadas, backups, históricos pessoais nem credenciais. A verificação SHA-256 confirma integridade relativamente ao manifesto, mas não substitui uma assinatura digital nem garante ausência de falsos positivos.
