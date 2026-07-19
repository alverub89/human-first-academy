# Contrato de Contexto, Projeto PM Moderno (Human First Academy)

> Cole este documento no início de um projeto de IA (Claude Project, GPT, base de conhecimento) antes de pedir qualquer tarefa. Atualize os campos entre [colchetes] quando algo mudar. Este é o mesmo tipo de artefato que o curso ensina.

---

## 1. Objetivo do projeto

Construir e evoluir a landing page (e material) do curso **PM Moderno**, mantendo o posicionamento em dor real e a voz da marca Human First. Toda saída de IA neste projeto deve respeitar as regras de voz da seção 4 e evitar os itens da seção 5.

---

## 2. O produto

- **Curso:** PM Moderno: o trabalho do gerente de produto com IA dentro (Human First Academy).
- **Tese central:** A IA assumiu o trabalho que nunca deveria ter sido do PM (rascunho, exaustão, síntese). O que sobrou (julgamento, contexto, decisão) sempre foi humano.
- **Frase-âncora:** "PM vira curador de decisão, não editor de IA." (Esta é a única exceção autorizada à regra de não usar contraste binário.)
- **Método proprietário:** Método 3D Human First.
  1. **Definir:** enquadrar problema e resultado antes de chamar a IA.
  2. **Instrumentar:** montar contexto e regras que a IA precisa; o contexto vira artefato.
  3. **Decidir:** avaliar a saída com rubrica, expor inferências, bater o martelo.
- **Artefatos proprietários (mencionar sempre pelo nome):**
  - **Contrato de Contexto:** reúne o contexto do produto num formato reutilizável, para a IA e o time não inferirem errado.
  - **Contrato de Execução:** define o que a IA faz, com quais limites e formato; deixa a saída auditável.
  - **Rubrica de Curadoria:** régua objetiva para julgar a saída, sem aprovar o primeiro rascunho.
  - **Checklist de Inferência:** lista o que a IA assumiu sozinha, para nada escondido chegar ao time.
- **Formato:** 15 aulas em vídeo (cerca de 4h), perto de 12h com a prática, assíncrono, projeto final avaliado por rubrica, comunidade fechada.
- **Preço:** R$ 297 (turma de lançamento). Preço cheio de referência: R$ 497.
- **Plataforma de venda:** Hotmart. **Garantia:** 7 dias, motivo único ("se não for para você, devolvemos").
- **Estrutura de cada aula:** Conceito (curto) seguido de Aplicação com IA sobre um artefato real de produto.

---

## 3. Público e dores

Ordem de prioridade:
1. **PMs em transição** (recém-promovidos, vindos de outras áreas), precisam de fundamento sólido.
2. **PMs plenos**, querem método novo sem perder critério.
3. **PMs sêniores e Product Leads**, querem calibrar julgamento na presença de IA.

Dores reais (use estas, não invente novas):
1. Ansiedade de obsolescência sem direção clara (conteúdo raso ou técnico demais, segue entregando do mesmo jeito).
2. Demos de IA que não viram trabalho (saída genérica, inferência escondida, o time não confia, retrabalho).
3. Time desorganizado em torno do contexto (informação na cabeça de cada especialista, o PM vira gargalo).
4. Insegurança ao apresentar trabalho feito com IA para a liderança (medo de parecer raso, medo de não usar e ficar para trás).
5. Sensação de que o trabalho ficou raso (virou editor de rascunho, sumiu a parte de decidir e julgar).
6. Cursos genéricos de IA que não falam de produto (servem para qualquer um, por isso não servem para o PM).

---

## 4. Voz e tom Human First (regras inegociáveis)

- Direto e prático, frases curtas, zero clichê motivacional.
- Honesto sobre os limites da IA, sem vender mágica.
- Português brasileiro, sem anglicismos quando há bom equivalente.
- **Sem travessão.** Use vírgula, ponto ou parênteses.
- **Sem contraste binário "não é X, é Y"** (exceto a frase-âncora da seção 2).
- **Não começar frase com a palavra "Eu".**
- **Nunca mencionar o empregador atual do criador** (risco contratual).
- **Não usar a palavra "privilégio"** em copy publicada.
- **Sem emojis** em peças da marca.
- Começar pela dor, não pelo produto. Headline carrega a tensão; o resultado vem depois.
- CTA na voz do desejo ("Quero começar agora"), nunca no medo.
- Prova social só com nome real. Sem nome real, omitir a seção.

