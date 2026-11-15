# B0P AETHER — Atualizações oficiais

Este repositório público disponibiliza instaladores da **B0P AETHER** por GitHub Releases e atualizações pela aplicação através de [stable.json](stable.json). O código-fonte de desenvolvimento, backups e históricos pessoais não são publicados aqui.

## Versão anunciada — B0P AETHER 13.2.8.7 / Gaming R8.2 FULL

- **Versão do atualizador:** `13.2.8.7`
- **Tag da release:** `13.2.8.7`
- **Asset do Setup:** `B0P_AETHER_Setup_13_2_8_7_FULL.exe`
- **Tamanho no GitHub:** `360223149` bytes (~343,5 MiB)
- **SHA-256 apresentado pelo GitHub:** `0ea42617fee691fc7eb3cef3b36270586c1bacfb16b5916303481b86ec08ca2e`
- **Release:** https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/13.2.8.7
- **Setup:** https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/download/13.2.8.7/B0P_AETHER_Setup_13_2_8_7_FULL.exe

O `stable.json` contém a versão numérica, o endereço do Setup, a soma SHA-256 e as notas. O atualizador compara a versão instalada com esse manifesto e pede confirmação antes da instalação.

### O que mudou na 13.2.8.7

- **Sensor de temperatura CPU:** auxiliar de sensores incluído, com elevação UAC apenas quando autorizada no Sensor Doctor; a aplicação principal continua com permissões normais.
- **Leituras com validade:** o valor da CPU expira após 8 segundos e o PING ICMP após 12 segundos, evitando apresentar dados antigos indefinidamente.
- **HUD e FPS:** mantém o controlo de mostrar/ocultar, dados FPS do RTSS em modo de leitura quando disponível, e melhorias de visibilidade em janela sem bordas. Não é garantido em ecrã inteiro exclusivo.
- **PING:** medição ICMP real de rede, não latência do servidor do jogo.
- **B0P AI Gaming:** monitorização de CPU, GPU, RAM, VRAM e FPS quando disponíveis, mais histórico e relatórios.
- **UE5:** instalador completo preparado para incluir o executável e os recursos do benchmark.
- **Setup Inno:** escolha da pasta de destino, progresso de instalação, ícone, atalhos e desinstalador.

[Ver notas completas da versão](PUBLICAR_13_2_8_7.md) · [Ver SHA256SUMS](SHA256SUMS.txt)

### Como testar o update pela aplicação

1. Abrir **B0P AETHER → Definições → Atualizações**.
2. Selecionar **Procurar atualização**.
3. Com uma instalação reconhecida e versão inferior a `13.2.8.7`, confirmar a atualização.
4. Depois de instalar, verificar o HUD, a leitura CPU, o PING e o benchmark UE5.

Para verificar a integridade do Setup descarregado:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath "$env:USERPROFILE\Downloads\B0P_AETHER_Setup_13_2_8_7_FULL.exe"
```

O resultado deve corresponder ao SHA-256 acima. Esta verificação não substitui uma assinatura digital de confiança.

**Limites de validação:** confirmei a release e o digest publicados pelo GitHub. A instalação, a atualização pela aplicação, a leitura prolongada dos sensores e a execução do UE5 ainda precisam de ser validadas num PC Windows. A B0P não certifica compatibilidade com anti-cheats nem instala controladores automaticamente.

## Histórico

- [13.2.8.6 — Gaming R8.2 Full](https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/13_2_8_6)
- [13.2.8.4 — HUD Fix](https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/13_2_8_R2)
- [13.2.8.2](https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/13.2.8)

## Privacidade

Não colocar neste repositório código-fonte privado, credenciais, backups, relatórios pessoais ou históricos dos utilizadores.
