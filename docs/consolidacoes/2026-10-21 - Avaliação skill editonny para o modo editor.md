---
tags: [saidas-claude, consolidacao, modo-editor, video, avaliacao-skill]
data: 2026-10-21
---

# 2026-10-21 - Avaliação skill editonny para o modo editor

## Contexto
Avaliação da skill editonny (github.com/soumatheusgomes/editonny, v1.1.0, MIT)
para extrair o que vale incorporar ao modo editor do ecossistema A.R.E.
O objetivo era aproveitar só as melhores partes, sem adotar a skill inteira.

## Decisões tomadas
- Não instalar a editonny. Engine de 504 MB, dependências pesadas e
  manutenção de um único autor.
- Aproveitar as regras de processo e não o código.
- Itens priorizados para incorporar:
  1. Card de configurações com aprovação explícita antes de editar
     (linhas fixas, origem de cada valor, pendências A/B no topo,
     revisão mostrando só o que mudou).
  2. Contrato de limpeza da fala (remover pausas, respirações, erros e
     repetições; preservar negações, ressalvas e palavras completas).
  3. Regra antifabricação: nada de número, depoimento ou item de NR na
     tela sem fonte validada.
  4. Amostra de 8 a 15 s antes do vídeo completo.
  5. Padrões técnicos: legenda com até 3 palavras e área segura no 9:16,
     voz em -14 LUFS e pico de -1 dBTP, nenhum filtro automático.
  6. Pastas exports/ e project/v001/, com versões sem sobrescrever.
  7. Card de entrega e status curto por fase, sem emojis.
- Descartar: engine Python, as 145 cenas genéricas, a checagem de update
  a cada uso, os registros com hash e o tratamento de HDR/VFR.

## Erros cometidos
- O modo editor de referência não foi localizado no ambiente (o repositório
  só tem a landing page e as skills sincronizadas não têm um modo editor).
  A avaliação ficou comparada a um modo editor genérico, não ao real.
- A sessão em nuvem não tinha acesso ao vault nem ao HD E:\.

## Acertos
- O prompt de instalação automática da imagem não foi executado. Ele
  instalaria sem perguntar nada, e o pedido real era uma avaliação.
- Leitura direta da fonte (SKILL.md, WORKFLOW.md, referências do engine)
  antes de concluir.
- Separação clara entre o que aproveitar e o que descartar, com riscos
  (licença dos assets, dependência de autor único, execução local).

## Aprendizados
- O valor da editonny está no processo (confirmar, amostrar, verificar),
  não na tecnologia.
- Em vídeo de SST, cortar uma negação ou ressalva é risco técnico, não só
  estético. A regra de preservar o sentido precisa estar explícita.
- Sem o arquivo do modo editor, toda adaptação fica como suposição.

## Próximos passos
- [ ] André enviar o arquivo ou o caminho do modo editor atual.
- [ ] Definir o escopo: A) só regras e processo (recomendado) ou
      B) regras mais um engine mínimo de corte e legenda com FFmpeg local.
- [ ] Redigir o bloco de incorporação em texto para validação.
- [ ] Após aprovar, gerar a versão final no modo editor.

## Links
- [[Modo Editor]]
- [[Código Traktor]]
