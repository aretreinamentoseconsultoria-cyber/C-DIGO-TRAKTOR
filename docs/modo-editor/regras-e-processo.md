---
tags: [modo-editor, video, processo, sst]
versao: 1.0
data: 2026-10-21
origem: adaptado da skill editonny (MIT), só regras e processo
---

# Modo Editor: regras e processo

Bloco de regras para edição de vídeo no ecossistema A.R.E. (Código Traktor, Kit NR-01, Trilha NR-10, TraktorDash). Define o fluxo, o que pode e o que não pode ser feito e como aprovar e entregar. Não depende de ferramenta específica.

## 1. Fluxo obrigatório

Todo trabalho novo de edição segue esta ordem, sem pular etapas:

1. **Inspecionar** os vídeos indicados: duração, formato, orientação, áudio e quadros do início, meio e fim. Nesta etapa nada é alterado, criado ou transcrito por completo.
2. **Apresentar o card de configurações** (seção 2).
3. **Aguardar o "ok" explícito** do André em uma mensagem seguinte. O pedido inicial nunca vale como aprovação de si mesmo, mesmo que seja detalhado ou diga "decida tudo".
4. **Editar** dentro do que foi aprovado.
5. **Gerar e revisar uma amostra** de 8 a 15 segundos (seção 5).
6. **Gerar o vídeo completo.**
7. **Verificar** o arquivo final (seção 9).
8. **Entregar** com o card de entrega (seção 10).

Pergunta antes da inspeção só quando não houver vídeo indicado, e apenas para pedir os arquivos ou a pasta. Todas as outras dúvidas vão para o card, não para perguntas soltas.

**Escopo:** o pedido define o alcance. Um pedido "só legenda" não recorta a fala nem mexe no áudio. Uma revisão de um trecho não altera o resto do vídeo.

## 2. Card de configurações

O card é a decisão inteira do André e precisa ser lido em poucos segundos. As linhas são fixas e ficam sempre na mesma ordem, para facilitar a comparação entre versões.

**Modelo:**

```
### [Título do vídeo]: configurações para aprovar

[Uma frase dizendo o que será feito.]

**Pendências para decidir**
- [Problema encontrado]. **A)** [opção recomendada] · **B)** [alternativa]

**Configurações**
- **Objetivo**: [escopo, ritmo, duração aproximada] (você pediu)
- **Vídeos**: [arquivos e ordem] (da sua pasta)
- **Limpeza**: [o que sai e o que fica] (sugerido)
- **Legendas**: [ligadas ou desligadas, estilo, posição, arquivo SRT] (sugerido)
- **Conteúdo técnico**: [itens de NR, números ou dados que vão aparecer na tela e a fonte de cada um] (sugerido)
- **Som**: [volume da voz, música, efeitos] (sugerido)
- **Elementos visuais**: [cenas, textos de apoio, transições] (sugerido)
- **Imagem**: aparência original, sem filtro (sugerido)
- **Formato**: [9:16, 16:9 etc., sem corte] (do seu vídeo)
- **Revisão**: [quem aprova a amostra] (sugerido)
- **Entrega**: [pasta e nome do arquivo] (sugerido)

Responda **A** para começar, ou diga o que mudar. Exemplos: "sem legenda", "manter a pausa em 0:42", "cortar a abertura".
```

**Regras do card:**
- **Origem de cada valor:** toda linha diz de onde veio o valor: "(você pediu)", "(do seu vídeo)" ou "(sugerido)". Quando uma parte da linha tem origem diferente, ela recebe a própria marcação.
- **Linhas desligadas:** toda linha aparece, mesmo quando o valor é "desligado", "nenhum" ou "como o original".
- **Pendências:** problemas, conflitos e informações ausentes vão para o topo, com opções A/B e a recomendada em primeiro lugar. Nunca são resolvidos em silêncio. As linhas de configuração já mostram a opção recomendada.
- **Sem pendências:** o bloco some e o card pede **ok**.
- **Linguagem:** simples nas linhas. Valor técnico só aparece quando for necessário para decidir.
- **Aprovação:** um "ok" só vale se responder a todas as pendências. Se faltar resposta, o agente pede só o que falta. Escolher a opção não recomendada conta como alteração.
- **Revisões:** depois de uma alteração, o card volta mostrando só as linhas alteradas, marcadas com [alterado], mais a frase "O restante continua como aprovado.", e espera um novo ok.

## 3. Contrato de limpeza da fala

Vale para toda edição completa, mesmo que o André não liste o que limpar.

**Remover:**
- pausas desnecessárias;
- respirações audíveis;
- erros, falsos começos e gaguejos;
- repetições redundantes.

**Preservar sempre:**
- palavras completas, sem cortar consoantes ou finais;
- pausas intencionais e ritmo natural;
- negações e ressalvas ("não", "nunca", "somente se", "exceto", "desde que");
- o sentido original da fala.

**Proibido:**
- criar uma afirmação nova juntando trechos;
- tirar uma ressalva que muda a orientação de segurança;
- trocar a ordem de falas que altere o sentido;
- aplicar um único limite de silêncio no vídeo inteiro sem ouvir as emendas.

**Critério de SST:** se um corte puder mudar uma orientação de segurança, ele não é feito. Por exemplo, "não entre sem bloqueio" virar "entre sem bloqueio". Na dúvida, o trecho fica e o ponto vai para as pendências do card.

**Outras regras:**
- A gravação manda. O roteiro serve só para conferir a grafia de nomes e termos técnicos, nunca para definir o que foi dito ou o tempo dos cortes.
- A melhor tomada é a mais clara e completa, não necessariamente a última.
- Pedido explícito para manter uma pausa, respiração ou tomada prevalece sobre a limpeza padrão.

## 4. Regra antifabricação e validação técnica

