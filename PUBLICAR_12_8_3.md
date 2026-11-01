# Publicar B0P AETHER 12.8.3

**Estado:** a versão 12.8.3 ainda não está publicada no canal stable. A versão pública atual é 12.5.3.

## 1. Compilar e validar em Windows

Usar o pacote de desenvolvimento `B0P_AETHER_12_8_3_TOPBAR_E_SETUP_FIX.zip` e executar o seu `INSTALAR_POR_POWERSHELL.ps1`. A compilação requer .NET 10 SDK e o pacote UE5 indicado nas instruções de desenvolvimento. Confirmar que a compilação terminou sem erros e testar o instalador em Windows.

**Não publicar apenas o ZIP de fontes como se fosse um instalador.**

## 2. Preparar o instalador

O ficheiro a publicar é `B0P_AETHER_Setup_12_8_3.exe`, gerado na pasta RELEASE da compilação **12.8.3**. Confirmar visualmente o cabeçalho, ícone B0P existente, versão, botão X do Setup e atualização da aplicação instalada. Evitar publicar um Setup de versões anteriores com nome mudado.

No PowerShell, obter o hash:

```powershell
$setup = "CAMINHO_COMPLETO_DO_SETUP_12_8_3.exe"
if (!(Test-Path -LiteralPath $setup)) { throw "Setup nao encontrado" }
(Get-FileHash -LiteralPath $setup -Algorithm SHA256).Hash.ToLowerInvariant()
```

## 3. Publicar o Release

Criar um novo release no GitHub com a tag `v12.8.3`, nome `B0P AETHER 12.8.3` e anexar `B0P_AETHER_Setup_12_8_3.exe` como asset público. Validar o download pelo endereço exato:

`https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/download/v12.8.3/B0P_AETHER_Setup_12_8_3.exe`

## 4. Atualizar stable.json APENAS após confirmar o asset

Preservar o formato do manifesto. Substituir `COLOCAR_SHA256_REAL` pelo hash do Setup **publicado**.

```json
{
  "version": "12.8.3",
  "setup_url": "https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/download/v12.8.3/B0P_AETHER_Setup_12_8_3.exe",
  "sha256": "COLOCAR_SHA256_REAL",
  "notes": "B0P AETHER 12.8.3: cabeçalho renovado, versão visível, controlo X do Setup corrigido e preservação das funcionalidades anteriores."
}
```

## 5. Testar atualização automática

Na app antiga: **Procurar atualização → Descarregar e Instalar**. Confirmar o SHA-256, pedido de confirmação, atualização efetiva da versão e ausência de instaladores desnecessários em cache. Manter a versão anterior no manifesto se algum teste falhar.

**Não divulgar credenciais nem publicar código-fonte privado no repositório público.**
