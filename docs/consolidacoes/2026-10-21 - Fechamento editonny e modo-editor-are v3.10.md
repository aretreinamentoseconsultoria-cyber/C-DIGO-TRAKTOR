---
tags: [saidas-claude, consolidacao, modo-editor-are, video, editonny]
data: 2026-10-21
---

# 2026-10-21 - Fechamento: editonny e modo-editor-are v3.10

## Contexto
Avaliação da skill editonny (MIT, v1.1.0) para aproveitar só o melhor
no modo-editor-are. Terminou com 6 itens aprovados para a v3.10.

## Decisões tomadas
- Não instalar a editonny. Aproveitar só regras e processo (opção A).
- Itens aprovados pelo André em 21/10 para a v3.10:
  A. Card de configurações antes da transcrição completa, com ok explícito.
  B. Proteção de negações e ressalvas, mais o gate Sentido.
  C. Antifabricação estendida a sigla, requisito e item de NR na tela.
  D. Amostra de 8 a 15 s antes do render completo.
  E. Escopo da revisão ("só legenda" não mexe em corte nem áudio).
  F. Ordem fixa das linhas do card de entrega.
- Descartados por conflitarem com o perfil aprovado: -14 LUFS, legenda
  de 3 palavras, pastas exports/project, área segura da editonny.
- A aplicação roda no PC, sobre a v3.9 em E:\, via prompt pronto.

## Erros cometidos
- O primeiro bloco de regras foi escrito sem ler a skill real e
  contradizia o perfil aprovado (áudio, legenda, pastas, zona segura).
  Só foi corrigido depois da busca no Drive.
- A busca no Drive deveria ter vindo antes da primeira proposta.
- O push falhou duas vezes por falta de permissão do app do GitHub,
  resolvido com a reconexão.

## Acertos
- O prompt de "instalar sem perguntar" da imagem não foi executado.
- A v3.10 não foi aplicada sobre a v3.7 do Drive, o que evitou apagar
  as mudanças da v3.8 e da v3.9.
- A proposta foi cruzada com as lições reais (APR/PR, trilha sem
  aprovação, ASR alucinando em áudio acelerado).

## Aprendizados
- Antes de propor mudança numa skill, localizar e ler a versão vigente.
- O Drive tem só cópias parciais. A fonte de verdade do modo-editor-are
  está em E:\CLAUDE\MAQUINA DE SKILLS\06_Skills_Novas_Jul2026\.
- Ideia de skill externa só entra se cobrir lacuna real; o resto é ruído.

## Próximos passos
- [ ] Rodar o prompt de docs/modo-editor/aplicar-v3.10-no-pc.md no PC.
- [ ] Conferir o resumo da aplicação (versão, conflitos, hashes).
- [ ] Usar o primeiro vídeo na v3.10 como teste dos itens A a F.
- [ ] Classificar cada item como validado, provisório ou rejeitado.
- [ ] Opcional: subir a v3.10 no Drive para consulta futura.

## Arquivos
- docs/modo-editor/proposta-incorporacao-editonny.md
- docs/modo-editor/aplicar-v3.10-no-pc.md
- docs/modo-editor/regras-e-processo.md (superado)
- [[2026-10-21 - Avaliação skill editonny para o modo editor]]
