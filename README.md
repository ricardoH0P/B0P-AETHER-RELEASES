# B0P AETHER — Atualizações oficiais

Este repositório público distribui os instaladores da **B0P AETHER** através de GitHub Releases e do manifesto `stable.json`. O código-fonte mantém-se privado no repositório de desenvolvimento.

## Canal stable — B0P AETHER 12.8.4 R2

<https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/12.8.4.2>

- **Versão do atualizador:** `12.8.4.2`
- **Nome da Release:** `B0P AETHER 12.8.4 R2`
- **Tag real:** `12.8.4.2` (sem o prefixo `v`)
- **Asset oficial:** `B0P_AETHER_Setup_12_8_4_R2.exe`
- **Download:** <https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/download/12.8.4.2/B0P_AETHER_Setup_12_8_4_R2.exe>
- **SHA-256 apresentado pelo GitHub:** `2e7fc6c18d202f330e7bbe37cf7242fe96d52b6f3e3c4bae501fa471bb252534`

A aplicação consulta [stable.json](stable.json) para obter a versão, o endereço do instalador, o hash e as notas. O manifesto só foi atualizado após a confirmação da Release pública e do asset correspondente.

## Alterações principais

- Recuperação do acesso ao laboratório de benchmarks em **B0P AI → Benchmarks**, usando os testes já existentes (UE5, CS2, GPU, CPU e RAM).
- Ligação do indicador de utilização GPU do Dashboard à telemetria NVIDIA disponível, sem inventar valores quando falta um sensor.
- Reorganização da **Rede**: secção **Velocidade** para testes de download/upload, ping e jitter; **Adaptadores** como inventário próprio em vez da duplicação com QoS.
- Preservação do visual da aplicação e do comportamento de confirmação para testes e alterações.

O GitHub confirma a presença e o SHA-256 do asset, mas isso **não substitui testes de instalação e regressão num computador Windows**. Os testes de velocidade podem consumir dados de rede; executa-os deliberadamente.

[Consultar o registo da publicação 12.8.4 R2](PUBLICAR_12_8_4_R2.md).

## Regras de segurança

O repositório público contém instaladores, manifestos e notas, não código privado, credenciais, backups locais ou fontes completas. Verifica o SHA-256 do ficheiro descarregado antes de executar o instalador. SHA-256 confirma a integridade em relação ao manifesto, não constitui uma assinatura digital do fabricante.

### Versão anterior

[B0P AETHER 12.8.3](https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/12.8.3) — [registo de publicação](PUBLICAR_12_8_3.md).