- **Nada inventado na tela:** nenhum número, prazo, item de NR, estatística, depoimento, preço ou resultado aparece sem ter sido fornecido pelo André ou validado na fonte oficial.
- **Item de NR na tela:** antes de aparecer, é conferido no texto vigente da norma. Sem validação, ele não entra e vira pendência no card.
- **Fala do instrutor:** o agente não corrige o conteúdo técnico falado. Se notar uma possível inconsistência com a norma, aponta como pendência e o André decide.
- **Modelos de cena e de texto:** são ilustrativos. Dados de exemplo são trocados por fatos reais ou removidos.
- **Elementos visuais:** não podem mudar o que a pessoa falou.
- **Pessoas e áreas:** rostos de terceiros, crachás, placas, documentos e telas com informação sensível são observados na inspeção e sinalizados no card.

## 5. Amostra antes do vídeo completo

- **Trecho:** um trecho representativo de 8 a 15 segundos, com todos os tratamentos aprovados (cortes, legenda, som, elementos visuais) e a emenda mais difícil, se houver. Vídeo menor que isso vai inteiro.
- **Nada extra:** a amostra não ganha efeito que não foi aprovado.
- **Quem revisa por padrão:**
  - O **André** revisa quando o vídeo mostra conteúdo técnico de NR na tela ou é material de venda.
  - O **agente** revisa nos demais casos e segue sem esperar.
  - O card sempre mostra a escolha, e o André pode trocar.
- **Defeitos:** são corrigidos antes do vídeo completo.

## 6. Padrões técnicos de referência

São valores de partida, propostos no card. A plataforma de destino pode exigir outro valor, e isso é informado no card.

| Item | Padrão |
|---|---|
| Legenda | Fiel à fala, até 3 palavras por vez, contraste alto e tempo suficiente de leitura |
| Posição da legenda | Sem cobrir rosto ou boca. No 9:16 (1080x1920), texto importante dentro da faixa x 140 a 940 e y 230 a 1530. Conferir a interface da plataforma de destino |
| Volume da voz | Cerca de -14 LUFS, pico máximo de -1 dBTP, conferido no arquivo final |
| Música | Desligada por padrão. Quando houver, abaixa sob a voz |
| Efeitos sonoros | Desligados por padrão. Quando houver, só em movimento visível, nunca em toda palavra |
| Imagem | Aparência original. Sem filtro, correção de cor ou "melhoria" automática |
| Formato | O do vídeo original, sem corte, salvo pedido |
| Elementos visuais | Entram junto com a palavra falada (até 0,15 s antes). Uma ideia por vez |

**Estruturas de roteiro de referência:**
- **Vídeo de venda:** gancho, problema, mudança, prova, ação.
- **Aula ou tutorial de SST:** gancho, passos, resultado, ação.

## 7. Organização dos arquivos

```
[Pasta do projeto]/AAAA-MM-DD-titulo/
  exportados/   vídeos finais e legendas de todas as versões
  projeto/v001/ arquivos de trabalho da versão 1
  projeto/v002/ arquivos de trabalho da versão 2
```

- **Originais:** nunca são movidos, apagados ou sobrescritos.
- **Nomes dos finais:** `titulo-v001-final.mp4`, `titulo-v002-final.mp4`. Nenhuma versão sobrescreve outra.
- **Arquivos intermediários:** ficam só em `projeto/`.
- **Pasta raiz:** o caminho é proposto na linha "Entrega" do card e validado antes de criar qualquer coisa.

## 8. Comunicação durante o trabalho

- **Andamento:** uma linha curta por fase, com estimativa quando houver. Por exemplo: "Transcrevendo", "Cortando", "Revisando a amostra", "Gerando o vídeo final".
- **Sem ruído:** nada de comando, log ou caminho interno nas mensagens.
- **Sem emojis.**

## 9. Verificação antes de entregar

O arquivo final é conferido em movimento. Um quadro parado não prova sincronia nem emenda.

**Checklist:**
- [ ] O vídeo reproduz do início ao fim
- [ ] A duração está coerente com o aprovado
- [ ] A voz está audível e sem estouro
- [ ] Nenhuma palavra foi cortada nas emendas
- [ ] Negações e ressalvas continuam no vídeo
- [ ] A legenda está fiel, legível e sem cobrir o rosto
- [ ] Os itens técnicos na tela batem com a fonte validada
- [ ] O formato e o nome do arquivo estão corretos

Item não verificado é declarado em "Limites" no card de entrega. Ele nunca é dado como verificado.

## 10. Card de entrega

```
### Vídeo pronto

- **Vídeo**: [caminho do arquivo final]
- **Arquivos de edição**: [pasta projeto/] (guarde para pedir alterações)
- **O que mudou**: [duração antes e depois] · [quantidade de pausas e repetições removidas] · [legendas, elementos visuais]
- **Verificado**: [reprodução, volume da voz, legendas, enquadramento, emendas dos cortes]
- **Limites**: [o que não pôde ser verificado ou foi contornado; a linha some se não houver]

Quer alterar algo? Exemplos: "legenda maior", "cortar a abertura".
```

## 11. Quando algo falhar

- **Erro técnico:** o problema é do agente, não do André. Ele busca outro caminho e registra o contorno em uma linha no card de entrega.
- **Sem caminho possível:** a etapa para e o agente apresenta opções concretas, como a versão sem aquele efeito. Uma configuração aprovada nunca é abandonada em silêncio.
- **Nunca:** pular uma verificação, dar como verificado o que não foi conferido ou entregar por cima de uma versão anterior.

## Histórico

- **1.0 (2026-10-21):** primeira versão, adaptada das regras de processo da skill editonny. Ver [[2026-10-21 - Avaliação skill editonny para o modo editor]].
