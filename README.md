# B0P AETHER — Atualizações oficiais

Este repositório público distribui o instalador da **B0P AETHER** através de GitHub Releases e do manifesto [stable.json](stable.json). O código-fonte de desenvolvimento continua privado.

## Versão atualmente anunciada — B0P AETHER 13.2.8.4 / Gaming R8.2 FULL HUD FIX

- **Versão reportada pelo atualizador:** `13.2.8.4`
- **Tag da release GitHub:** `13_2_8_R2`
- **Asset:** `B0P_AETHER_Setup_13_2_8_R8_2_FULL_HUD_FIX.exe`
- **Tamanho publicado:** 346894720 bytes (330,8 MiB)
- **SHA-256 publicado pelo GitHub:** `6a61f538010d36ce5bff09f434aa842c53d2028073eb857ca3eed27b0b5bfec9`
- **Página da release:** https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/13_2_8_R2
- **Instalador:** https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/download/13_2_8_R2/B0P_AETHER_Setup_13_2_8_R8_2_FULL_HUD_FIX.exe

O manifesto anuncia a versão `13.2.8.4`, mesmo que a tag da release tenha outro formato. Isto é intencional: o atualizador compara a versão numérica do executável com a versão do `stable.json`.

### Alterações incluídas nesta revisão

- Ajuste do HUD para recuperar a prioridade visual quando um jogo em janela sem bordas recebe foco, sem ativar a janela da B0P.
- Consolidação da leitura válida de temperatura CPU para o Gaming.
- Recolha Gaming de CPU, GPU, RAM, VRAM e FPS quando as fontes estão disponíveis.
- Empacotamento Full destinado a incluir o benchmark UE5 e os seus recursos na pasta `Benchmark/UE5`.
- Instalador Windows com Inno Setup, com progresso de instalação.

**Aviso de validação:** o GitHub confirma o asset e o respetivo digest, mas a presença e execução correta de todos os recursos UE5, a visibilidade do HUD e a atualização real precisam de teste no Windows. Um HUD WPF não tem garantia de aparecer em ecrã inteiro exclusivo. Não existe certificação de compatibilidade com anti-cheats.

### Verificar atualizações na B0P

Na aplicação instalada: **Definições → Atualizações → Procurar atualização**. Uma instalação reconhecida com versão anterior a `13.2.8.4` deverá apresentar a atualização e pedir confirmação antes de instalar.

### Verificar SHA-256 do instalador

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath "$env:USERPROFILE\Downloads\B0P_AETHER_Setup_13_2_8_R8_2_FULL_HUD_FIX.exe"
```

O resultado deve coincidir com o SHA-256 apresentado acima. Esta verificação confirma integridade, não é uma assinatura digital de confiança.

### Versões anteriores

- [B0P AETHER 13.2.8.2](https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/13.2.8)
- [B0P AETHER 12.8.4 R2](https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/12.8.4.2)

## Privacidade

Publicar apenas os instaladores e documentação: não colocar código-fonte privado, ficheiros de credenciais, backups, relatórios de benchmark pessoais nem históricos de jogo.