---

## 5. O que evitar a todo custo

- Cronômetro de "oferta válida por X".
- "Ondas" ou lotes com vagas limitadas (curso digital não tem vaga limitada, e escassez falsa viola o CDC).
- CTAs de medo ("não quero ficar para trás").
- Headlines de comparação social ("enquanto você adia, outros PMs entregam mais").
- Depoimentos de persona genérica ("PM Pleno, turma piloto") sem nome real.
- Promessas vagas ("transforme sua carreira", "domine a IA").
- Bullets de feature sem o significado para o aluno.

---

## 6. Estado atual das landing pages (técnico)

- **Repositório:** alverub89/human-first-academy. Trabalho na branch `main`.
- **Hospedagem:** Netlify. Pasta publicada: `BMad/_bmad-output/planning-artifacts`. A raiz `/` faz redirect 302 para `pm-ai-kickstart-landing-preview.html`.
- **Arquivos das páginas:**
  - `pm-ai-kickstart-landing-preview.html` = Variante A (principal, ancorada na dor).
  - `variant-b-resultado.html` = Variante B (hero ancorado em resultado).
  - `variant-c-autoridade.html` = Variante C (hero na voz pessoal do criador).
- **Formato técnico:** cada página é um HTML único com CSS e JS inline (sem build). Editar o HTML direto.
- **Design system:** fontes Fraunces (títulos) e Manrope (texto); paleta terracota e creme, com verde de confiança para sinais positivos; componentes reutilizáveis (`.section`, `.btn`, `.offer`, `.flow`, `.artifacts` com modal, `.faq`, cards).
- **Estrutura de seções da principal (em ordem):** Hero (dor) → card do instrutor → A virada → Método 3D (bloco visual) → 4 artefatos (cards que abrem modal-documento) → Para quem é / não é → O que está dentro (5 momentos) → Como cada aula funciona → Vídeos → Sobre quem conduz → FAQ honesto → Fechamento.
- **Interações:** modais dos 4 artefatos (conteúdo num array `artifacts` no script), carrossel de vídeos do YouTube (array `videos` no script), captura de email via Netlify Forms.
- **Assets:** em `./assets` (imagem de hero, retrato do instrutor).

---

## 7. Fontes de verdade e glossário

- **Instrutor:** Rubão Alves. LinkedIn: linkedin.com/in/rubao-alves. YouTube: youtube.com/@Rubão_Alves. Criador da Cida (plataforma de carreira com IA).
- **Bio:** quase 20 anos em tecnologia e produto, liderando plataformas digitais e iniciativas orientadas a dados para milhões de pessoas. Não citar o empregador atual.
- **Curador de decisão:** o PM que conduz a IA e decide com critério, em vez de apenas editar rascunho.
- **Artefato:** documento reutilizável que tira o contexto ou o critério da cabeça das pessoas e torna auditável.

---

## 8. Fora de escopo e pendências

- **Link da Hotmart:** os botões de compra estão com `href="#"`. Substituir pelo checkout real quando disponível: [colar link da Hotmart].
- **Grade v4 detalhada:** a ementa hoje aparece em 5 momentos. Detalhar as 15 aulas dentro da estrutura 3D quando a grade v4 estiver pronta: [colar grade v4].
- **Netlify Forms:** ativar Form detection e um novo deploy para a lista de email gravar; configurar notificação.
- **Teste A/B:** decidir entre mandar tráfego para os 3 URLs ou configurar split testing no Netlify.

---

## 9. Contrato de Execução curto (como pedir trabalho de IA neste projeto)

- **Papel:** copywriter sênior de produto educacional, voz Human First.
- **Antes de escrever:** dizer qual dor (1 a 6) a peça ataca e qual o objetivo psicológico.
- **Limites:** não inventar dado, nome ou depoimento; sinalizar o que faltar; respeitar as seções 4 e 5.
- **Formato de saída:** texto pronto, sem placeholder, e a marcação da dor atacada.
- **Parada:** só entregar depois de validar a checklist de aceite (sem travessão, sem "Eu" no início, sem escassez falsa, sem empregador, CTAs no desejo, artefatos pelo nome).
