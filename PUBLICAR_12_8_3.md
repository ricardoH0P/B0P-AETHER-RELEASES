# Publicar B0P AETHER 12.8.3 R2

**Canal stable atual:** 12.5.3. **Próxima versão:** 12.8.3 R2.

## Identificação exata do Release

- **Tag:** `v12.8.3`
- **Título:** `B0P AETHER 12.8.3 R2 — Navegação sem Bloqueios`
- **Asset a anexar:** `B0P_AETHER_Setup_12_8_3.exe`
- **Pre-release:** não, depois de validado no Windows
- **Latest release:** sim, depois de anexado o instalador e confirmada a versão

O pacote `B0P_AETHER_12_8_3_R2_GITHUB_COMPLETO.zip` foi recebido para publicação. Confirmar que o executável incluído foi gerado a partir das fontes R2; **não renomear um setup anterior** nem publicar o ZIP de fontes no canal público.

## Testes antes de publicar

1. Instalar o executável em Windows e confirmar a versão 12.8.3.
2. Testar o X do Setup e a barra superior com o ícone original.
3. Em Sistema → Windows, alternar rapidamente entre Segurança e Personalizado; o scroll não pode prender nem ativar outra categoria.
4. Confirmar que o Dashboard e os módulos anteriores se mantêm.
5. Verificar que a app não requer desativar antivírus ou proteção de jogos.

## Hash do instalador

No PowerShell, com o caminho correto do instalador:

```powershell
$setup = "CAMINHO_COMPLETO_DO_B0P_AETHER_Setup_12_8_3.exe"
if (!(Test-Path -LiteralPath $setup)) { throw "Setup nao encontrado" }
(Get-FileHash -LiteralPath $setup -Algorithm SHA256).Hash.ToLowerInvariant()
```

## Publicação no GitHub

Criar a tag e o título acima, anexar `B0P_AETHER_Setup_12_8_3.exe` e guardar o Release. Depois verificar que o asset está acessível em:

`https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/download/v12.8.3/B0P_AETHER_Setup_12_8_3.exe`

## Atualização de stable.json — só após o anexo existir

Substituir o manifesto *inteiro* pelo JSON abaixo, **apenas depois de obter o SHA-256 real e confirmar o URL público**. Nunca publicar o valor ilustrativo de SHA-256:

```json
{
  "version": "12.8.3",
  "setup_url": "https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/download/v12.8.3/B0P_AETHER_Setup_12_8_3.exe",
  "sha256": "SUBSTITUIR_PELO_SHA256_REAL",
  "notes": "B0P AETHER 12.8.3 R2 — melhorias de alinhamento da barra superior e do Setup, correção da navegação e do scroll sem bloqueios prolongados. Instalação mediante confirmação."
}
```

**O `stable.json` mantém-se em 12.5.3 até esta publicação estar pronta.**

## Teste final na aplicação

Na versão anterior: **Procurar atualização → Descarregar e Instalar**. Verificar URL, SHA-256, confirmação do utilizador, instalação efetiva e versão após reiniciar a app.

O código-fonte é privado, em `ricardoH0P/B0P-OPTIMIZOR`; não o anexar ao Release público. O SHA-256 verifica a integridade em relação ao manifesto, mas não equivale a uma assinatura digital.
