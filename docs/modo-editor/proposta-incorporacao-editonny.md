---
tags: [modo-editor, modo-editor-are, video, proposta, editonny]
data: 2026-10-21
status: aprovado pelo André em 21/10/2026 (itens A a F); aplicação em aplicar-v3.10-no-pc.md
alvo: skill modo-editor-are (vigente v3.9, aprovada em 09/10/2026)
---

# Proposta de incorporação ao modo-editor-are (aprendizados da editonny)

## Base desta proposta

Lido no Google Drive em 21/10/2026:
- `SKILL.md` do `modo-editor-are` **v3.7** (pasta `_BUILD_MODO_EDITOR_3_7`, 26/09/2026);
- `00_PADRAO_EDICAO_DE_VIDEO.md` (modificado em 05/10/2026);
- `LICOES_PARA_MODO_EDITOR.md` (projeto agentes trabalhando, 06/10/2026);
- `decisao-2026-10-09-agentes-pop-sem-trilha-e-finais.md` e `erro-2026-10-09-agentes-pop-capcut-apr-e-ordem-dos-segmentos.md`.

**Limite:** a versão vigente é a **v3.9**, que está em `E:\CLAUDE\MAQUINA DE SKILLS\06_Skills_Novas_Jul2026\modo-editor-are\` e não está no Drive. O que a v3.9 mudou só aparece aqui pelas notas de decisão e de erro. Antes de aplicar, conferir cada item contra a v3.9.

Pela regra da própria skill, nenhuma observação vira regra sem aprovação explícita do André. Tudo abaixo é proposta.

## 1. O que sai do rascunho anterior (a skill já cobre melhor)

O arquivo `regras-e-processo.md` foi escrito sem acesso à skill. Ao comparar, estes itens conflitam com o perfil aprovado ou repetem regras já validadas, e **não devem entrar**:

| Item do rascunho | O que o modo-editor-are já define | Decisão |
|---|---|---|
| Pastas `exportados/` e `projeto/v001/` | Bruto em `VIDEO PARA EDIÇÃO`, projeto em `trombino-kit-edicao-ia\video-projects`, versão final na raiz de `EDIÇÃO DE VIDEO`, intermediárias para a Lixeira | Descartar |
| Voz em -14 LUFS | Trilha perto de 20 dB abaixo da voz; nivelamento por trecho em -17 LUFS provisório; **sem trilha como padrão** desde a v3.9 | Descartar |
| Legenda com até 3 palavras | Karaokê palavra a palavra, até 2 linhas, Montserrat ExtraBold, altura de maiúscula de 61 px, cores aprovadas em 26/09 | Descartar |
| Área segura x 140 a 940, y 230 a 1530 | Zona por destino: Reel orgânico pelo vault (250 px no topo, 340 px na base, 90 px nas laterais) e anúncio Meta (y 269 a 1248, x 65 a 1015) | Descartar |
| Elementos visuais até 0,15 s antes | Já existe, e só quando o quadro de técnicas da decupagem indicar | Descartar |
| Checklist de verificação | Gates Sincronia, Zona, Rosto, Nível, Efeitos, Técnico e lista de segundos de risco para escuta | Descartar (os gates são mais rigorosos) |
| Preservar originais e versões sem sobrescrever | Regra de retenção do `00_PADRAO` | Já coberto |
| Não publicar sem autorização | Item 14 do contrato de execução | Já coberto |
| Card de entrega | Item 14 do contrato: versão, caminho, duração, decisões, evidências e limites | Já coberto. Ver item F, opcional |

## 2. O que entra (o que a skill ainda não tem)

### A. Card de configurações antes de começar

**Lacuna:** a ativação pede só o dado ausente que muda a entrega, mas não consolida as decisões num lugar só antes do trabalho pesado. Os erros de 09/10 (APR trocado por PR, trilha calibrada em sete versões sem aprovação) começaram com uma premissa não confirmada.

**Onde entra:** seção Ativação, como novo item entre os itens 4 e 5 (renumerar os seguintes).

**Texto proposto:**

> Antes da transcrição completa, apresente o card de configurações e espere a resposta do André em mensagem separada. O pedido inicial não aprova o próprio card. O card tem linhas fixas, sempre na mesma ordem: Objetivo e destino, Vídeos, Duração-alvo, Legenda, Trilha e efeitos, CTA, Zona, Entrega, Revisão. Cada valor leva a origem: (você pediu), (do bruto) ou (padrão da skill). O que estiver em aberto ou em conflito vai para o topo como pendência, com opções A e B e a recomendação. Um "ok" só vale se responder a todas as pendências. Depois de uma alteração, mostre só as linhas alteradas e a frase "O restante continua como aprovado."

**Compatibilidade:** não cria pergunta nova. O que o André já informou entra como "(você pediu)" e o resto vem do perfil aprovado.

**Estado:** não testado.

### B. Proteção de negações e ressalvas

**Lacuna:** o contrato preserva reflexão, pausas com função e suficiência narrativa, mas não protege explicitamente palavras que invertem o sentido. Em SST, perder um "não" ou um "somente se" muda a orientação de segurança.

**Onde entra:** contrato de execução, item 4 (suficiência narrativa), e `gates-e-erros.md`.

**Texto proposto para o item 4:**

> Nenhum corte remove ou separa negação, ressalva ou condição ("não", "nunca", "sem", "somente se", "exceto", "desde que", "a não ser") da frase que ela altera. Nenhum corte junta trechos que, emendados, formem uma afirmação que o André não fez. Na dúvida, o trecho fica e entra como pendência na decupagem.

**Gate proposto, Sentido:** a decupagem lista as negações e ressalvas de cada trecho aprovado, e o gate confere a lista contra a legenda final. Divergência vai para a lista de segundos de risco, não reprova sozinha, porque o ASR alucina em áudio acelerado (lição 16 de 06/10).

**Estado:** não testado.

### C. Antifabricação estendida a NR

**Lacuna:** a regra atual cobre número técnico ("número técnico só com fonte conferida"). Ela não cobre sigla, requisito ou item de norma em texto na tela ou em rótulo de animação, que foi onde o erro APR/PR apareceu.

**Onde entra:** contrato de execução, item 6 (legenda literal e texto adicional).

**Texto proposto:**

> Número, sigla, requisito ou item de NR que aparece na tela (legenda, rótulo de animação, cartão de tema, CTA) só entra com fonte conferida no texto vigente da norma ou confirmação do André. Em instrução do tipo "escrito X e não Y", confirme qual forma é a desejada antes de mexer. Em divergência entre o ASR e o André, vale o André.

**Estado:** a segunda frase já foi decidida em 09/10. O resto não foi testado.

### D. Amostra antes do render completo

**Lacuna:** a skill tem o ensaio de enquadramento e a demonstração de legenda, mas não exige um trecho com todos os tratamentos juntos antes do render inteiro. Com 2 núcleos e 7,8 GB de RAM, um render completo errado custa caro.

**Onde entra:** contrato de execução, entre os itens 6 e 13.

**Texto proposto:**

> Antes do render completo, renderize uma amostra de 8 a 15 s com todos os tratamentos aprovados (cortes, legenda, cartão, efeitos e nível), incluindo a emenda mais difícil. Rode nela os gates aplicáveis. Só depois renderize a peça inteira.

**Estado:** não testado. Pode se sobrepor ao ensaio de enquadramento; o André decide se vale como etapa própria.

### E. Escopo da revisão

**Lacuna:** a skill não diz o que uma revisão pontual pode tocar.

**Onde entra:** contrato de execução, item 12 (registro da rodada).

**Texto proposto:**

> Um pedido de revisão vale só para o que foi pedido. "Só legenda" não recorta fala nem mexe no áudio. Revisão de um trecho não altera o resto da peça. Se a mudança pedida obrigar outra alteração, ela entra como pendência antes do render.

**Estado:** não testado.

### F. Formato do card de entrega (opcional)

O item 14 já define o conteúdo. A proposta é só fixar a ordem das linhas para facilitar a leitura: Vídeo (caminho), O que mudou (duração antes e depois, cortes), Verificado (gates que passaram), Ouvir (segundos de risco), Limites. Baixo impacto; aplicar só se o André quiser.

## 3. O que não vem da editonny

Fica de fora, por não ter ganho sobre o que já existe: o engine Python, as 145 cenas genéricas, a checagem de atualização no GitHub, o registro de confirmação com hash de mensagem e o tratamento de HDR/VFR.

## 4. Para aplicar

1. André aprova, ajusta ou rejeita cada item (A a F).
2. Conferir os itens aprovados contra a v3.9, em `E:\CLAUDE\MAQUINA DE SKILLS\06_Skills_Novas_Jul2026\modo-editor-are\`.
3. Aplicar na origem editável, gerar a v3.10 e atualizar as réplicas do Claude Code e do Codex conferidas por hash, como manda o cabeçalho da skill.
4. Registrar os itens aplicados como "não testado" até o primeiro projeto que os exercite.
