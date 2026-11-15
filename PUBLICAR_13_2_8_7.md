# B0P AETHER 13.2.8.7 — Gaming R8.2 FULL

Versao de teste para Windows x64.

- Benchmark UE5 completo incluído no Setup, com recursos do motor e executável.
- B0P AI Gaming: monitorização de CPU, GPU, RAM, VRAM e FPS via RTSS quando disponível.
- Histórico de sessões e relatórios; sem inventar FPS quando indisponíveis.
- HUD B0P: controlo mostrar/ocultar. FPS: controlo funcional e dados RTSS so de leitura.
- Definicoes: removida a caixa duplicada de versao da aba Geral.
- Ping de rede ICMP real no HUD, apresentado como PING (nao e o ping do servidor do jogo).
- HUD corrigido para jogos em janela sem bordas, sem roubar foco. Em fullscreen exclusivo a visibilidade do overlay WPF nao e garantida.
- A temperatura CPU da analise Gaming usa a mesma fonte validada do HUD.
- Auxiliar de sensores incluido no Setup: apenas este auxiliar recebe elevacao UAC, quando autorizado no Sensor Doctor.
- Aplicacao principal permanece sem elevacao. Nao instala drivers. Requer um fornecedor de hardware compativel (PawnIO em algumas CPUs).
- Leitura CPU tem validade de 8 segundos; PING usa validade de 12 segundos para falhas ICMP isoladas.
- Instalador Inno Setup com pasta de destino, progresso real, icone B0P, atalhos e desinstalador.

Não altera ficheiros do jogo nem certifica compatibilidade com anti-cheats.
O benchmark só foi validado estruturalmente durante o empacotamento: executar um teste UE5 no Windows após instalar.

---

## Publicação verificada no GitHub

- **Tag:** `13.2.8.7`
- **Publicado em:** 2026-11-15 (UTC)
- **Asset:** `B0P_AETHER_Setup_13_2_8_7_FULL.exe`
- **Tamanho do ficheiro publicado:** `360223149` bytes
- **SHA-256 disponibilizado pelo GitHub:** `0ea42617fee691fc7eb3cef3b36270586c1bacfb16b5916303481b86ec08ca2e`
- **Release:** https://github.com/ricardoH0P/B0P-AETHER-RELEASES/releases/tag/13.2.8.7

A release está publicada e o digest do ficheiro coincide com o `SHA256SUMS.txt` fornecido para esta versão. O funcionamento do auxiliar, HUD, ping e benchmark deve ser validado no Windows antes de a considerar estável.
