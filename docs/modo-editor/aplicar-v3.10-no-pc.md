---
tags: [modo-editor, modo-editor-are, video, aplicacao]
data: 2026-10-21
status: pronto para rodar no Claude Code do PC do André
origem: proposta-incorporacao-editonny.md (itens A a F aprovados pelo André em 21/10/2026)
---

# Aplicar a v3.10 do modo-editor-are no PC

A versão vigente (v3.9) só existe em `E:\CLAUDE\MAQUINA DE SKILLS\06_Skills_Novas_Jul2026\modo-editor-are\`. Aplicar sobre a cópia do Drive (v3.7) apagaria o que mudou na v3.8 e na v3.9. Por isso a aplicação roda no PC.

**Como usar:** abra o Claude Code no PC, com o HD E: conectado, e cole o prompt abaixo inteiro.

---

## Prompt

```
Aplique na skill modo-editor-are os itens A a F abaixo, aprovados por mim em 21/10/2026. Não me pergunte nada que esteja respondido aqui.

Origem editável: E:\CLAUDE\MAQUINA DE SKILLS\06_Skills_Novas_Jul2026\modo-editor-are\
Réplicas: C:\Users\andre\.claude\skills\modo-editor-are\ e E:\CLAUDE\CODEX_HOME\skills\modo-editor-are\

Passos:
1. Confirme que a origem está na v3.9 (cabeçalho do SKILL.md). Se não estiver, pare e me avise.
2. Arquive a v3.9 inteira em _arquivo\v3.9-2026-10-21\ na origem, como nas versões anteriores. Não apague nada.
3. Aplique os itens A a F na origem. Para cada item, localize o trecho pelo sentido, não pelo número: a numeração pode ter mudado na v3.9. Se a v3.9 já cobrir um item, não duplique: registre "já coberto" e siga.
4. Mantenha todas as regras da v3.9 que conflitarem com estes itens e me avise do conflito (exemplo: a v3.9 define sem trilha como padrão, então o card mostra "Trilha: sem trilha (padrão da skill)").
5. Atualize o cabeçalho para versão 3.10, de 21/10/2026, com uma linha sobre o que mudou e o caminho do arquivo da v3.9.
6. Registre cada item aplicado como "não testado" na referência de aprendizado ou de gates, conforme a seção Aprendizado da skill.
7. Copie a origem para as duas réplicas e confira por hash SHA256 que as três estão idênticas.
8. Valide o frontmatter (name e description) e confirme que nenhuma referência aponta para arquivo inexistente.
9. Termine com um resumo: versão, itens aplicados, itens já cobertos, conflitos encontrados, hashes e se preciso reabrir o Claude Code ou o Codex.

ITEM A. Card de configurações (seção Ativação, depois do item que manda perguntar só o dado ausente)
Antes da transcrição completa, apresente o card de configurações e espere a resposta do André em mensagem separada. O pedido inicial não aprova o próprio card. O card tem linhas fixas, sempre na mesma ordem: Objetivo e destino, Vídeos, Duração-alvo, Legenda, Trilha e efeitos, CTA, Zona, Entrega, Revisão. Cada valor leva a origem: (você pediu), (do bruto) ou (padrão da skill). O que estiver em aberto ou em conflito vai para o topo como pendência, com opções A e B e a recomendação. Um "ok" só vale se responder a todas as pendências. Depois de uma alteração, mostre só as linhas alteradas e a frase "O restante continua como aprovado."

ITEM B. Proteção de negações e ressalvas (contrato de execução, item de suficiência narrativa)
Nenhum corte remove ou separa negação, ressalva ou condição ("não", "nunca", "sem", "somente se", "exceto", "desde que", "a não ser") da frase que ela altera. Nenhum corte junta trechos que, emendados, formem uma afirmação que o André não fez. Na dúvida, o trecho fica e entra como pendência na decupagem.
Gate novo em gates-e-erros.md, chamado Sentido: a decupagem lista as negações e ressalvas de cada trecho aprovado, e o gate confere a lista contra a legenda final. Divergência vai para a lista de segundos de risco e não reprova sozinha, porque o ASR alucina em áudio acelerado.

ITEM C. Antifabricação estendida a NR (contrato de execução, item da legenda literal e do texto adicional)
Número, sigla, requisito ou item de NR que aparece na tela (legenda, rótulo de animação, cartão de tema, CTA) só entra com fonte conferida no texto vigente da norma ou confirmação do André. Em instrução do tipo "escrito X e não Y", confirme qual forma é a desejada antes de mexer. Em divergência entre o ASR e o André, vale o André.

ITEM D. Amostra antes do render completo (contrato de execução, antes dos gates)
Antes do render completo, renderize uma amostra de 8 a 15 s com todos os tratamentos aprovados (cortes, legenda, cartão, efeitos e nível), incluindo a emenda mais difícil. Rode nela os gates aplicáveis. Só depois renderize a peça inteira.

ITEM E. Escopo da revisão (contrato de execução, item do registro da rodada)
Um pedido de revisão vale só para o que foi pedido. "Só legenda" não recorta fala nem mexe no áudio. Revisão de um trecho não altera o resto da peça. Se a mudança pedida obrigar outra alteração, ela entra como pendência antes do render.

ITEM F. Ordem do card de entrega (contrato de execução, item da entrega)
A entrega segue esta ordem de linhas: Vídeo (caminho), O que mudou (duração antes e depois, cortes), Verificado (gates que passaram), Ouvir (segundos de risco), Limites.
```

---

## Depois de rodar

- **Confirmação:** cole o resumo final aqui na conversa para eu conferir.
- **Teste:** o primeiro vídeo editado com a v3.10 é o teste dos itens. Ao fim dele, os itens passam de "não testado" para validado, provisório ou rejeitado.
