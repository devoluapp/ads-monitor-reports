# Dossiê ConcursoRadar — Técnico Judiciário — TRF (11/10/2026)

## Métricas da Rodada
- **Buscas na Meta Ad Library:** `concurso TRF`, `tribunal regional federal`, `técnico judiciário`, `técnico judiciário área administrativa`, `TRF1`, `TRF2`, `TRF3`, `TRF4`, `TRF5`, `TRF6`, `concurso tribunal`
- **Filtro:** anúncios ativos no Brasil, no ar há 7+ dias (coleta ampla para achar padrões; a longevidade é analisada nas tabelas)
- **Ofertas do nicho:** 130 (de 315 anúncios; agrupadas por anunciante + página de destino)
- **Descartadas por não citarem concurso:** 94 (listadas no fim para auditoria)
- **Ofertas de foco direto:** 47 | adjacentes: 83
- **Sinal de tração:** 8 forte, 3 fraco, 119 médio
- **Landing pages lidas:** 89 de 130
- **Ticket confirmado no checkout:** 22 de 24 ofertas com checkout detectado (92%)
- **Tempo de processamento:** 1003 segundos

## O que esta evidência prova e o que não prova
- **Prova:** que o anunciante mantém o anúncio pago no ar há N dias, o texto exato da copy, a página de destino e, quando `fonte_ticket` é `checkout`, o preço cobrado.
- **Não prova:** faturamento, número de vendas ou lucro. A Meta não publica gasto nem impressões de anúncios comerciais no Brasil.
- **Sinais indiretos de escala:** `anuncios_ativos_estimados` (quantos anúncios a oferta mantém no ar) e `anuncios_com_baixo_volume_de_impressoes` (selo da própria Meta: anúncio no ar, mas com pouca verba). Longevidade com baixo volume não é validação.
- **`sinal_tracao`:** fraco = todos os anúncios com baixo volume; forte = 90+ dias, 3+ anúncios ativos e nenhum com baixo volume; médio = o resto.
- **Preços:** só `fonte_ticket: checkout` é preço lido na página de pagamento. `precos_exibidos_na_lp` lista valores soltos da página (preço cheio, parcela, bônus) sem interpretação.
- **Amostra:** até o limite de anúncios por busca, na ordem de relevância da Meta. Não é um censo do mercado.

> ⚠️ **AVISO PARA A IA ANALISADORA (SALVAGUARDA EPISTÊMICA):**
> Os campos `heuristica_*`, `sinal_tracao`, `foco_direto` e a lista de entregáveis são classificações automáticas por regras de código (palavras-chave e links).
> **NÃO os considere como classificação definitiva ou curada.**
> Baseie a análise no texto da copy e da LP, cite o `id_oferta` de cada afirmação e separe o que está nos dados do que é inferência sua.

---

# Parte 0 — Padrões dos anúncios do nicho

Base: **315 anúncios de 93 anunciantes**; 136 estão no ar há 45+ dias (veteranos); mediana de 23 dias.

Como ler: **Anunciantes** = quantos produtores distintos usam (popularidade). **Veteranos** = quantos desses anúncios estão no ar há 45+ dias, e **% dos veteranos** = a fatia da categoria entre todos os veteranos. Se a fatia entre veteranos é maior que a fatia geral (% anúncios), a categoria aparece mais entre os que duram. Categoria com 1 ou 2 anunciantes é só um caso isolado.

A coleta junta duas amostras por busca (anúncios com 7+ dias e anúncios com 45+ dias), então a proporção de veteranos no total não é uma taxa de sobrevivência.

## Formato do criativo

Vídeo, imagem única ou carrossel.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| vídeo | 46 | 49% | 115 | 37% | 33 | 56 | 41% |
| imagem | 38 | 41% | 154 | 49% | 16 | 62 | 46% |
| carrossel | 30 | 32% | 46 | 15% | 31 | 18 | 13% |

## Proporção do criativo

Vertical (4:5 ou 9:16), quadrada (1:1) ou horizontal.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| vídeo vertical | 44 | 47% | 113 | 36% | 33 | 55 | 40% |
| imagem vertical | 34 | 37% | 116 | 37% | 14 | 39 | 29% |
| carrossel vertical | 24 | 26% | 34 | 11% | 32 | 14 | 10% |
| carrossel quadrada | 8 | 9% | 12 | 4% | 24 | 4 | 3% |
| imagem quadrada | 7 | 8% | 38 | 12% | 54 | 23 | 17% |
| vídeo quadrada | 2 | 2% | 2 | 1% | 44 | 1 | 1% |

## Duração dos vídeos

Só anúncios em vídeo.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| 1 a 2min | 20 | 43% | 29 | 25% | 46 | 16 | 29% |
| 31s a 1min | 19 | 41% | 57 | 50% | 33 | 26 | 46% |
| Até 30s | 12 | 26% | 24 | 21% | 9 | 10 | 18% |
| Mais de 2min | 5 | 11% | 5 | 4% | 79 | 4 | 7% |

## Botão (CTA)

Rótulo do botão exibido no anúncio.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| sem botão | 42 | 45% | 113 | 36% | 13 | 42 | 31% |
| Saiba mais | 37 | 40% | 105 | 33% | 41 | 52 | 38% |
| Ver detalhes | 16 | 17% | 55 | 17% | 46 | 28 | 21% |
| Visitar perfil do Instagram | 15 | 16% | 20 | 6% | 28 | 8 | 6% |
| Comprar agora | 5 | 5% | 9 | 3% | 15 | 2 | 1% |
| Enviar mensagem pelo WhatsApp | 3 | 3% | 4 | 1% | 11 | 0 | 0% |
| Solicitar agora | 2 | 2% | 3 | 1% | 8 | 1 | 1% |
| Cadastre-se | 2 | 2% | 3 | 1% | 88 | 2 | 1% |
| Enviar mensagem | 1 | 1% | 1 | 0% | 16 | 0 | 0% |
| Fale conosco | 1 | 1% | 1 | 0% | 11 | 0 | 0% |
| Inscreva-se | 1 | 1% | 1 | 0% | 90 | 1 | 1% |

## Destino do clique

Para onde o anúncio leva.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Página própria (LP / site) | 60 | 65% | 225 | 71% | 30 | 103 | 76% |
| Página / formulário no Facebook | 37 | 40% | 80 | 25% | 19 | 28 | 21% |
| Checkout direto | 3 | 3% | 6 | 2% | 15 | 1 | 1% |
| WhatsApp | 2 | 2% | 4 | 1% | 117 | 4 | 3% |

## Tamanho da copy

Texto principal do anúncio.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Média (200 a 600) | 55 | 59% | 156 | 50% | 48 | 92 | 68% |
| Longa (mais de 600) | 41 | 44% | 107 | 34% | 13 | 39 | 29% |
| Curta (até 200 caracteres) | 15 | 16% | 51 | 16% | 14 | 4 | 3% |
| Sem texto | 1 | 1% | 1 | 0% | 46 | 1 | 1% |

## Tipo de gancho (1ª linha da copy)

Classificação por palavras-chave; um gancho pode cair em mais de um tipo.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos | Exemplo |
|---|---|---|---|---|---|---|---|---|
| Outro | 38 | 41% | 100 | 32% | 46 | 53 | 39% | 🔥 A sua aprovação em Concursos Públicos não depende dos Materiais! Depende de direcionamento correto. — Gustavo Dias |
| Notícia de concurso / edital | 34 | 37% | 93 | 30% | 9 | 28 | 21% | Saiu o edital do TRT 8 — comece sua preparação agora — Thállius Moraes com Esquadrão de Elite |
| Pergunta | 24 | 26% | 47 | 15% | 59 | 29 | 21% | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? — Isaque Concursos |
| Chamada direta ao público | 14 | 15% | 22 | 7% | 46 | 11 | 8% | E se você pudesse montar a sua própria formação em Direito Previdenciário? — Esmafe RS |
| Número / lista | 12 | 13% | 24 | 8% | 14 | 4 | 3% | 9 magistrados em exercício. 4 deles já aprovados no ENAM. — Esmafe RS |
| Oferta / desconto / urgência | 12 | 13% | 21 | 7% | 51 | 16 | 12% | "📚🆓 Curso Grátis TJ-SP 2026 - Escrevente Técnico Judiciário! 🆓📚 — Nova Concursos |
| Salário / estabilidade | 11 | 12% | 25 | 8% | 14 | 8 | 6% | O TJ-SP Escrevente é uma grande oportunidade para quem busca estabilidade e carreira pública com nível médio. — Central de Concursos |
| Dor / erro do candidato | 11 | 12% | 18 | 6% | 14 | 7 | 5% | Muitos candidatos chegam ao ENAM com domínio teórico em Direito Penal — e erram nas questões mesmo assim. — Esmafe RS |
| Prova social / autoridade | 10 | 11% | 23 | 7% | 59 | 13 | 10% | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? — Isaque Concursos |
| Promessa de método | 5 | 5% | 15 | 5% | 61 | 14 | 10% | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? — Isaque Concursos |
| Contraintuitivo / inimigo comum | 4 | 4% | 6 | 2% | 15 | 1 | 1% | Você pode ter um bom cursinho e ainda perder tempo decidindo o que entra em cada dia. Na mentoria, você recebe planejamento completo, orientação por tarefa e um — LH no pódio |

## Elementos da copy

Recursos presentes no texto; não são excludentes.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Usa emojis | 57 | 61% | 162 | 51% | 48 | 86 | 63% |
| Cita valor em R$ | 29 | 31% | 77 | 24% | 11 | 19 | 14% |
| Lista com marcadores (✔, ✅, •) | 28 | 30% | 69 | 22% | 31 | 32 | 24% |
| Hashtags | 18 | 19% | 36 | 11% | 19 | 9 | 7% |
| Gancho em CAIXA ALTA | 10 | 11% | 23 | 7% | 10 | 5 | 4% |
| Link ou 'link na bio' no texto | 9 | 10% | 12 | 4% | 45 | 6 | 4% |
| Cita bônus | 4 | 4% | 10 | 3% | 43 | 5 | 4% |
| Cita garantia | 3 | 3% | 3 | 1% | 31 | 1 | 1% |

## Sinais de público (ICP) citados na copy

Quem o anúncio diz atender, por palavras-chave. Indica a quem o mercado fala, não quem compra.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos | Exemplo |
|---|---|---|---|---|---|---|---|---|
| Motivado por salário / estabilidade | 33 | 35% | 96 | 30% | 13 | 38 | 28% | 💰 Concursos com salários de até R$20.000 estão ao seu alcance — mas você precisa do caminho certo. — Gustavo Dias |
| Esquece o que estuda / revisão | 19 | 20% | 44 | 14% | 16 | 18 | 13% | Você não precisa apenas ler mais a lei seca. Precisa saber o que memorizar, como revisar e onde concentrar seus esforços. — Decorando a Lei Seca Cursos Para Concursos E OAB |
| Pré-edital / sair na frente | 15 | 16% | 37 | 12% | 33 | 18 | 13% | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. — Tjteiros |
| Trabalha / tem pouco tempo | 13 | 14% | 55 | 17% | 14 | 26 | 19% | Durante essa jornada de estudos, eu estudava de 2h a 3h por dia, já que estudava e trabalhava como CLT. — Isaque Concursos |
| Reta final / pós-edital | 13 | 14% | 27 | 9% | 9 | 10 | 7% | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. — Tjteiros |
| Dificuldade em discursiva / redação | 11 | 12% | 21 | 7% | 18 | 10 | 7% | O edital do TRT 8 (PA/AP) foi publicado. Prepare-se para Analista e Técnico com um curso completo: videoaulas, questões, cronogramas, Lei Seca, redação e muito  — Thállius Moraes com Esquadrão de Elite |
| Nível superior / Direito | 10 | 11% | 23 | 7% | 9 | 7 | 5% | Trata-se de uma oportunidade de nível superior com MUITAS vagas, e uma remuneração inicial muito atrativa. — Concursos Ceisc |
| Perdido no excesso de conteúdo | 10 | 11% | 19 | 6% | 9 | 6 | 4% | Se você tá perdido sem saber como começar ou já estuda mas sente que não evolui, está correndo um sério risco de ficar anos sem a sua aprovação. — Gustavo Dias |
| Começando do zero | 9 | 10% | 26 | 8% | 59 | 16 | 12% | • Esteja começando os estudos agora; — Isaque Concursos |
| Estuda há tempo e não passa | 9 | 10% | 13 | 4% | 75 | 9 | 7% | Questões sobre Direitos Humanos reprovam candidatos no ENAM por um motivo simples: a maioria estuda o tema de forma genérica, sem entender o que a FGV realmente — Esmafe RS |
| Nível médio | 7 | 8% | 22 | 7% | 61 | 22 | 16% | Para você ter uma ideia, eu só me formei no ensino médio por meio do ENCCEJA, já que tinha repetido em todas as matérias. — Isaque Concursos |
| Erra questões / pegadinhas da banca | 5 | 5% | 9 | 3% | 16 | 3 | 2% | Não tem pegadinha, esse preparatório é gratuito. — Ceisc Concursos |
| Mãe / família | 2 | 2% | 10 | 3% | 61 | 10 | 7% | Se isso não fosse o bastante, eu tive uma infância/adolescência bem difícil. Sou filho de ex -empregada doméstica e, por isso, não tínhamos condições financeira — Isaque Concursos |

## Tipo de produto × ticket

Tipo identificado por palavras-chave na copy, no título do link e na headline (uma oferta pode ter vários). Ticket só entra quando foi lido no checkout.

| Tipo de produto | Anunciantes | Ofertas | Veteranas | Com ticket lido | Mínimo | Mediana | Máximo | Tickets lidos |
|---|---|---|---|---|---|---|---|---|
| Material em PDF / apostila / caderno | 52 | 55 | 27 | 4 | R$ 397 | R$ 498 | R$ 1.489 | Brabo Editora R$ 397; Caderno do Aprovado - Materiais para Concursos R$ 497; Decorando a Lei Seca Cursos para Concursos LTDA R$ 500; Discursiva na Prática R$ 1.489 |
| Curso em videoaulas | 29 | 52 | 33 | 8 | R$ 247 | R$ 683 | R$ 6.346 | Thállius Moraes com Esquadrão de Elite R$ 247; Brabo Editora R$ 397; Professor Raphael Reis R$ 450; Decorando a Lei Seca Cursos Para Concursos E OAB R$ 540; Instituto INAPI R$ 827; Decorando a Lei Seca Cursos Para Concursos E OAB R$ 928; Discursiva na Prática R$ 1.489; Ceisc Concursos R$ 6.346 |
| Questões / simulados | 25 | 33 | 17 | 7 | R$ 58 | R$ 500 | R$ 827 | Aprovando Concurseiro R$ 58; Thállius Moraes com Esquadrão de Elite R$ 247; Brabo Editora R$ 397; Decorando a Lei Seca Cursos para Concursos LTDA R$ 500; Decorando a Lei Seca Cursos Para Concursos E OAB R$ 540; Decorando a Lei Seca Cursos para Concursos LTDA R$ 540; Instituto INAPI R$ 827 |
| Isca gratuita / grupo VIP | 19 | 24 | 15 | 5 | R$ 298 | R$ 827 | R$ 6.346 | Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24 R$ 298; Isaque Concursos R$ 497; Instituto INAPI R$ 827; Jus Expert R$ 997; Ceisc Concursos R$ 6.346 |
| Cronograma / plano de estudos | 19 | 22 | 10 | 4 | R$ 247 | R$ 497 | R$ 500 | Thállius Moraes com Esquadrão de Elite R$ 247; Isaque Concursos R$ 497; Isaque Concursos R$ 497; Decorando a Lei Seca Cursos para Concursos LTDA R$ 500 |
| Mentoria / acompanhamento | 19 | 21 | 12 | 2 | R$ 497 | R$ 497 | R$ 497 | Isaque Concursos R$ 497; Isaque Concursos R$ 497 |
| Lei seca / legislação | 11 | 14 | 7 | 8 | R$ 58 | R$ 498 | R$ 928 | Aprovando Concurseiro R$ 58; Thállius Moraes com Esquadrão de Elite R$ 247; Legislação Integrada R$ 377; Caderno do Aprovado - Materiais para Concursos R$ 497; Decorando a Lei Seca Cursos para Concursos LTDA R$ 500; Decorando a Lei Seca Cursos Para Concursos E OAB R$ 540; Decorando a Lei Seca Cursos para Concursos LTDA R$ 540; Decorando a Lei Seca Cursos Para Concursos E OAB R$ 928 |
| Discursiva / redação | 10 | 11 | 4 | 3 | R$ 247 | R$ 450 | R$ 1.489 | Thállius Moraes com Esquadrão de Elite R$ 247; Professor Raphael Reis R$ 450; Discursiva na Prática R$ 1.489 |
| Não identificado | 9 | 9 | 5 | 4 | R$ 197 | R$ 697 | R$ 1.997 | Uniforenses Instituto de Pericias Forenses R$ 197; Decorando a Lei Seca Cursos Para Concursos E OAB R$ 397; Jus Expert R$ 997; flaviaholandagaeta R$ 1.997 |
| Assinatura / clube / vitalício | 6 | 8 | 2 | 7 | R$ 298 | R$ 540 | R$ 1.489 | Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24 R$ 298; Legislação Integrada R$ 377; Decorando a Lei Seca Cursos para Concursos LTDA R$ 500; Decorando a Lei Seca Cursos Para Concursos E OAB R$ 540; Decorando a Lei Seca Cursos para Concursos LTDA R$ 540; Decorando a Lei Seca Cursos Para Concursos E OAB R$ 928; Discursiva na Prática R$ 1.489 |
| Mapas mentais / esquemas | 5 | 5 | 1 | 3 | R$ 497 | R$ 500 | R$ 540 | Caderno do Aprovado - Materiais para Concursos R$ 497; Decorando a Lei Seca Cursos para Concursos LTDA R$ 500; Decorando a Lei Seca Cursos Para Concursos E OAB R$ 540 |
| Flashcards | 1 | 1 | 1 | 0 | — | — | — |  |

## Expressões repetidas entre anunciantes

Sequências de 2 ou 3 palavras (sem acento) usadas na copy por 3 ou mais anunciantes distintos.

`tecnico judiciario` (14), `tribunal regional` (12), `clique em saiba` (12), `r$ 16` (10), `nivel superior` (10), `analista judiciario` (10), `concursos publicos` (9), `tj sp` (8), `regional do trabalho` (8), `link da bio` (8), `8a regiao` (8), `tribunal de justica` (7), `publicacao do edital` (7), `novo concurso` (7), `edital publicado` (7), `agora mesmo` (7), `remuneracao inicial` (6), `r$ 16 040` (6), `quem quer` (6), `pos edital` (6), `garanta sua vaga` (6), `edital sair` (6), `cronograma de estudos` (6), `concurso publico` (6), `trabalho da 8a` (5), `toque em saiba` (5), `sair para comecar` (5), `realmente importa` (5), `quer comecar` (5), `prova objetiva` (5)

## Arquivo de ganchos (anúncios mais replicados e mais antigos)

| Anunciante | Dias | Cópias | Formato | Botão | Gancho (1ª linha) | Título do link |
|---|---|---|---|---|---|---|
| Gustavo Dias | 9 | 10 | imagem | sem botão | 🔥 A sua aprovação em Concursos Públicos não depende dos Materiais! Depende de direcionamento correto. |  |
| Decorando a Lei Seca Cursos Para Concursos E OAB | 16 | 6 | imagem | sem botão | Três ferramentas. Um mesmo objetivo: transformar o seu estudo em aprovação. 🎯 |  |
| Isaque Concursos | 61 | 4 | vídeo | sem botão | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? |  |
| Esmafe RS | 12 | 4 | vídeo | sem botão | E se você pudesse montar a sua própria formação em Direito Previdenciário? |  |
| Thállius Moraes com Esquadrão de Elite | 9 | 4 | imagem | sem botão | Saiu o edital do TRT 8 — comece sua preparação agora |  |
| Central de Concursos | 89 | 3 | vídeo | sem botão | O TJ-SP Escrevente é uma grande oportunidade para quem busca estabilidade e carreira pública com nível médio. |  |
| Nova Concursos | 51 | 3 | imagem | sem botão | "📚🆓 Curso Grátis TJ-SP 2026 - Escrevente Técnico Judiciário! 🆓📚 |  |
| Esmafe RS | 13 (baixo volume) | 3 | vídeo | sem botão | Muitos candidatos chegam ao ENAM com domínio teórico em Direito Penal — e erram nas questões mesmo assim. |  |
| Esmafe RS | 13 | 3 | vídeo | sem botão | Questões sobre Direitos Humanos reprovam candidatos no ENAM por um motivo simples: a maioria estuda o tema de forma genérica, sem entender o que a FGV realmente cobra. |  |
| Monica Freitas MTE | 11 | 3 | imagem | sem botão | ⚖️ O próximo concurso do TRF da 3ª Região pode ser uma grande oportunidade para quem quer conquistar uma vaga no serviço público. |  |
| Monica Freitas MTE | 11 | 3 | imagem | sem botão | ⚖️ O TJ-SP já iniciou os estudos para um próximo concurso, com salários que passam de R$6.000,00. |  |
| Monica Freitas MTE | 11 | 3 | imagem | sem botão | ⚖️ O TRF da 3ª Região já iniciou os estudos para um próximo concurso, com salários que podem começar em torno de R$ 10 mil para técnico e R$ 16 mil para analista. |  |
| Tjteiros | 100 | 2 | vídeo | sem botão | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. |  |
| Brabo Concursos | 95 | 2 | vídeo | sem botão | O TJ-SP tem um novo concurso previsto para 2026, são mais de 3.300 cargos vagos de Escrevente Técnico Judiciário, temos contrato assinado com a banca organizadora e recentemente foram criados novas 720 vagas de Escrevent |  |
| Central de Concursos | 89 | 2 | vídeo | sem botão | O concurso do Tribunal de Justiça de São Paulo (TJ-SP) é uma das maiores oportunidades para quem tem apenas o ensino médio completo. Além de um excelente salário inicial, você conquista estabilidade financeira, benefício |  |
| Estratégia Concursos | 87 | 2 | vídeo | sem botão | 📢 O professor Herbert Almeida indica: vale a pena estudar para CGU e Tribunal de Contas da União! |  |
| Venâncio & Delgado - Advogados | 61 | 2 | vídeo | sem botão | ⚖️ A banca examinadora pode mudar de entendimento e te eliminar como PCD? Saiba o que o Superior Tribunal de Justiça (STJ) decidiu! |  |
| G7 Jurídico | 52 (baixo volume) | 2 | imagem | sem botão | ADI sobre o regime remuneratório da magistratura, novo entendimento sobre taxas estaduais, marco legal do crime organizado, mudanças na legislação eleitoral. Em poucos meses, o STF redesenhou o cenário e o Legislativo en |  |
| Lucas Viégas | 47 | 2 | vídeo | sem botão | Concurso TCE GO: Edital Publicado hoje! Provas em janeiro, como será a sua preparação até o dia da prova? |  |
| Esmafe RS | 13 | 2 | carrossel | Saiba mais | 9 magistrados em exercício. 4 deles já aprovados no ENAM. | Conheça quem vai te preparar para o ENAM. |
| Esmafe RS | 13 | 2 | vídeo | sem botão | Pessoa física doa livros para uma biblioteca. Há imposto? |  |
| GG Concursos | 10 | 2 | imagem | Comprar agora | Vai deixar essa oportunidade passar? | Assine o GG Play 360 |
| Giovanna Carranza Desenvolvimento Profissional | 9 | 2 | imagem | sem botão | Concurso TRT8! |  |
| Isaque Concursos | 9 | 2 | vídeo | sem botão | ATENÇÃO! EDITAL PUBLICADO: TRT-8 (PA/AP) |  |
| Sou Concurseiro | 9 | 2 | vídeo | sem botão | Acabou a faculdade ou vai se formar este ano? O concurso do TJ-AM pode ser o seu próximo passo. |  |
| Sou Concurseiro | 9 | 2 | vídeo | sem botão | Qualquer curso superior, salário acima de R$ 15 mil e jornada das 8h às 14h: esse é o concurso do TJ-AM. |  |
| Sou Concurseiro | 9 | 2 | vídeo | sem botão | Acha que já passou da idade para estudar? No TJ-AM tem gente de 30, 40 e 50 anos se preparando agora. |  |
| Sou Concurseiro | 9 | 2 | vídeo | sem botão | Mais de 30 ou 40 anos e ensino superior? Presta atenção no concurso do TJ-AM: 400 vagas e jornada das 8h às 14h. |  |
| Sou Concurseiro | 9 | 2 | vídeo | sem botão | Mais de 40 anos, ensino superior e vontade de mudar de carreira? Conheça o concurso do TJ-AM: 400 vagas. |  |
| Sou Concurseiro | 9 | 2 | vídeo | sem botão | Cada vez mais gente com 40, 50 anos está estudando para o TJ-AM: salário acima de R$ 15 mil e jornada das 8h às 14h. |  |
| Sou Concurseiro | 9 | 2 | vídeo | sem botão | Tem mais de 30, 40 ou 50 anos e já tem ensino superior? O Tribunal de Justiça do Amazonas pode ser a sua transição de carreira. |  |
| Delta Fabio Silva | 8 | 2 | vídeo | sem botão | E aí vamos cair de cabeça nesses CONCURSOS POLICIAIS DO AMAZONAS? |  |
| Flávio Britto Advocacia | 8 | 2 | vídeo | sem botão | Quer saber quais questões são passíveis de anulação pela via judicial no concurso da PPRN? |  |
| Decorando a Lei Seca Cursos Para Concursos E OAB | 924 | 1 | vídeo | sem botão | Lançados em março de 2024 |  |
| Caderno do Aprovado - Materiais para Concursos | 619 | 1 | vídeo | sem botão | Lançados em janeiro de 2025 |  |
| Concursos Ceisc | 255 | 1 | imagem | Saiba mais | Lançados em janeiro de 2026 |  |
| Concursos Ceisc | 234 | 1 | imagem | Saiba mais | Lançados em fevereiro de 2026 |  |
| Concursos Ceisc | 214 | 1 | imagem | Saiba mais | Está precisando de mais direcionamento para o concurso do Ministério Público de Minas Gerais? |  |
| Concursos Ceisc | 194 | 1 | vídeo | Saiba mais | A sua preparação para o TJ-SP exige foco e direcionamento. |  |
| Concursos Ceisc | 194 | 1 | vídeo | Saiba mais | O edital do concurso do TJ-BA com o cargo de Analista Judiciário pode sair a qualquer momento, e o momento de estudar é agora. 🚀 |  |

---

# Parte 1 — Ofertas de foco direto (47)

---
id_oferta: 001
anunciante: "Isaque Concursos"
url_destino: "https://projetotrt.com.br/imersao1v1/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1556242356236977"
dias_ativo: 65
anuncios_coletados: 9
anuncios_ativos_estimados: 29
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "onprofit"
ticket_principal: "R$ 497,00"
fonte_ticket: "checkout"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (9)"
botoes: "sem botão (8), Saiba mais (1)"
parcelas: "12x R$ 42,99"
precos_exibidos_na_lp: "R$ 9.776,71 | R$ 90,00 | R$ 11.928 | R$ 0 | R$ 997 | R$ 100 | R$ 497 | R$ 397"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"TRT | Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário?
Depois de ser aprovado 2x no TRT-PI, 1x no TRT-PR e 1x no TRT-RS, gravei uma Imersão para contar exatamente o que eu fiz para ser aprovado nesses TRTs.
Durante essa jornada de estudos, eu estudava de 2h a 3h por dia, já que estudava e trabalhava como CLT.
Não foi uma jornada nada fácil…
Principalmente porque eu não tive uma boa base escolar.
Para você ter uma ideia, eu só me formei no ensino médio por meio do ENCCEJA, já que tinha repetido em todas as matérias.
Se isso não fosse o bastante, eu tive uma infância/adolescência bem difícil. Sou filho de ex -empregada doméstica e, por isso, não tínhamos condições financeiras para pagar cursinhos pra mim.
E mesmo sem pagar cursinhos caros, desenvolvi um método de estudos extremamente eficiente que me fez passar em 4 provas de TRTs. Hoje, sou Técnico Judiciário de um TRT.
Estou ensinando esse mesmo método para diversos alunos e, com toda certeza, qualquer concurseiro pode começar aplicar hoje mesmo e alcançar os mesmos resultados que eu e meus alunos tivemos.
Se você quer chegar competitivo para ser aprovado e nomeado nas próximas provas de TRTs, a Imersão Aprova TRT pode ser um divisor de águas para conquistar a tão sonhada estabilidade financeira como servidor público.
Mesmo que você:
• Tenha pouco tempo para estudar;
• Esteja começando os estudos agora;
• Tenha mais de 40 anos;
• Ou seja um concurseiro experiente
E o melhor: ela é 100% gratuita e on-line. Você pode assistir agora mesmo, onde você estiver.
⚠️ Mas, atenção: essa Imersão pode sair do ar a qualquer momento, de verdade.
Não estou falando isso da boca para fora…
Se a Imersão não estiver fazendo sentido para as pessoas que estão assistindo, eu e minha equipe removeremos do ar. É por esse motivo que ela pode sair do ar a qualquer momento.
De verdade? É uma oportunidade em tanto, pois temos MILHARES de alunos que passaram por essa Imersão e, se eu fosse você, eu reservaria um tempo também para assisti-la.
Para isso, aperte em “saiba mais” para assistir à Imersão agora mesmo.
Te espero lá na outra página!
Bons estudos!"

### Títulos do link nos anúncios
- Imersão Aprova TRT

### Landing Page: Headline & Promessa Central
"Como estudar em alto nível para o cargo de Técnico Judiciário de qualquer TRT do Brasil e alcançar a aprovação, mesmo começando do zero e sem cursinho? — Assista agora à Imersão Aprova TRT e veja como um método simples e comprovado pode te levar à aprovação — usado por quem já foi aprovado em 4 TRTs."

### Seções da Landing Page (títulos, na ordem)
- Tenha tudo que precisa para estudar em alto nível com organização e direcionamento para o cargo de Técnico Judiciário do TRT e alcance sua aprovação
- Você terá acesso ao pós-edital de todos os TRTs do Brasil
- Pós-edital do TRT-8 (PA/AP)
- Técnico Judiciário – Área Administrativa
- Pré-Edital do TRT
- Este é o momento ideal para começar. Quem espera o edital sair já começa atrasado.
- Uma das melhores áreas de concursos do Brasil
- A onda dos TRTs está chegando
- O melhor custo-benefício entre os concursos
- Quanto mais cedo você começar, maior sua chance de ser aprovado
- TRTs Previstos para 2026, 2027 e 2028
- 3 coisas que você precisa saber
- O cargo que trabalhamos
- Você precisa ter ensino superior
- Prepare-se certo e esteja pronto para qualquer TRT
- Conheça os 3 pilares do Projeto TRT
- Cronograma de Estudos Guiado e Inteligente
- Materiais de Estudo e Links Estratégicos
- Contato Direto com o Mentor
- Estude mesmo com pouco tempo
- Acesso imediato com direção desde o primeiro dia
- Acompanhamento real com quem já passou
- Suporte rápido no WhatsApp
- Veja como o método transforma os estudos antes mesmo da aprovação
- Tudo que você terá acesso ao entrar no Projeto TRT
- Cronograma de Estudos Flexível
- Materiais de Estudos em PDF
- Videoaulas Selecionadas do YouTube
- Grupo Exclusivo no WhatsApp com Isaque
- Mentorias Quinzenais em Grupo com Isaque

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Discursiva / redação
- Mentoria
- PDF
- Resumos
- Simulados
- Videoaulas


========================================

---
id_oferta: 002
anunciante: "Leandro Reinhardt l Estudos & Concursos"
url_destino: "https://leandroreinhardt.com.br/trt-desafio-nucleo-duro-tjaa/?utm_source=meta-ads&utm_medium=%7B%7Badset.name%7D%7D%7C%7B%7Badset.id%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D%7C%7B%7Bcampaign.id%7D%7D&utm_content=%7B%7Bad.name%7D%7D%7C%7B%7Bad.id%7D%7D&utm_term=%7B%7Bplacement%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=3626400700862360"
dias_ativo: 14
anuncios_coletados: 20
anuncios_ativos_estimados: 20
anuncios_com_baixo_volume_de_impressoes: 1
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tjaa"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados"
formatos_dos_anuncios: "imagem (20)"
botoes: "Saiba mais (20)"
precos_exibidos_na_lp: "R$ 297 | R$ 97 | 12x de R$ 9,70"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"<100
33 tópicos, 71% das questões específicas
70 dias, 1 hora por dia, dentro do que a FCC cobra de verdade."

### Ganchos das variações (1ª linha de cada anúncio)
- 33 tópicos, 71% das questões específicas
- R$ 12.200 de remuneração inicial
- Você não precisa do edital inteiro
- 1 hora por dia, depois do trabalho
- <100
- Os próximos TRTs já estão confirmados

### Landing Page: Headline & Promessa Central
"71% das questões específicas estão em 33 tópicos . E é isso o que vai decidir sua aprovação. — Mapeamos as questões do Núcleo Duro que a FCC cobrou nos TRTs dos últimos 5 anos. Em 70 dias, você se desafia a dominar esses tópicos."

### Seções da Landing Page (títulos, na ordem)
- Você já sabe estudar. O problema é que nunca teve o mapa certo.
- O Núcleo Duro te mostra o que a banca cobra de verdade, e onde vale a pena se aprofundar.
- 3.021 questões analisadas
- 33 tópicos favoritos da FCC
- Padrões que se repetem
- Profundidade na medida certa
- Disciplinas do Núcleo Duro
- O que não está no Desafio
- Os dados que provam o que você vai estudar.
- Administração Geral e Pública
- Engenharia reversa da banca
- Levantamento estatístico de questões
- Análise dos padrões de cobrança da FCC
- Seleção dos tópicos de maior impacto
- Comentários aprofundados para estudo
- Mapa de Engenharia Reversa da FCC
- Veja como funciona na prática.
- 1 hora por dia. Pensado para acelerar sua preparação e te fazer dominar os tópicos de maior peso da prova.
- O Desafio potencializa o seu estudo, não substitui.
- Você já faz isso
- O Desafio acrescenta isso, todo dia
- 70 dias com começo, meio e fim. Não um desafio interminável.
- Uma dose diária do núcleo duro
- Simulado final
- Para quem é o Desafio Núcleo Duro TRT?
- É para você se:
- Não é para você se:
- Quem já está dentro do Desafio
- Quem criou o Desafio
- Liane Reinhardt

### Seção "Para Quem NÃO É" (declarado na LP)
- ×acredita que passar em TRT é só assistir videoaulas do cursinho×quer mais um material para colecionar sem executar×não está disposto à rotina diária de 70 dias

### Entregáveis / Formato (termos encontrados na LP)
- Mentoria
- Simulados
- Videoaulas


========================================

---
id_oferta: 003
anunciante: "Nova Concursos"
url_destino: "https://aprovacao.novaconcursos.com.br/curso-gratis-tj-sp-ads"
ad_library_url: "https://www.facebook.com/ads/library/?id=1014609301122831"
dias_ativo: 117
anuncios_coletados: 7
anuncios_ativos_estimados: 14
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Questões / simulados, Cronograma / plano de estudos, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (7)"
botoes: "Saiba mais (6), sem botão (1)"
precos_exibidos_na_lp: "R$ 297,00 | R$ 0,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Captura de Lead (Isca Digital / Lista de Espera)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
""📚🆓 Curso Grátis TJ-SP 2026 - Escrevente Técnico Judiciário! 🆓📚
Prepare-se para o TJ-SP 2026 com nosso curso grátis! 🌟
✅ 24 Aulas abrangentes para dominar o conteúdo do TJ-SP 2026.
📅 Plano de Estudos projetado para apenas 1 hora por dia - encaixe nos seus horários.
👨‍🏫 Tutoria Especializada com Professores experientes para esclarecer todas as suas dúvidas.
📝 Questões atualizadas para você praticar e se preparar da melhor maneira.
Inscreva-se agora mesmo e comece sua jornada rumo ao sucesso no TJ-SP 2026! 🚀
Garanta sua Vaga!"

### Landing Page: Headline & Promessa Central
"Preencha os dados para garantir seu acesso ao Curso Gratuito TJ-SP 2026 - Escrevente — Isso vai mudar seu nível de preparação para concursos e você finalmente vai mudar seu status de concurseiro para concursado!"

### Seções da Landing Page (títulos, na ordem)
- Isso vai mudar seu nível de preparação para concursos e você finalmente vai mudar seu status de concurseiro para concursado!
- Trabalha e estuda;
- Tem 1h por dia para se dedicar aos estudos;
- Precisa de ajuda na organização do que estudar até a prova;
- Se sente perdido em meio a tantos materiais e conteúdos.
- Thiago Henrique – Aprovado TJ-SP
- Jéssica de Oliveira – Aprovado TJ-SP
- 45 dias de Acesso
- Aulas completas para - TJ-SP - Escrevente
- Plano de Estudos com 1h por dia
- Tutoria Especializada com Professores
- Questões Atualizadas
- de: R$ 297,00
- R$ 0,00 (ZERO)

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 004
anunciante: "Esmafe RS"
url_destino: "https://www.facebook.com/esmafers/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1626896835656894"
dias_ativo: 13
anuncios_coletados: 5
anuncios_ativos_estimados: 13
anuncios_com_baixo_volume_de_impressoes: 1
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf4"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno, Questões / simulados"
formatos_dos_anuncios: "carrossel (1), vídeo (4)"
botoes: "Enviar mensagem pelo WhatsApp (1), sem botão (4)"
primeira_coleta_propria: "2026-10-09"
dias_distintos_coletado: 3
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Carreiras Policiais"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Muitos candidatos chegam ao ENAM com domínio teórico em Direito Penal — e erram nas questões mesmo assim.
O motivo: a FGV trabalha com casos concretos e exige que o candidato faça a adequação típica da conduta com precisão. Não basta saber a teoria. É preciso treinar o raciocínio no perfil exato da banca.
A Juíza Federal Yasmin Duarte — 1º lugar no XVIII Concurso do TRF4 e professora de Direito Penal no Curso Intensivo ENAM 2026 da ESMAFE/RS — entrega no vídeo duas orientações diretas: como resolver questões no perfil da FGV e quais legislações especiais do edital têm o melhor custo-benefício para a prova.
📚 128h com professores que são magistrados em exercício
✅ 4 de 9 docentes já aprovados no próprio ENAM
📅 Aulas a partir de 11 de agosto — 1º lote: 75 vagas
🔗 Clique no link para garantir sua vaga.
#ENAM2026 #DireitoPenal #MagistraturaFederal #ESMAFE #ConcursosJurídicos #JuizFederal"

### Ganchos das variações (1ª linha de cada anúncio)
- 9 magistrados em exercício. 4 deles já aprovados no ENAM.
- Muitos candidatos chegam ao ENAM com domínio teórico em Direito Penal — e erram nas questões mesmo assim.
- E se você pudesse montar a sua própria formação em Direito Previdenciário?
- Questões sobre Direitos Humanos reprovam candidatos no ENAM por um motivo simples: a maioria estuda o tema de forma genérica, sem entender o que a FGV realmente cobra.
- Pessoa física doa livros para uma biblioteca. Há imposto?

### Títulos do link nos anúncios
- Conheça quem vai te preparar para o ENAM.

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 005
anunciante: "Portal & OAB"
url_destino: "https://olympus.cursosdoportal.com.br/o-adm-trt-pa/?utm_source=%7B%7Bsite_source_name%7D%7D&utm_medium=%7B%7Badset.name%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D&utm_term=%7B%7Bplacement%7D%7D&utm_content=%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1648368803684858"
dias_ativo: 9
anuncios_coletados: 10
anuncios_ativos_estimados: 10
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados, Cronograma / plano de estudos, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (3), imagem (7)"
botoes: "Ver detalhes (3), sem botão (7)"
precos_exibidos_na_lp: "R$ 9.776,71 | R$ 16.040,88"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O Tribunal Regional do Trabalho da 8ª Região (TRT 8), que abrange Pará e Amapá, avançou na preparação de um novo concurso público. A Fundação Carlos Chagas (FCC) já foi contratada como banca organizadora do certame.
A seleção deverá contemplar os cargos de Técnico e Analista Judiciário, em diversas especialidades. O número de vagas ainda não foi definido, mas o tribunal registra 102 cargos vagos, sendo 82 de Técnico Judiciário e 11 de Analista Judiciário. O cronograma está em ajuste entre o TRT 8 e a FCC, com expectativa de publicação do edital.
No grupo de estudos, você terá acesso a materiais gratuitos, orientações de estudo, resolução de questões e atualizações sobre cargos, edital, inscrições, provas e todas as etapas do concurso.
Clique em “Saiba Mais” e entre no grupo de WhatsApp para receber materiais gratuitos e acompanhar todas as novidades do concurso do TRT 8.
See Details"

### Landing Page: Headline & Promessa Central
"Seu próximo capítulo: TRT-8. Comece a escrever a sua aprovação. — Entre no grupo de estudos GRATUITO e avance com foco disciplina e direção."

### Seções da Landing Page (títulos, na ordem)
- Uma carreira. Um novo horizonte.
- Dois caminhos. Um futuro à sua altura.
- Técnico Judiciário
- Analista Judiciário
- Preparação que sai da intenção.
- Materiais de estudo
- Questões e prática
- Revisão com foco
- Informação relevante
- Estudar é individual. Evoluir pode ser coletivo.
- O Portal de quem decidiu ir além.
- Cada trajetória merece ser contada.

### Entregáveis / Formato (termos encontrados na LP)
- Mentoria


========================================

---
id_oferta: 006
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2549-concurso-trf-3-analista-judiciario-area-judiciaria"
ad_library_url: "https://www.facebook.com/ads/library/?id=1355671819846214"
dias_ativo: 101
anuncios_coletados: 9
anuncios_ativos_estimados: 9
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trf, trf 3"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "imagem (9)"
botoes: "Ver detalhes (5), Saiba mais (3), sem botão (1)"
precos_exibidos_na_lp: "R$ 16.040,85 | R$ 9.007,67 | R$ 1.199,00 | R$ 824,25 | 12x de R$ 68,69"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O TRF-3 é uma das grandes oportunidades para quem busca uma carreira na área jurídica!
O edital do concurso para Analista Judiciário será publicado em breve e este é o momento ideal para entender o cenário e começar a construir uma preparação consistente.
Remuneração inicial: R$ 16.040,85
Nível superior: Direito
Atuação: São Paulo e Mato Grosso do Sul
Em concursos de alto nível, a diferença está na preparação prévia!
Saiba mais sobre essa oportunidade e comece sua preparação.
TRF-3 | Analista Judiciário"

### Ganchos das variações (1ª linha de cada anúncio)
- Estudar com direcionamento te poupa tempo e energia.
- Estude com método!
- O TRF-3 é uma das grandes oportunidades para quem busca uma carreira na área jurídica!
- Uma preparação eficiente para ingressar nos tirbunais exige planejamento, prática e acompanhamento ao longo da jornada.
- A diferença para sua aprovação no TRF-3 pode estar em como você vai se preparar.
- Comece sua preparação para o TRF-3 com quem entende de aprovação!

### Títulos do link nos anúncios
- TRF-3 | Analista Judiciário

### Landing Page: Headline & Promessa Central
"TRF-3 | Analista Judiciário - Área Judiciária"

### Seções da Landing Page (títulos, na ordem)
- Sobre o curso
- Nesse curso você terá
- Conheça os professores
- Sobre a prova
- Conteúdo Programático

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Discursiva / redação
- Mentoria
- PDF
- Simulados
- Videoaulas


========================================

---
id_oferta: 007
anunciante: "Monica Freitas MTE"
url_destino: "https://form.respondi.app/yLeg4HU6"
ad_library_url: "https://www.facebook.com/ads/library/?id=2170313573699395"
dias_ativo: 11
anuncios_coletados: 3
anuncios_ativos_estimados: 9
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Curso em videoaulas, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (3)"
botoes: "sem botão (3)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"⚖️ O TRF da 3ª Região já iniciou os estudos para um próximo concurso, com salários que podem começar em torno de R$ 10 mil para técnico e R$ 16 mil para analista.
Mas estudar para concursos de tribunais exige muito mais do que apenas seguir matérias e assistir aulas.
Foi por isso que eu criei o Método MTE.
✅ Cronograma de estudos
✅ Planejamento personalizado
✅ Estratégia de revisões
✅ Direcionamento da preparação
✅ Acompanhamento durante toda a trajetória
✅ Estratégias para evitar travas e autossabotagem
Com mais de 10 anos estudando comportamento humano, eu também te ajudo a manter constância e seguir em frente durante o processo.
👉 Clique em Saiba Mais e conheça o Método MTE."

### Ganchos das variações (1ª linha de cada anúncio)
- ⚖️ O próximo concurso do TRF da 3ª Região pode ser uma grande oportunidade para quem quer conquistar uma vaga no serviço público.
- ⚖️ O TJ-SP já iniciou os estudos para um próximo concurso, com salários que passam de R$6.000,00.
- ⚖️ O TRF da 3ª Região já iniciou os estudos para um próximo concurso, com salários que podem começar em torno de R$ 10 mil para técnico e R$ 16 mil para analista.

### Landing Page: Headline & Promessa Central
"Mentoria MTE | Formulário de Aplicação"

### Entregáveis / Formato (termos encontrados na LP)
- Mentoria


========================================

---
id_oferta: 008
anunciante: "Thállius Moraes com Esquadrão de Elite"
url_destino: "https://lp.oesquadraodeelite.com.br/curso-intensivo-trt-8-reta-final"
ad_library_url: "https://www.facebook.com/ads/library/?id=1842940127056507"
dias_ativo: 9
anuncios_coletados: 3
anuncios_ativos_estimados: 9
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario, tjaa"
plataforma_checkout: "onprofit"
ticket_principal: "R$ 247,00"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Questões / simulados, Lei seca / legislação, Discursiva / redação, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (3)"
botoes: "sem botão (2), Ver detalhes (1)"
parcelas: "12x R$ 24,80"
precos_exibidos_na_lp: "R$ 13 | R$ 597,00 | R$ 247,00 | 12x de R$ 24,80"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Saiu o edital do TRT 8 — comece sua preparação agora
O edital do TRT 8 (PA/AP) foi publicado. Prepare-se para Analista e Técnico com um curso completo: videoaulas, questões, cronogramas, Lei Seca, redação e muito mais. Garanta seu acesso e estude para conquistar uma vaga com remuneração acima de R$ 13 mil."

### Títulos do link nos anúncios
- CLIQUE EM SAIBA MAIS

### Landing Page: Headline & Promessa Central
"Curso Intensivo TRT 8 – Reta Final! – O Esquadrão De Elite — Professores especialistas em Tribunais"

### Seções da Landing Page (títulos, na ordem)
- Professores especialistas em Tribunais
- Curso de Resolução de Questões
- Sistema de questões
- Flashcards
- Cronograma integrado
- IA integrada
- Central de Comando
- Lei Seca organizada
- O que isso significa na prática?
- Método direcionado
- Evolução constante
- Resultados reais
- Técnico Judiciário
- Analista Judiciário
- Técnico Judiciário (TJAA)
- Analista Administrativo (AJAA)
- Analista Judiciário e oficial de justiça (AJAJ)
- Dúvidas frequentes
- Tudo o que você precisa para estudar com estratégia

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Flashcards
- Videoaulas


========================================

---
id_oferta: 009
anunciante: "Portal Concursos"
url_destino: "https://oportalconcursos.com.br/h-adm-trt-mt/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1861645355201548"
dias_ativo: 11
anuncios_coletados: 8
anuncios_ativos_estimados: 8
anuncios_com_baixo_volume_de_impressoes: 1
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (1), imagem (7)"
botoes: "Saiba mais (8)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"<100
🚨 CONCURSO TRT/MT: EDITAL SE APROXIMA!
O concurso do TRT/MT está autorizado, e a publicação do edital fica cada vez mais próxima.
⚖️ Cargos: Técnico Judiciário (Médio) e Analista Judiciário (Superior)
💰 Salários previstos: podem chegar a R$ 9,7 mil e R$ 16 mil
👉 Toque em “Saiba Mais” e entre gratuitamente no grupo de estudos!"

### Ganchos das variações (1ª linha de cada anúncio)
- 🚨 CONCURSO TRT/MT: EDITAL SE APROXIMA!
- <100

### Landing Page: Headline & Promessa Central
"TRT/MT – oportalconcursos.com.br — Concurso do Tribunal Regional do Trabalho do Mato Grosso"

### Seções da Landing Page (títulos, na ordem)
- Concurso do Tribunal Regional do Trabalho do Mato Grosso
- Venha fazer parte do número 01 em aprovação!
- O que você recebe ao acessar o grupo:
- Materiais de estudos gratuitos
- Nóticias Sobre o Concurso
- Aulas gratuitas no Youtube
- O que dizem os aprovados
- Sua preparação em boas mãos...
- Política de Privacidade | Termos de Uso
- © 2026 Portal Concursos. Todos os direitos reservados.
- CNPJ: 46.402.627/0001-70

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 010
anunciante: "Isaque Concursos"
url_destino: "https://projetotrt.com.br/trt8/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1400478538904369"
dias_ativo: 9
anuncios_coletados: 4
anuncios_ativos_estimados: 8
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "onprofit"
ticket_principal: "R$ 497,00"
fonte_ticket: "checkout"
tipos_produto: "Mentoria / acompanhamento, Cronograma / plano de estudos"
formatos_dos_anuncios: "vídeo (4)"
botoes: "sem botão (4)"
parcelas: "12x R$ 42,99"
precos_exibidos_na_lp: "R$ 9.776,71 | R$ 90,00 | R$ 11.928 | R$ 0 | R$ 997 | R$ 100 | R$ 497 | R$ 397"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"ATENÇÃO! EDITAL PUBLICADO: TRT-8 (PA/AP)
Tenha tudo que você precisa para chegar competitivo na prova e ser aprovado no cargo de Técnico Judiciário 🔥
Depois sair do zero, ter apenas 2h por dia para estudar e ser aprovado 2x no TRT-PI, 1x no TRT-PR e 1x no TRT-RS...
Resolvi consolidar o mesmo método que usei em um só lugar.
Mas não apenas isso...
Eu e minha equipe juntamos todos os materiais, bizus estratégicos, cronograma com todas as metas e diversas outras ferramentas em uma plataforma só.
Essa plataforma é o que chamamos de Projeto TRT.
Além de tudo isso que falei, você ainda terá mentorias em grupo comigo, painel estatístico inteligente, cronograma adaptável para a sua realidade e muito mais.
Sem precisar pagar cursinhos caros, é exatamente isso que tá fazendo alunos serem aprovados em diversos TRTs espalhados por todo Brasil.
Essa é a plataforma ideal para você que não quer brincar de estudar para o concurso do TRT-8.
Para você que não quer gastar dinheiro em vão com cursinhos caros...
É para você que busca estudar em alto nível para ser aprovado já nessa prova do TRT-8.
Mesmo que você:
• Tenha 3 horas de estudos por dia;
• Esteja começando os estudos agora;
• Tenha mais de 40 anos;
• Ou seja um concurseiro experiente
Para conhecer o Projeto TRT, com acesso ao pós-edital para o TRT-8, aperte em 'saiba mais'.
Na próxima página, te explico com todos os detalhes. Te espero lá."

### Landing Page: Headline & Promessa Central
"Tenha tudo que você precisa para chegar competitivo na prova e ser aprovado no cargo de Técnico Judiciário do TRT-8 (AP/PA) — Isso mesmo que você tenha apenas 3h de estudos por dia. A mesma metodologia de estudos que eu usei para ser aprovado em 4 TRTs, agora direcionado para o pós-edital do TRT-8 (PA/AP)."

### Seções da Landing Page (títulos, na ordem)
- Cronograma Pós-Edital do TRT-8 : do edital até o dia da prova
- Não dá mais para esperar. O edital do TRT-8 já foi publicado.
- Uma das melhores áreas de concursos do Brasil
- O edital já foi publicado
- O melhor custo-benefício entre os concursos
- Quem começar agora sai na frente da maioria
- Técnico Judiciário – Área Administrativa
- 3 coisas que você precisa saber
- O cargo que trabalhamos
- Você precisa ter ensino superior
- Você estuda com o Cronograma Pós-Edital
- Conheça os 3 pilares do Projeto TRT
- Cronograma de Estudos Guiado e Inteligente
- Materiais de Estudo e Links Estratégicos
- Contato Direto com o Mentor
- Estude mesmo com pouco tempo
- Acesso imediato com direção desde o primeiro dia
- Acompanhamento real com quem já passou
- Suporte rápido no WhatsApp
- Veja como o método transforma os estudos antes mesmo da aprovação
- Tudo que você terá acesso ao entrar no Projeto TRT
- Cronograma de Estudos Flexível
- Materiais de Estudos em PDF
- Videoaulas Selecionadas do YouTube
- Grupo Exclusivo no WhatsApp com Isaque
- Mentorias Quinzenais em Grupo com Isaque
- Legislação Organizada por Disciplina
- Painel de Estatísticas para Erros e Acertos de Questões
- Links prontos no TecConcursos e QConcursos
- Raio-X do Concurso

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Discursiva / redação
- Mentoria
- PDF
- Resumos
- Simulados
- Videoaulas


========================================

---
id_oferta: 011
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://www.facebook.com/simboraconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=9045055822237560"
dias_ativo: 619
anuncios_coletados: 7
anuncios_ativos_estimados: 7
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trf, tribunal regional federal, trf3"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Questões / simulados, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (5), carrossel (2)"
botoes: "sem botão (6), Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Comente TRF3 e receba também! 🎁
O próximo concurso do Tribunal Regional Federal da 3ª Região, que abrange os estados de São Paulo e Mato Grosso do Sul, é um dos mais aguardados na área de tribunais em 2026. Os salários iniciais vão até R$ 14.852,66!
Começar antes do edital é uma das maiores vantagens competitivas em concursos públicos. Enquanto muita gente espera a publicação do edital para iniciar os estudos, quem se baseia no conteúdo cobrado no último concurso consegue construir uma base sólida e chega ao pós-edital focado em revisões e resolução de questões.
Pensando nisso, disponibilizamos gratuitamente a planilha verticalizada com o conteúdo programático do último edital do TRF-3, uma ferramenta prática para organizar seus estudos desde já.
👉 Comente TRF3 e receba também! 🎁
#trf3 #concursotrf3 #concursotrf #trt3regiao"

### Ganchos das variações (1ª linha de cada anúncio)
- 📚 Conheça o Caderno do Aprovado e prepare-se em alto nível para os próximos concursos de tribunais.
- Comente TRF3 e receba também! 🎁
- Lançados em janeiro de 2025
- 👉 Comente PLANILHA para receber gratuitamente a minha planilha de conteúdo verticalizado indicando quais são os assuntos mais relevantes para estudar nesse período pré-edital.
- 👉 Comente PLANILHA para receber a minha planilha indicando, dentro de cada uma dessas disciplinas, quais são os assuntos mais relevantes para estudar nesse período pré-edital.

### Títulos do link nos anúncios
- Beto (José Humberto) - Caderno Do Aprovado - TRT/TST/TJ/MP (@cadernoaprovado) • Instagram photos and videos

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 012
anunciante: "Concursosmeucurso"
url_destino: "https://meucurso.com.br/categorias/concursos-publicos-escrevente--tjsp?utm_source=meta&utm_medium=cpc&utm_campaign=cp-vendas&utm_content=v5-img-tjsp-savedspwadv"
ad_library_url: "https://www.facebook.com/ads/library/?id=941559835572125"
dias_ativo: 115
anuncios_coletados: 7
anuncios_ativos_estimados: 7
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "imagem (5), vídeo (1), carrossel (1)"
botoes: "Ver detalhes (3), Saiba mais (3), sem botão (1)"
precos_exibidos_na_lp: "R$ 1.899,00 | 12x de R$ 94,92 | R$ 1.139,00 | R$ 1.499,00 | 12x de R$ 58,67 | R$ 704,00 | R$ 999,50 | 12x de R$ 29,08"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Se você está esperando o edital ser publicado para começar a estudar, talvez esteja perdendo a melhor oportunidade de conquistar sua aprovação.
O concurso para Escrevente Técnico Judiciário do TJ/SP reúne características que fazem dele uma das melhores opções para quem busca estabilidade no serviço público.
Por que vale a pena começar agora?
• Os editais acontecem com frequência, permitindo que quem inicia a preparação antes do lançamento saia na frente da concorrência.
• O requisito é apenas ensino médio completo, tornando o concurso acessível para milhares de candidatos que desejam ingressar no Poder Judiciário.
• A banca organizadora mantém um padrão consolidado, o que permite uma preparação muito mais direcionada e eficiente.
Além disso, o cargo oferece remuneração de até R$ 9.358, considerando vencimentos, benefícios e gratificações previstos.
Com o preparatório do MeuCurso, você estuda com método, flexibilidade e foco no perfil da prova, aumentando suas chances de chegar competitivo quando o próximo edital for publicado.
Comece sua preparação hoje e esteja pronto quando a oportunidade chegar.
HTTPS://MEUCURSO.COM.BR/
3 motivos para começar hoje sua preparação para Escrevente do TJ/SP.
Remuneração atrativa, exigência de nível médio e concursos recorrentes. Conheça por que este é um dos cargos mais disputados do Judiciário paulista.
Remuneração atrativa, exigência de nível médio e concursos recorrentes. Conheça por que este é um dos cargos mais disputados do Judiciário paulista.
HTTPS://MEUCURSO.COM.BR/
HTTPS://MEUCURSO.COM.BR/
HTTPS://MEUCURSO.COM.BR/
HTTPS://MEUCURSO.COM.BR/"

### Ganchos das variações (1ª linha de cada anúncio)
- Quer começar sua preparação para Escrevente TJ/SP?
- Seu próximo objetivo pode começar hoje.
- Quer se preparar para o concurso de Escrevente Técnico Judiciário do TJ/SP, mas não sabe por onde começar?
- O concurso para Escrevente Técnico Judiciário do TJ/SP exige preparação consistente — e você já pode começar.
- NOVOS CONCURSOS TJSP ESTÃO A CAMINHO. E VOCÊ PODE COMEÇAR AGORA.
- Se você está esperando o edital ser publicado para começar a estudar, talvez esteja perdendo a melhor oportunidade de conquistar sua aprovação.

### Títulos do link nos anúncios
- Prepare-se para o TJ/SP com o MeuCurso
- Concurso TJ/SP: 53% OFF no preparatório
- Sua preparação para o TJ/SP começa aqui
- Escrevente TJ/SP: prepare-se agora
- TJSP: novos concursos estão a caminho

### Landing Page: Headline & Promessa Central
"Escrevente TJSP — Explore os cursos disponíveis e encontre a formação ideal para o seu desenvolvimento profissional."

### Seções da Landing Page (títulos, na ordem)
- Combo Escrevente TJ/SP + Analista MPSP
- Escrevente Técnico Judiciário TJ/SP | Regular Pré-Edital
- Escrevente Técnico Judiciário TJ/SP | Treino de Questões - Pré- Edital
- Escrevente Técnico Judiciário TJ/SP | Treino de Questões + Regular - Pré- Edital
- OAB + Residência Jurídica TJ/SP

### Seção "Para Quem É" (declarado na LP)
- 5cursos disponíveis

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 013
anunciante: "Tjteiros"
url_destino: "https://www.facebook.com/61582438800580/"
ad_library_url: "https://www.facebook.com/ads/library/?id=4654373284799285"
dias_ativo: 100
anuncios_coletados: 2
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trf3"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "vídeo (2)"
botoes: "sem botão (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital.
É nesse tempo que se corrigem falhas, se fortalece a base e se constrói a competitividade real.
Se você quer disputar uma vaga no TRF3 em alto nível, não espere o edital para levar isso a sério. Comece já.💙📚"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 014
anunciante: "MEQ Concursos"
url_destino: "https://www.facebook.com/61586241338760/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1684375369487437"
dias_ativo: 92
anuncios_coletados: 4
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (1), vídeo (2), carrossel (1)"
botoes: "sem botão (3), Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Concurso TRT 4/RS: o edital pode sair a qualquer momento.
Para quem espera o edital sair para começar, pode parecer cedo.
Para quem entende o ciclo dos TRTs, já é hora de estudar com estratégia.
Se o TRT 4 está no seu radar, este é o momento de organizar base, banca e revisão.
Você está de olho em Analista Judiciário ou Técnico Judiciário?
Salve este post para acompanhar a movimentação do edital TRT 4.
E não esqueça de se cadastrar no workshop gratuito: Os 5 Pilares do Estudo para TRT.
#ConcursoTRT4 #TRT4 #TRT2026 #EditalTRT4 #AnalistaJudiciario"

### Ganchos das variações (1ª linha de cada anúncio)
- Concurso TRT 4/RS: o edital pode sair a qualquer momento.
- “TRT não vale a pena…”
- Alguns TRTs estão entrando em uma fase decisiva. 👀
- Tem tribunal com banca em definição, grupo de trabalho formado, concurso prorrogado e validade chegando ao fim. Não é promessa de edital imediato, mas é cenário para acompanhar de perto.

### Títulos do link nos anúncios
- www.instagram.com

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 015
anunciante: "Ceisc Concursos"
url_destino: "https://lp.ceisc.com.br/projeto-nomeacao-tj-sp/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2095494471007965"
dias_ativo: 90
anuncios_coletados: 4
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "sympla"
ticket_principal: "R$ 6.345,94"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (4)"
botoes: "Ver detalhes (2), Solicitar agora (1), Inscreva-se (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Seu objetivo é ser Oficial de Justiça ou Escrevente Técnico Judiciário do maior tribunal da América Latina?
Então comece estudar agora mesmo, porque os editais devem ser publicados pela banca Vunesp em breve.
Mas não basta estudar sem dedicação, esse concurso exigirá disciplina e foco no que realmente poderá ser cobrado na sua prova.
E para estudar com direcionamento desde o início, participe gratuitamente do Projeto Nomeação TJ-SP. Assista aulas quinzenais com professores especialistas em Concursos para Carreiras de Tribunais e materiais exclusivos para iniciar seus estudos.
Inscreva-se para dicas de estudo e conheça nosso método."

### Ganchos das variações (1ª linha de cada anúncio)
- Seu objetivo é ser Oficial de Justiça ou Escrevente Técnico Judiciário do maior tribunal da América Latina?
- Em breve devem ser publicados os editais para Oficial de Justiça e Escrevente Técnico Judiciário do TJ-SP e você já sabe que estudar sem direcionamento é perda de tempo.
- Você pode ser o próximo Escrevente Técnico Judiciário do maior tribunal da América Latina, basta estudar com direcionamento, organização e foco na banca.
- Muitos desejam ser Oficial de Justiça do maior tribunal da América Latina, mas apenas quem estuda com direcionamento, organização e foco na banca consegue essa mudança de vida.

### Títulos do link nos anúncios
- Estude Com Ceisc

### Landing Page: Headline & Promessa Central
"Projeto Nomeação TJ-SP | Escrevente Técnico e Oficial de Justiça — O primeiro passo para conquistar uma vaga no maior tribunal da América Latina está aqui"

### Seções da Landing Page (títulos, na ordem)
- O primeiro passo para conquistar uma vaga no maior tribunal da América Latina está aqui
- Não espere o edital!
- Inscreva-se de graça ⤵️
- Você vai receber:
- E muito mais para acelerar o seu desempenho
- Inscreva-se gratuitamente e estude com especialistas na banca Vunesp
- Garanta seu ingresso nos aulões presenciais na nossa sede em São Paulo!
- AULÃO 04 Escrevente
- Direito Penal (Geral e Especial) com Denis Pigozzi - Procurador da República
- AULÃO 05 Oficial de Justiça
- Direito Civil com Thiago Romero - Pós-Doutor em Direito
- AULÃO 05 Escrevente
- Direito Constitucional com Fabiana Rossi - Delegada de Polícia do Estado de SP
- AULÃO 06 Oficial de Justiça
- Seu ponto de partida para o TJ-SP
- Você sabe por onde começar?
- Estudar para o TJ-SP sem direcionamento pode transformar sua preparação em horas de conteúdo sem saber se você está no caminho certo.
- Não sabe quais disciplinas priorizar? Ainda não conhece o estilo de cobrança da Vunesp?
- É para isso que existe o Projeto Nomeação TJ-SP.
- Uma jornada gratuita e contínua de preparação para os concursos do Tribunal de Justiça de São Paulo.
- Aulas quinzenais de acompanhamento
- Materiais exclusivos para aprofundamento
- Direcionamento para iniciar os estudos corretamente
- Orientações práticas sobre a banca Vunesp
- Conteúdos focados nos temas mais relevantes
- Organização da rotina de estudos
- Preparação consistente durante todo o período pré-edital
- Saiba tudo o que você precisa para cada concurso, que deve sair ainda em 2026!
- Oficial de Justiça
- Escrevente Técnico Judiciário

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma


========================================

---
id_oferta: 016
anunciante: "Isaque Concursos"
url_destino: "https://projetotrt.com.br/vsl1v1/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1023281740551609"
dias_ativo: 65
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "onprofit"
ticket_principal: "R$ 497,00"
fonte_ticket: "checkout"
tipos_produto: "Mentoria / acompanhamento, Cronograma / plano de estudos"
formatos_dos_anuncios: "vídeo (3)"
botoes: "Saiba mais (3)"
parcelas: "12x R$ 42,99"
precos_exibidos_na_lp: "12x de R$ 43 | R$ 9.776,71 | R$ 90,00 | R$ 11.928 | R$ 0 | R$ 997 | R$ 100 | R$ 497"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Tenha organização e direcionamento para
estudar em alto nível para qualquer TRT do
Brasil com essa plataforma 🔥
Depois sair do zero, ter apenas 2h por dia
para estudar e ser aprovado 2x no TRT-PI, 1x
no TRT-PR e 1x no TRT-RS...
Resolvi consolidar o mesmo método que usei em um só lugar.
Mas não apenas isso...
Eu e minha equipe juntamos todos os
materiais, bizus estratégicos, cronograma com
todas as metas e diversas outras ferramentas
em uma plataforma só.
Essa plataforma é o que chamamos de
Projeto TRT.
Além de tudo isso que falei, você ainda terá
mentorias em grupo comigo, painel estatístico
inteligente, cronograma adaptável para a sua
realidade e muito mais.
Sem precisar pagar cursinhos caros, é
exatamente isso que tá fazendo alunos serem
aprovados em diversos TRTs espalhados por
todo Brasil.
Essa é a plataforma ideal para você que não quer
brincar de estudar para os concursos do TRT.
Para você que não quer gastar dinheiro em vão com
cursinhos caros...
É para você que busca estudar em alto nível para ser
aprovado já na próxima prova de TRT que você for
fazer.
Mesmo que você:
• Tenha pouco tempo para estudar;
• Esteja começando os estudos agora;
• Tenha mais de 40 anos;
• Ou seja um concurseiro experiente
Para conhecer essa plataforma que está mudando
completamente o mercado de tribunais, aperte em
"saiba mais".
Na próxima página, te explico com todos os
detalhes. Te espero lá."

### Ganchos das variações (1ª linha de cada anúncio)
- Total organização e direcionamento para
- Tenha organização e direcionamento para

### Títulos do link nos anúncios
- Projeto TRT: Ecossistema Completo para TRTs
- TRTs: Organização e Direcionamento

### Landing Page: Headline & Promessa Central
"Tenha tudo que precisa para estudar em alto nível com organização e direcionamento para o cargo de Técnico Judiciário do TRT e alcance sua aprovação — Mesmo que você tenha apenas 2 horas de estudos por dia ou esteja começando do zero. O mesmo método que usei para ser aprovado no TRT e em outros 3 TRTs, assim como meus alunos aprovados em TRTs."

### Seções da Landing Page (títulos, na ordem)
- Você terá acesso ao pós-edital de todos os TRTs do Brasil
- Pós-edital do TRT-8 (PA/AP)
- Técnico Judiciário – Área Administrativa
- Pré-Edital do TRT
- Este é o momento ideal para começar. Quem espera o edital sair já começa atrasado.
- Uma das melhores áreas de concursos do Brasil
- A onda dos TRTs está chegando
- O melhor custo-benefício entre os concursos
- Quanto mais cedo você começar, maior sua chance de ser aprovado
- TRTs Previstos para 2026, 2027 e 2028
- 3 coisas que você precisa saber
- O cargo que trabalhamos
- Você precisa ter ensino superior
- Prepare-se certo e esteja pronto para qualquer TRT
- Conheça os 3 pilares do Projeto TRT
- Cronograma de Estudos Guiado e Inteligente
- Materiais de Estudo e Links Estratégicos
- Contato Direto com o Mentor
- Estude mesmo com pouco tempo
- Acesso imediato com direção desde o primeiro dia
- Acompanhamento real com quem já passou
- Suporte rápido no WhatsApp
- Veja como o método transforma os estudos antes mesmo da aprovação
- Tudo que você terá acesso ao entrar no Projeto TRT
- Cronograma de Estudos Flexível
- Materiais de Estudos em PDF
- Videoaulas Selecionadas do YouTube
- Grupo Exclusivo no WhatsApp com Isaque
- Mentorias Quinzenais em Grupo com Isaque
- Legislação Organizada por Disciplina

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Discursiva / redação
- Mentoria
- PDF
- Resumos
- Simulados
- Videoaulas


========================================

---
id_oferta: 017
anunciante: "Instituto INAPI"
url_destino: "https://cursos.inapionline.com.br/pre-trt-pi"
ad_library_url: "https://www.facebook.com/ads/library/?id=1054686240270707"
dias_ativo: 55
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 827,00"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Questões / simulados, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (2), imagem (1)"
botoes: "Saiba mais (2), Ver detalhes (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O edital está cada vez mais próximo, e quem quer conquistar uma vaga no TRT/PI precisa começar com estratégia desde já.
No Pré TRT/PI – Preparação Total, você terá:
📚 Turmas para Técnico Judiciário e Analista Judiciário
👨‍🏫 Corpo docente especializado
🎯 10 semanas de preparação intensiva
💻 Opção presencial ou transmissão ao vivo
🎁 BÔNUS: acesso gratuito ao INAPI Questões até 30 de novembro
E tem mais: lote promocional de lançamento válido por apenas 72 horas! ⏰
Não espere o edital sair para começar. Saia na frente e estude com quem mais aprova no Piauí.
📅 Início: 14/09 📍 Garanta sua vaga agora, clique em "Saiba mais""

### Títulos do link nos anúncios
- [ ⭐️ 4.9/5.0 ] Avaliação

### Landing Page: Headline & Promessa Central
"Quem se prepara cedo, sai na frente da concorrência! — Comece agora sua preparação para o TRT-PI e transforme o período pré-edital em vantagem para conquistar sua vaga de Técnico ou Analista Judiciário."

### Seções da Landing Page (títulos, na ordem)
- NOSSAS AULAS

### Entregáveis / Formato (termos encontrados na LP)
- PDF
- Simulados


========================================

---
id_oferta: 018
anunciante: "Nova Concursos"
url_destino: "https://aprovacao.novaconcursos.com.br/curso-gratis-tj-sp-escrevente-ads-ca2"
ad_library_url: "https://www.facebook.com/ads/library/?id=2888791104852798"
dias_ativo: 51
anuncios_coletados: 1
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Questões / simulados, Cronograma / plano de estudos, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (1)"
botoes: "sem botão (1)"
precos_exibidos_na_lp: "R$ 297,00 | R$ 0,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
""📚🆓 Curso Grátis TJ-SP 2026 - Escrevente Técnico Judiciário! 🆓📚
Prepare-se para o TJ-SP 2026 com nosso curso grátis! 🌟
✅ 24 Aulas abrangentes para dominar o conteúdo do TJ-SP 2026.
📅 Plano de Estudos projetado para apenas 1 hora por dia - encaixe nos seus horários.
👨‍🏫 Tutoria Especializada com Professores experientes para esclarecer todas as suas dúvidas.
📝 Questões atualizadas para você praticar e se preparar da melhor maneira.
Inscreva-se agora mesmo e comece sua jornada rumo ao sucesso no TJ-SP 2026! 🚀"

### Landing Page: Headline & Promessa Central
"Prepare-se com a metodologia que já ajudou na aprovação de mais de 70 mil alunos! — De: R$ 297,00"

### Seções da Landing Page (títulos, na ordem)
- Isso vai mudar seu nível de preparação para concursos e você finalmente vai mudar seu status de concurseiro para concursado!
- Trabalha e estuda;
- Tem 1h por dia para se dedicar aos estudos;
- Precisa de ajuda na organização do que estudar até a prova;
- Se sente perdido em meio a tantos materiais e conteúdos.
- Fernanda Marchesini – Aprovada em 1º lugar no INSS
- Marcos Santos – Aprovado no INSS
- 45 dias de Acesso
- 24 Aulas completas para o TJ-SP Escrevente
- Plano de Estudos com 1h por dia
- Tutoria Especializada com Professores
- Questões Atualizadas
- de: R$ 297,00
- R$ 0,00 (ZERO)

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 019
anunciante: "Decorando a Lei Seca Cursos Para Concursos E OAB"
url_destino: "https://www.decorandoaleiseca.com.br/retafinal/analista-judiciario-area-judiciaria-trt-8-regiao"
ad_library_url: "https://www.facebook.com/ads/library/?id=1807015203847696"
dias_ativo: 9
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 397,00"
fonte_ticket: "checkout"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "imagem (2), vídeo (1)"
botoes: "Ver detalhes (2), Saiba mais (1)"
precos_exibidos_na_lp: "12x de R$ 39,55 | R$ 16.040,88 | R$ 18.380,17 | R$ 9.776,71"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps:
  - nome: "Assinatura ILIMITADA Ao incluir esta opção, você garante"
    valor: "R$ 7.997,00"
---
### Copy do Anúncio (Gancho de Entrada)
"EDITAL PUBLICADO: TRT-8ª REGIÃO (PA/AP)
Banca: FCC
Cargos: Analista Judiciário e Técnico Judiciário
Inicial: R$ 9.776,71 a R$ 16.040,88
Vagas: CR
Inscrições: 5/10 a 5/11/2026
Prova Objetiva: 17/01/2027
Reta Final: Lançado! Link na HOME do site!"

### Ganchos das variações (1ª linha de cada anúncio)
- Cronograma de Estudos da Lei Seca do TRT-8 com a legislação exigida no edital, com metas diárias, para você não gastar tempo decidindo por onde começar. Você lê os artigos do dia, treina no Vade Mecum de Questões e revis
- EDITAL PUBLICADO: TRT-8ª REGIÃO (PA/AP)

### Títulos do link nos anúncios
- Analista Judiciário - Área Judiciária (TRT-8)

### Landing Page: Headline & Promessa Central
"Reta Final TRT-8 para Analista e Técnico Judiciário — * Marca registrada no INPI"

### Seções da Landing Page (títulos, na ordem)
- TRT da 8ª Região: o que diz o edital
- Tudo o que entra no Reta Final do TRT-8
- O método é um ciclo de três passos, todo dia.
- Aprovados que estudaram com a plataforma
- Perguntas frequentes

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Mapas mentais
- PDF


========================================

---
id_oferta: 020
anunciante: "cadernodoconcurseiro"
url_destino: "https://cadernodoconcurseiro.com.br/produto/combo-trt-8-tecnico-judiciario-area-administrativa/"
ad_library_url: "https://www.facebook.com/ads/library/?id=3497705397069418"
dias_ativo: 8
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Mapas mentais / esquemas"
formatos_dos_anuncios: "vídeo (3)"
botoes: "Ver detalhes (3)"
precos_exibidos_na_lp: "R$ 10.500,00 | R$ 399,00 | R$ 59,00 | R$ 557,00 | R$ 469,00 | R$ 997 | R$ 147"
primeira_coleta_propria: "2026-10-11"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Estude com o MELHOR combo de mapas mentais para o concurso do TRIBUNAL REGIONAL DO TRABALHO DA 8 REGIÃO.
.
-Material atualizado e didático, separado por disciplina e assunto.
-Cada mapa foi elaborado para ser revisado em MENOS de 1 minuto.
•⁠ ⁠Destaque em cores dos pontos mais cobrados em cada mapa.
•⁠ ⁠O material contempla a lei, doutrina e jurisprudência em um só lugar.
•⁠ ⁠Estude de onde quiser, pelo celular, tablet ou computador.
•⁠ ⁠Revise de uma forma muito mais rápida e eficiente.
.
+ 1 Bônus incluso.
.
Se o seu foco é ser aprovado no concurso da TRT-8 e você está perdido com tanto conteúdo para revisar, não deixe de conhecer os mapas mentais do COMBO TRT-8 MAPEADO e TURBINAR a sua revisão para a prova.
."

### Landing Page: Headline & Promessa Central
"COMBO TRT-8: Técnico Judiciário – Área Administrativa – Caderno do Concurseiro — O COMBO TRT-8 MAPEADO é o caminho para você se tornar TÉCNICO JUDICIÁRIO e garantir a sua"

### Seções da Landing Page (títulos, na ordem)
- O COMBO TRT-8 MAPEADO é o caminho para você se tornar TÉCNICO JUDICIÁRIO e garantir a sua
- ESTABILIDADE FINANCEIRA.
- Completamente diferente de tudo que você já estudou!
- Veja a diferença de estudar pelo nosso material!
- O que você garante ao comprar o Combo TRT-8?
- Se você não tem tempo , esse é o material ideal para você!
- Veja os depoimentos de nossos alunos que melhoraram seu percentual de acertos e já conseguiram as suas aprovações:
- Você quer ser Técnico Judiciário do TRT-8 ?
- Super Bônus Exclusivo!
- Bônus 2!
- 12X 15,20
- ou R$147 à vista
- Você não corre risco algum!
- Luiz Serruya
- Dúvidas frequentes
- Ainda tem Alguma Dúvida?
- Damos valor à sua privacidade
- Cookies estritamente necessários
- Cookies de desempenho
- Cookies de funcionalidade
- Cookies de publicidade

### Entregáveis / Formato (termos encontrados na LP)
- Mapas mentais
- PDF
- Questões comentadas


========================================

---
id_oferta: 021
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2092-concurso-tj-sp-club-escrevente-tecnico-judiciario?utm_source=meta_ads&utm_medium=cpc&utm_campaign=vendas_tj_sp_escrevente"
ad_library_url: "https://www.facebook.com/ads/library/?id=864887869547603"
dias_ativo: 135
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Questões / simulados, Discursiva / redação"
formatos_dos_anuncios: "vídeo (2)"
botoes: "Ver detalhes (2)"
precos_exibidos_na_lp: "R$ 6 | R$ 6.345,94 | R$ 9.007,67 | R$ 1.797,00 | R$ 1.257,90 | 12x de R$ 104,83"
primeira_coleta_propria: "2026-10-09"
dias_distintos_coletado: 3
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O Concurso para Escrevente Técnico Judiciário do Tribunal de Justiça de São Paulo deve ter seu edital publicado em 2026.
Estude com um time professores especialistas em Concursos de Tribunais. No último concurso do TJ-RS 7 dos 10 primeiros colocados foram nossos alunos.
No Club do Ceisc você tem acesso a:
✅ Simulados com foco na banca Vunesp
✅ Resolução de questões ao vivo e gravadas
✅ Fórum de Português ao vivo
✅ Correção de redação
✅ E muito mais!
Matricule-se AGORA em 12x sem juros de R$ 119,75."

### Ganchos das variações (1ª linha de cada anúncio)
- O Concurso para Escrevente Técnico Judiciário do Tribunal de Justiça de São Paulo deve ter seu edital publicado em 2026.
- Já pensou ser Escrevente Técnico Judiciário do TJ-SP, atuar no maior tribunal da América Latina e receber mais de R$ 6 mil/mês?

### Títulos do link nos anúncios
- Aprove com Ceisc

### Landing Page: Headline & Promessa Central
"TJ-SP Club | Escrevente Técnico Judiciário — Sobre o curso"

### Seções da Landing Page (títulos, na ordem)
- Sobre o curso
- Nesse curso você terá
- Conheça os professores
- Sobre a prova
- Conteúdo Programático
- Perguntas frequentes

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Discursiva / redação
- Mentoria
- Planner
- Simulados
- Videoaulas


========================================

---
id_oferta: 022
anunciante: "Brabo Concursos"
url_destino: "https://www.facebook.com/braboconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=4583317258660193"
dias_ativo: 95
anuncios_coletados: 1
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno, Cronograma / plano de estudos, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (1)"
botoes: "sem botão (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O TJ-SP tem um novo concurso previsto para 2026, são mais de 3.300 cargos vagos de Escrevente Técnico Judiciário, temos contrato assinado com a banca organizadora e recentemente foram criados novas 720 vagas de Escrevente.
Lembrando que esse concurso exige só o nível médio, não tem limite de idade e paga um salário inicial de R$ 7.772 reais.
Vou fazer um curso grátis sobre como estudar para o TJ-SP 2026, lá vou te entregar o plano de estudo que eu usei para ser aprovado nesse concurso com 93% de acerto.
Quer começar a estudar agora? Digite “TJSP” nos comentários que eu te ajudo!
#concursopúblico #concursos #concursotjsp #tjsp #escreventetjsp"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 023
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2138-concurso-trt-4-club-tecnico-judiciario-area-administrativa?utm_source=meta_ads&utm_medium=cpc&utm_campaign=vendas_trt_4_club_tec_judiciario&utm_term=advantage"
ad_library_url: "https://www.facebook.com/ads/library/?id=1020843757391368"
dias_ativo: 88
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Curso em videoaulas, Questões / simulados, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (2)"
botoes: "Saiba mais (2)"
precos_exibidos_na_lp: "R$ 9 | R$ 9.776,71 | R$ 9.007,67 | R$ 1.797,00 | R$ 1.257,90 | 12x de R$ 104,83"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Com reajuste de 8% o cargo no judiciário passa a ser mais valorizado. A partir de julho desse ano já entra em vigor,
E para chegar lá, você precisa da preparação que o Ceisc Club tem, confira:
✅ Garantia de atualização do curso na fase pós-edital
✅ Professores especialistas em concursos de Tribunais
✅ Simulados com gabarito comentado
✅ Mentorias ao vivo
✅ Aulas de resolução de questões
✅ Cronogramas de estudos e MUTO MAIS!
Matricule-se agora e e comece a sua preparação antes da concorrência.
Garanta sua Vaga
Ceisc Concursos"

### Ganchos das variações (1ª linha de cada anúncio)
- Com reajuste de 8% o cargo no judiciário passa a ser mais valorizado. A partir de julho desse ano já entra em vigor,
- Um reajuste de 8% já foi aprovado, e o Judiciário ficou ainda mais atrativo.

### Landing Page: Headline & Promessa Central
"TRT-4 Club | Técnico Judiciário - Área Administrativa — Sobre o curso"

### Seções da Landing Page (títulos, na ordem)
- Sobre o curso
- Nesse curso você terá
- Conheça os professores
- Sobre a prova
- Conteúdo Programático
- Perguntas frequentes

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Mentoria
- Planner
- Simulados
- Videoaulas


========================================

---
id_oferta: 024
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://cadernodoaprovado.com/trf-tj-mp/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1533733075435407"
dias_ativo: 68
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 497,00"
fonte_ticket: "checkout"
tipos_produto: "Material em PDF / apostila / caderno, Mapas mentais / esquemas, Lei seca / legislação"
formatos_dos_anuncios: "imagem (1), carrossel (1)"
botoes: "Ver detalhes (1), sem botão (1)"
precos_exibidos_na_lp: "R$ 7.150,91 | R$ 891,00 | 12x de R$ 41,42 | R$ 4.715,48 | R$ 14.852,66 | R$ 1.188,00 | 12x de R$ 53,92 | R$ 9.052,51"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps:
  - nome: "[REDAÇÃO IMBATÍVEL] Guia de redação dissertativa-argumentativa para concursos"
    valor: "R$ 149,00"
  - nome: "[COMBO MP-PE] Técnico Ministerial - Área Administrativa (Nível"
    valor: "R$ 497,00"
  - nome: "[COMBO TRT BRASIL] Técnico Judiciário - Área Adm."
    valor: "R$ 597,00"
  - nome: "[COMBO TRT BRASIL] Analista Judiciário - Área Judiciária"
    valor: "R$ 647,00"
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 O edital do TRF-3 pode sair a qualquer momento!
Enquanto você não sabe por onde começar, quem já está estudando com direcionamento certo larga na frente.
Foi por isso que criei os Cadernos do Aprovado para TRF-3, TJ e MP:
👉 Método que me levou ao 1º lugar no TRT-PI, com 100% de acertos na prova.
✅ Todas as disciplinas do edital, com teoria direto ao ponto
✅ Legislação grifada e esquematizada, pronta pra revisão
✅ Guia de Estudos com plano de metas: o que estudar, em que ordem e quando revisar
✅ Atualizações automáticas quando o edital sair
🎯 Não espere o edital sair para começar. Quem se antecipa chega mais afiado na prova.
📲 Clique em "Saiba mais" e conheça o combo completo para TRF-3, TJ e MP.
---"

### Títulos do link nos anúncios
- Combos TRF, TJ e MP – Caderno do Aprovado – Caderno do Aprovado – Materiais de estudos para concursos públicos
- Combo TRF-3, TJ e MP

### Landing Page: Headline & Promessa Central
"Combos TRF, TJ e MP – Caderno do Aprovado – Caderno do Aprovado – Materiais de estudos para concursos públicos — Prepare-se em alto nível para as próximas grandes oportunidades na área de tribunais."

### Seções da Landing Page (títulos, na ordem)
- Prepare-se em alto nível para as próximas grandes oportunidades na área de tribunais.
- 1º lugar
- O Caderno do Aprovado resolve isso organizando tudo em um só lugar.
- Tudo pronto para estudar, revisar e avançar.
- Conheça por dentro.
- A diferença está em quem faz e em como é feito.
- Oi, eu sou o Beto.
- Estude para os próximos concursos de TRF, TJ e MP com quem conhece o caminho da aprovação.
- (Sem juros)
- GUIA DE ESTUDOS
- Sem riscos, com garantia de 7 dias para ter certeza.
- O material de estudos dos primeiros colocados!
- Estudar sozinho x Estudar com o Caderno do Aprovado
- Para ficar despreocupado(a) pelos próximos 2 anos
- 12x de R$ 116,42
- Dúvidas frequentes e suas respostas.
- Outras dúvidas?
- Não encontrou um combo específico para o seu concurso?

### Entregáveis / Formato (termos encontrados na LP)
- Caderno de erros
- Cronograma
- Discursiva / redação
- PDF
- Resumos
- Videoaulas


========================================

---
id_oferta: 025
anunciante: "JusConc"
url_destino: "https://www.facebook.com/61555120221977/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1070081985496959"
dias_ativo: 57
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf5"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "vídeo (1), imagem (1)"
botoes: "sem botão (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Carreiras Jurídicas / OAB"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Matrículas abertas: Linha Essencial TRF5!
⚠️ Informações importantes para quem não conseguiu acompanhar a live:
* O material será disponibilizado em 10 semanas consecutivas.
* A ordem do conteúdo será definida de acordo com a relevância e incidência em provas de Magistratura Federal e provas da banca FGV. Ou seja, não seguiremos a ordem convencional dos manuais na disposição do conteúdo. Isso evita que você chegue no dia da prova sem ter estudado o que tem de mais relevante para a prova.
* O material da primeira semana estará disponível no dia 21/08.
* Na página do site, vocês conseguem ver o conteúdo de cada disciplina que será abordado em cada semana; basta clicar na semana respectiva.
Qualquer dúvida, estamos à disposição.
Grande abraço!"

### Ganchos das variações (1ª linha de cada anúncio)
- Um pequeno recorte do que foram os 4 dias intensos de curso presencial para a prova oral do TRF1.
- Matrículas abertas: Linha Essencial TRF5!

### Títulos do link nos anúncios
- instagram.com

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 026
anunciante: "Rô Santtana - OAB"
url_destino: "https://rosanttana.com.br/captacao/lp-discursiva-oab.html"
ad_library_url: "https://www.facebook.com/ads/library/?id=1643357417410487"
dias_ativo: 54
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tribunal regional federal, trf1"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Discursiva / redação"
formatos_dos_anuncios: "carrossel (2)"
botoes: "Saiba mais (1), sem botão (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Deixar de questionar uma nota zero em uma resposta que está correta pode custar a sua carteira.
No 42º Exame de Ordem, na prova prático-profissional de Direito do Trabalho, um candidato precisava de apenas 0,45 pontos para confirmar sua aprovação. A diferença entre conquistar a carteirinha ou ter que recomeçar do zero estava concentrada em uma única questão: a Questão 4-A e B.
A banca avaliadora atribuiu nota zero a uma resposta que o próprio espelho de correção mandava pontuar. O candidato apresentou o fundamento e o dispositivo legal corretos, mas os pontos foram negados sem que a banca sequer explicasse a divergência com seus próprios critérios.
Inconformado, ele foi à Justiça contra a OAB. Na primeira instância, sofreu um revés: o juiz negou o pedido usando como argumento o Tema 485 do STF, que impede o Judiciário de reexaminar o mérito de provas de concurso. Parecia que as portas haviam se fechado, mas o jogo virou no Tribunal Regional Federal da 1ª Região (TRF1).
A 13ª Turma do TRF1 teve uma leitura impecável do caso: a discussão não era sobre o mérito da resposta do candidato, mas sim sobre a legalidade da correção. Se a banca contraria o próprio espelho, ela age na ilegalidade.
O resultado? A segurança foi concedida por unanimidade pelos desembargadores, obrigando a OAB a atribuir os pontos que haviam sido negados indevidamente. A OAB ainda tentou recorrer da decisão, mas perdeu novamente no Tribunal.
O recado que fica é claro: quando a banca examinadora foge das suas próprias regras e do próprio espelho, existe caminho jurídico para reverter a nota e garantir a sua aprovação.
Ficou com alguma dúvida ou passou por uma situação parecida?
📲 Clique no link da Bio ou envie uma mensagem no nosso WhatsApp: (51) 99447-6006."

### Ganchos das variações (1ª linha de cada anúncio)
- Deixar de questionar uma nota zero em uma resposta que está correta pode custar a sua carteira.
- Mesma questão, respostas quase iguais: um candidato recebeu zero e o outro, nota máxima.

### Títulos do link nos anúncios
- Reprovado na 2ª Fase da OAB? · Rô Santtana Advogada

### Landing Page: Headline & Promessa Central
"Foi reprovado na 2ª fase do Exame de Ordem por poucos décimos? A correção da sua prova pode estar errada. — O padrão de respostas da FGV não está acima da lei. Quando os critérios de correção não são respeitados ou aplicados de forma divergente, a nota atribuída à sua prova pode ser revisada pela Justiça."

### Seções da Landing Page (títulos, na ordem)
- Você se preparou, entregou uma boa peça e a nota não refletiu isso.
- A preparação
- Se você passou por uma dessas situações, vale a pena buscar uma avaliação do seu caso.
- A peça profissional foi zerada por elemento essencial ausente
- Os critérios aplicados divergem do padrão de respostas da FGV
- O recurso administrativo foi indeferido sem análise individualizada
- Faltaram poucos décimos para os 6,0 da aprovação
- Decisões reais de candidatos que reverteram a nota da 2ª fase.
- Como revisamos a nota da sua 2ª fase.
- Análise da sua prova
- Recurso administrativo, se ainda houver prazo
- Ação judicial com fundamento técnico
- Revisão da nota e habilitação para a advocacia
- Resultados reais. Nas palavras de quem viveu.
- Rô Santtana Advogada
- Acompanhe casos reais no Instagram
- O que talvez esteja te impedindo de lutar pelo seu direito.
- O prazo para agir é de 120 dias.
- Fale agora com nossa equipe

### Entregáveis / Formato (termos encontrados na LP)
- Discursiva / redação


========================================

---
id_oferta: 027
anunciante: "Pratique Concursos"
url_destino: "https://ti.pratiqueconcursos.com.br/fcti/main.html"
ad_library_url: "https://www.facebook.com/ads/library/?id=999076996486447"
dias_ativo: 31
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf, tribunal regional federal"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Mapas mentais / esquemas, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "carrossel (2)"
botoes: "Saiba mais (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Fiscal e Controle"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Prepare-se antes de todo mundo para o Concurso do TRT!
Chegou o Super Resumo Pré-Edital TRT, feito para quem quer começar os estudos antes da publicação do edital — com base no conteúdo completo do último concurso (TRT 2ª Região).
Com nossos resumos diretos ao ponto, você economiza tempo, foca no que realmente cai e ganha vantagem sobre a concorrência.
- Conteúdo 100% focado em TI
- Resumos, esquemas, tabelas e mapas mentais
- Feito por aprovados em concursos da área
- Baixe agora a amostra GRÁTIS e conheça o material que vai te deixar pronto pro edital!
#ConcursoTRT #TI #SuperResumos #PratiqueConcursos #ConcursoPublico #CarreiraTI #EstudoInteligente #ResumoPreEdital"

### Ganchos das variações (1ª linha de cada anúncio)
- Prepare-se antes de todo mundo para o Concurso do TRT!
- Use o Super Resumo para aumentar seu desempenho na busca pela aprovação.

### Títulos do link nos anúncios
- Super Resumos para Concurso TRT
- Super Resumo - Banco do Brasil

### Landing Page: Headline & Promessa Central
"Aumente suas chances de aprovação nos concursos de TI — Pesquise por concurso, curso ou assunto."

### Seções da Landing Page (títulos, na ordem)
- Nenhum material encontrado
- FCTI - Formação Concursado de TI
- Guia para Concursos (GRÁTIS)
- Super Intensivo CGU Pós-Edital
- DATAPREV
- Transpetro
- Super Intensivo SEFAZ SP
- TCE GO - Técnico de Controle Externo (TI)
- SEPLAG RJ - EPPGG (TI)
- SEFAZ AL - Auditor Fiscal
- Discursivas de TI
- TCE SP Pós Edital
- Curso Regular
- TI para Fiscal e Controle
- STM Pré Edital
- Banco do Brasil - Pré Edital
- TCE Pré Edital - Tribunal de Contas do Estado
- Petrobras Pré Edital
- TRF Pré Edital - Tribunal Regional Federal
- TRT Pré Edital - Tribunal Regional do Trabalho
- FLASHCARDS de TI
- Nós, do Pratique Concursos, somos especialistas no ensino de Tecnologia da Informação para concursos públicos.
- Conheça o professor
- Prof. Achiles Júnior
- Pratique Concursos

### Entregáveis / Formato (termos encontrados na LP)
- Discursiva / redação
- Flashcards


========================================

---
id_oferta: 028
anunciante: "Memorização Bruno Campos Concursos"
url_destino: "https://www.facebook.com/100088833677510/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1699256514500630"
dias_ativo: 24
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf, trf 2"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "carrossel (2)"
botoes: "Visitar perfil do Instagram (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Esta imagem marca um momento solene e inesquecível: a posse (15/04/25) do nosso aluno Reili como Juiz Federal do TRF 2 🙏
Mais do que um ato formal, esta cerimônia representa o ponto culminante de uma jornada marcada por esforço silencioso, noites de estudo, superações e um compromisso inabalável com o sonho da magistratura.
Vestir a toga é mais do que alcançar um cargo. É assumir uma missão. É carregar nas mãos a responsabilidade de decidir com justiça, de ouvir com empatia e de transformar o direito em instrumento de dignidade humana.
A partir de agora, cada decisão do Reili impactará vidas. Cada despacho, cada audiência, cada sentença — será escrita por alguém que sabe o que é lutar por cada página lida, por cada aprovação, por cada passo até aqui.
Sua posse não é apenas uma conquista pessoal. É a vitória de todos que acreditam no mérito, na disciplina e na força de quem não desiste — mesmo quando ninguém está olhando.
Que essa nova etapa seja guiada pela sabedoria, pela coragem e por tudo aquilo que o trouxe até aqui.
Reili, que honra ter feito parte da sua caminhada. Hoje o Sistema de Memorização BC se emociona com você.
Parabéns, Reili. Que essa toga te abrace como símbolo de tudo o que você superou — e do quanto merece estar exatamente onde está."

### Ganchos das variações (1ª linha de cada anúncio)
- Esta imagem marca um momento solene e inesquecível: a posse (15/04/25) do nosso aluno Reili como Juiz Federal do TRF 2 🙏
- 🎯 A jornada até a aprovação nunca é fácil... mas é possível!

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 029
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2465-concurso-trf-1-juiz-federal-prova-oral-online"
ad_library_url: "https://www.facebook.com/ads/library/?id=1663276888536516"
dias_ativo: 23
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf, trf 1"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "imagem (2)"
botoes: "Ver detalhes (2)"
precos_exibidos_na_lp: "R$ 37.765,55 | R$ 9.007,67 | R$ 3.859,00 | R$ 2.894,25 | 12x de R$ 241,19"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Futuros magistrados do TRF-1 exigem um nível avançado de preparo.
E na modalidade on-line do Ceisc, você tem acesso a um curso de alta performance, confira:
✅ Gravação, feedback e ficha de avaliação por candidato;
✅ Arguição diagnóstico preliminar individual;
✅ Materiais estratégicos complementares
✅ Grupo estratégico de acompanhamento
✅ Encontro final pré-prova
As vagas são limitadas, garanta sua agora mesmo!"

### Ganchos das variações (1ª linha de cada anúncio)
- TRF-1 em foco?
- Futuros magistrados do TRF-1 exigem um nível avançado de preparo.

### Títulos do link nos anúncios
- Aprove com Especialistas

### Landing Page: Headline & Promessa Central
"TRF-1 | Juiz Federal | Prova Oral | Online — Sobre o curso"

### Seções da Landing Page (títulos, na ordem)
- Sobre o curso
- Nesse curso você terá
- Conheça os professores
- Sobre a prova
- Conteúdo Programático
- Perguntas Frequentes
- Acesse nosso blog

### Entregáveis / Formato (termos encontrados na LP)
- Videoaulas


========================================

---
id_oferta: 030
anunciante: "Prime Curso"
url_destino: "https://sala.concurseiroprime.com.br/buscar?query=trt"
ad_library_url: "https://www.facebook.com/ads/library/?id=1129411490041604"
dias_ativo: 16
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "imagem (2)"
botoes: "Comprar agora (2)"
precos_exibidos_na_lp: "R$ 42,00 | 10x de R$ 42,00 | R$ 1200 | R$ 378,00 | R$ 49,00 | 10x de R$ 49,00 | R$ 1400 | R$ 441,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Prepare-se para o concurso da Tribunal Regional do Trabalho com o Prime. Clique e comece hoje mesmo!"

### Títulos do link nos anúncios
- Curso TRT 65% OFF

### Landing Page: Headline & Promessa Central
"Concurseiro Prime | Busca por "trt""

### Seções da Landing Page (títulos, na ordem)
- [ON-LINE] TRT 8ª REGIÃO (PA/AP) - ANALISTA JUDICIÁRIO - ÁREA JUDICIÁRIA & OFICIAL DE JUSTIÇA - PÓS EDITAL
- [ON-LINE] TRT 8ª REGIÃO (PA/AP) - TÉCNICO JUDICIÁRIO - ÁREA ADMINISTRATIVA - PÓS-EDITAL
- [ON-LINE] TRT 22ª REGIÃO (PI) - ANALISTA JUDICIÁRIO - ÁREA JUDICIÁRIA & OFICIAL DE JUSTIÇA - PRÉ-EDITAL
- [ON-LINE] TRT 22ª REGIÃO (PI) - TÉCNICO JUDICIÁRIO - ÁREA ADMINISTRATIVA - PRÉ-EDITAL
- [ON-LINE] DOBRADINHA | TRT8/TRT22 (TRT PA/AP & TRT PI) - ANALISTA JUDICIÁRIO - ÁREA JUDICIÁRIA & OFICIAL DE JUSTIÇA
- [ON-LINE] DOBRADINHA | TRT8/TRT22 (TRT PA/AP & TRT PI) - TÉCNICO JUDICIÁRIO - ÁREA ADMINISTRATIVA

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 031
anunciante: "Professor Raphael Reis"
url_destino: "https://www.facebook.com/profraphaelreis/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1252750147028904"
dias_ativo: 11
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Questões / simulados, Discursiva / redação"
formatos_dos_anuncios: "imagem (1), carrossel (1)"
botoes: "sem botão (1), Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🔴No universo dos concursos públicos, muitos candidatos concentram sua energia quase exclusivamente nas questões objetivas. De fato, elas são essenciais: funcionam como filtro inicial, abrindo a porta para as etapas seguintes. Mas é preciso compreender com clareza — a verdadeira nomeação, o diferencial que separa os aprovados dos convocados, está na **REDAÇÃO**.
➡A prova objetiva mede o conhecimento técnico, a capacidade de lembrar conteúdos e aplicar regras. Já a redação vai além: avalia organização de ideias, clareza na comunicação, raciocínio lógico, domínio da norma culta, capital cultural, repertório e, principalmente, a capacidade de argumentar de forma estruturada e coerente. Não basta apenas saber — é preciso demonstrar maturidade intelectual e habilidade de expressão.
🔴Quantos candidatos ficam pelo caminho não por falta de acertos nas objetivas, mas por não atingirem a nota mínima na redação? Quantos, mesmo com um bom desempenho nas questões, perdem posições preciosas porque subestimaram o peso do texto argumentativo dissertativo?
✅Portanto, o recado é simples e direto: **NÃO HÁ CONCURSO DE ALTO NÍVEL SEM UM DOMÍNIO SÓLIDO DA ESCRITA .**
🔴Quem deseja não apenas ser aprovado, mas efetivamente ser NOMEADO, precisa tratar a redação como prioridade estratégica. Estudar técnicas de argumentação, treinar produção textual, revisar com rigor e praticar com constância são passos indispensáveis para transformar conhecimento em resultado.
➡A objetiva abre a porta. A redação decide quem entra.
#RedacaoParaConcurso #RedacaoQueAprova #DomineARedacao #RedacaoNotaMil #concursos #trt #temasderedacao #concursospublicos #aulaespecial #TJ #FCC #FGV #TRF #cebraspe #concursopublico #dicadomago #redaçãonota10 #jeitomagodefazerredação #magodaredacao #redaçãoconcurso #redacaoaovivo #cursoderedação #Vunesp"

### Ganchos das variações (1ª linha de cada anúncio)
- 🔴No universo dos concursos públicos, muitos candidatos concentram sua energia quase exclusivamente nas questões objetivas. De fato, elas são essenciais: funcionam como filtro inicial, abrindo a porta para as etapas segui
- Historicamente, desde 2018, os melhores resultados são dos meus alunos 🧙‍♂️

### Títulos do link nos anúncios
- instagram.com

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 032
anunciante: "cadernodoconcurseiro"
url_destino: "https://www.facebook.com/100064118526627/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1101272539160972"
dias_ativo: 9
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Cronograma / plano de estudos"
formatos_dos_anuncios: "carrossel (2)"
botoes: "Visitar perfil do Instagram (2)"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 EDITAL PUBLICADO: CONCURSO TRT-8 (PA/AP)
Saiu o edital do Tribunal Regional do Trabalho da 8ª Região, com banca FCC e remuneração inicial de até R$ 16.040,88! 📚
📌 Resumo rápido:
✅ 24 opções de cargos: 20 de Analista e 4 de Técnico Judiciário
✅ Nível superior para todos, inclusive Técnico
✅ Analista: R$ 16.040,88 | taxa de R$ 110
✅ Técnico: R$ 9.776,71 | taxa de R$ 90
✅ Inscrições de 05/10 a 05/11/2026 em concursosfcc.com.br
✅ Isenção da taxa de 05/10 a 09/10 para inscritos no CadÚnico e doadores de medula óssea
✅ Provas em 17/01/2027, em Belém, Marabá, Santarém e Macapá
👉 Arrasta pro lado e veja os cargos, a estrutura das provas e o cronograma completo!
💾 Salva este post para não perder os prazos e marca aquele amigo que vai estudar com você! 👇"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 033
anunciante: "Site RP"
url_destino: "https://www.trt8.jus.br/noticias/2026/edital-para-concurso-publico-do-trt-8-e-publicado"
ad_library_url: "https://www.facebook.com/ads/library/?id=2510089052822709"
dias_ativo: 9
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Discursiva / redação, Cronograma / plano de estudos, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (2)"
botoes: "Comprar agora (2)"
precos_exibidos_na_lp: "R$ 110,00 | R$ 90,00"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚨SAIU O EDITAL | TRT 8ª Região
💬 Comente “EU QUERO” e receba gratuitamente nosso cronograma de estudos!
Concurso Público
Banca: FCC
Inscrições: 05/10/2026 até 05/11/2026.
Prova objetiva e discursiva: 17/01/2027.
Cargos:
🔹 Analista Judiciário | Especialidade Enfermagem 40h: CR | R$ 16.040,88
🔹 Técnico Judiciário | Especialidade Enfermagem 40h: CR | R$ 9.776,71
Conteúdo programático: Conhecimentos Gerais, Conhecimentos Específicos e Redação.
Locais de prova: Belém/PA, Marabá/PA, Santarém/PA e Macapá/AP
Edital: https://www.trt8.jus.br/noticias/2026/edital-para-concurso-publico-do-trt-8-e-publicado
📚 Comece já sua preparação:
👉 www.romulopassos.com.br"

### Landing Page: Headline & Promessa Central
"Edital para concurso público do TRT-8 é publicado — O edital para a realização de concurso público para preenchimento de vagas e formação de cadastro de reserva de cargos do quadro permanente de pessoal do Tribunal Regional do Trabalho da 8ª região já está publicado no Diário Oficial da União. Confira o edital completo AQUI!"

### Seções da Landing Page (títulos, na ordem)
- Você está aqui
- Links rápidos

### Entregáveis / Formato (termos encontrados na LP)
- Discursiva / redação


========================================

---
id_oferta: 034
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/categorias/concursos?subcategorie=trf-1-magis&utm_source=facebook&utm_medium=cpc&utm_campaign=vendas_trf_1_juiz_federal"
ad_library_url: "https://www.facebook.com/ads/library/?id=888699670925217"
dias_ativo: 137
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf, trf 1"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno"
formatos_dos_anuncios: "imagem (1)"
botoes: "Ver detalhes (1)"
precos_exibidos_na_lp: "R$ 1.597,60 | 12x de R$ 133,13 | R$ 1.437,84 | R$ 2.497,00 | 12x de R$ 208,08 | R$ 2.247,30 | R$ 949,00 | 12x de R$ 79,08"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Seu cargo como magistrado pode estar mais próximo. E cada dia importa nessa fase decisiva.
Por isso, a modalidade híbrida de preparação do Ceisc + JusFederal foi estruturada com foco em treino prático, com segurança e referências nacionais na área que conhecem a banca examinadora.
➡️ Acesse o site e inscreva-se no curso preparatório."

### Títulos do link nos anúncios
- Aprove com Especialistas

### Landing Page: Headline & Promessa Central
"Confira nossos cursos preparatórios de Concursos e fique um passo mais perto de conquistar o seu sonho. — Concursos"

### Seções da Landing Page (títulos, na ordem)
- Cursos de Concursos
- Confira nossos cursos preparatórios de Concursos e fique um passo mais perto de conquistar o seu sonho.

### Entregáveis / Formato (termos encontrados na LP)
- Discursiva / redação
- Mentoria


========================================

---
id_oferta: 035
anunciante: "Concursosmeucurso"
url_destino: "https://meucurso.com.br/cursos/concursos-publicos"
ad_library_url: "https://www.facebook.com/ads/library/?id=1542521100851019"
dias_ativo: 81
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf3, tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "carrossel (1)"
botoes: "Saiba mais (1)"
precos_exibidos_na_lp: "R$ 350 | R$ 2.999,00 | 12x de R$ 149,92 | R$ 1.799,00 | 12x de R$ 99,92 | R$ 1.199,00 | 12x de R$ 139,92 | R$ 1.679,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"TRF3, TJSP e TSE/TREs estão entre os concursos mais aguardados do momento, com centenas de cargos previstos e remuneração inicial que pode ultrapassar R$ 18 mil.
Se o seu objetivo é conquistar estabilidade e uma carreira no serviço público, este é o momento de começar sua preparação.
No MeuCurso, você encontra cursos completos para chegar competitivo quando o edital for publicado. E, durante a promoção de aniversário, ainda garante até 78% OFF em cursos selecionados.
Quem começa antes estuda com mais tranquilidade, consolida o conteúdo e aumenta as chances de aprovação.
Invista na sua preparação hoje e aproveite as condições especiais antes que a promoção termine."

### Títulos do link nos anúncios
- Concursos com remuneração de até R$ 18 mil

### Landing Page: Headline & Promessa Central
"Curso Preparatório para Concursos Jurídicos — Concursos Públicos"

### Seções da Landing Page (títulos, na ordem)
- Preparação direcionada para concursos com foco em resultado.
- Navegue pela categoria que melhor combina com seu objetivo
- COMECE SEUS ESTUDOS AGORA!
- Por onde começar sua preparação para concursos
- Vanessa Netto | @van.netto
- Thamirys Calandro | @thamiscalandro
- Mykarla Francyelli | @mykarlafrancyelli
- Alexandre A Brollo | @alexandreabrollo
- Érika Teixeira | @erika.txra
- Barbie do Direito | @barbiedodireito
- Ouvidoria do CFOAB – Como apresentar uma reclamação por erro material no Exame de Ordem?
- Escala 9&#215;1: supermercado é condenado a pagar 594 horas extras e indenização por danos morais
- Exigência de depósito prévio para internação emergencial é ilegal: análise do caso no TJSP
- ENAM | Assinatura
- TSE/ TREs - Unificado | Assinatura
- Tribunais | Assinatura
- Formação Essencial | Assinatura
- Procuradorias | Assinatura
- 6º ENAM 2026.2 - Online - início 08/09
- Procuradorias FCC | Resolução de Questões - online
- Procuradoria do Estado de São Paulo | Peças Práticas
- Regular Procuradorias Estaduais e Municipais
- Procuradorias Municipais e Estaduais | Peças Práticas
- Combo Escrevente TJ/SP + Analista MPSP
- Analista do MPSP | Pré-Edital Online
- OAB + Residência Jurídica TJ/SP
- Escrevente Técnico Judiciário TJ/SP | Regular Pré-Edital
- Escrevente Técnico Judiciário TJ/SP | Treino de Questões - Pré- Edital
- Escrevente Técnico Judiciário TJ/SP | Treino de Questões + Regular - Pré- Edital
- TRF3 - Analista Judiciário - Área Judiciária | Pré-Edital - Online

### Entregáveis / Formato (termos encontrados na LP)
- PDF
- Simulados


========================================

---
id_oferta: 036
anunciante: "Atleta dos Concursos - OAB"
url_destino: "https://www.facebook.com/61582789201469/"
ad_library_url: "https://www.facebook.com/ads/library/?id=958630850523730"
dias_ativo: 79
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "vídeo (1)"
botoes: "sem botão (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Carreiras Jurídicas / OAB"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Eu acredito que eu posso te ajudar. Por quê?
✅ Eu fiz direito na UFRJ e passei na OAB no 9º período com 1 mês de estudo. Em 2011.
✅ Virei concurseiro em 2012 virei concurseiro.
✅ Foram 5 anos só me preparando para concursos públicos.
✅ Reprovei em mais de 15 provas de carreiras jurídicas, foram muitos erros e aprendizados.
✅ Obtive 6 aprovações em provas de 1ª fase, de procuradorias, defensoria pública e outras carreiras.
✅ Obtive 2 grandes aprovações: Advogado do BNDES e Advogado da União na AGU, que é um dos concursos mais difíceis do Brasil.
✅ Em 2017 fui nomeado como Advogado da União.
✅ Desde então já são 9 anos atuando na advocacia pública.
✅ Defendendo a União, eu já participei de processos com cifras bilionárias. Já despachei com juízes, desembargadores, fiz sustentações orais no TRF, enfim, tive uma atuação em processos bem relevantes.
✅ Fora o grande acervo que já passou pela minha mão, é realmente uma experiência de milhares e milhares de processos.
✅ Atualmente na AGU sou Coordenador de uma equipe com mais de 20 Advogados da União, semanalmente passam por essa Coordenação que eu lidero mais de 2 mil processos.
✅ E depois que eu entrei na AGU, eu também me tornei mentor para concursos, já orientei a preparação de milhares de alunos nos mais diversos concursos públicos, com aprovações em advocacia pública, magistratura, o ENAM, que é o Exame Nacional da Magistratura pela FGV, para carreiras fiscais, policiais, de tribunais etc .
✅ Eu conheço a FGV de uma longa data, sei exatamente como vencer essa banca.
Então sim, eu confio que eu posso te ajudar, eu sei como te orientar por um caminho seguro até a sua aprovação na OAB.
Aí eu te pergunto: você quer ser ajudado por mim?
É só clicar no link da bio e se inscrever no meu Treinamento para a 1ª fase da OAB.
Vamos pra cima!"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 037
anunciante: "Decorando a Lei Seca Cursos para Concursos LTDA"
url_destino: "https://www.decorandoaleiseca.com.br/assinatura-ilimitada"
ad_library_url: "https://www.facebook.com/ads/library/?id=1022898813852937"
dias_ativo: 74
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 539,99"
fonte_ticket: "checkout"
tipos_produto: "Assinatura / clube / vitalício, Questões / simulados, Lei seca / legislação"
formatos_dos_anuncios: "vídeo (1)"
botoes: "Ver detalhes (1)"
precos_exibidos_na_lp: "R$ 7.999,90 | 12x de R$ 53 | R$ 539,99 | 12x de R$ 39,65 | 12x de R$ 53,99 | R$ 14 | 12x de R$ 42,67 | R$ 427,49"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Carreiras Policiais"
order_bumps:
  - nome: "Ilimitada Vitalícia Dupla Ao incluir esta opção, o"
    valor: "R$ 447,00"
  - nome: "Ilimitada Vitalícia TRIPLA Ao incluir esta opção, você"
    valor: "R$ 15.999,80"
---
### Copy do Anúncio (Gancho de Entrada)
"🎯 O Anaor Gomes sentiu na pele o que todo concurseiro sabe: não dá para ignorar a legislação seca se você quer a aprovação. Atualmente, ele é o 2º colocado no Ranking do Vade Mecum de Questões. Somente no ano de 2025, ele foi aprovado nos certames:
✅ Aprovado no MPU (Analista Oficial)
✅ Aprovado no TRF 5ª Região
✅ +80% de acertos na 1ª fase de Delegado do Ceará
✅ Aprovado na prova objetiva de Delegado da Polícia Federal
📲 Toque no link e saiba mais!"

### Landing Page: Headline & Promessa Central
"Todos os Retas Finais para sempre — Faça parte de uma comunidade gigantesca. Em média, 1 em cada 5 aprovados nos maiores concursos jurídicos do país estudou conosco."

### Seções da Landing Page (títulos, na ordem)
- Plataforma validada por mais de 310.000 usuários
- Casos de sucesso
- Conheça a plataforma por dentro
- Raio-X da Lei Seca por banca
- Bancas já liberadas
- Como usar
- Quem usou, validou o método
- Assinatura Anual
- Ilimitada Vitalícia
- Risco Zero: 7 dias de garantia
- Dúvidas Frequentes

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Mapas mentais
- PDF


========================================

---
id_oferta: 038
anunciante: "Golden Cursos Jurídicos"
url_destino: "https://www.facebook.com/100083153801246/"
ad_library_url: "https://www.facebook.com/ads/library/?id=4430567703874887"
dias_ativo: 60
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno"
formatos_dos_anuncios: "carrossel (1)"
botoes: "Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Radar de Aprovações Golden: Magistratura
Cruzamos os resultados recentes de quatro concursos de magistratura, dois estaduais (TJPR e TJGO) e dois federais (TRF-6 e TRF-1), com a base de alunos GoldenJus, direto nas publicações oficiais das bancas e dos tribunais. Em todos, havia aluno nosso."

### Títulos do link nos anúncios
- GoldenJus | Preparatório Carreiras Jurídicas e Pós (@goldenjus_oficial) • Instagram photos and videos

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 039
anunciante: "Hugo de Freitas com 123 Questões"
url_destino: "https://go.123questoes.com.br/lp/tribunais/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1781444589524819"
dias_ativo: 18
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados, Discursiva / redação, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (1)"
botoes: "Saiba mais (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Se você estuda pra Tribunal e ainda treina com questão genérica, está treinando pra prova errada.
Dia 13 de outubro chega a nova Área de Tribunais da 123 Questões: questões inéditas, simulados, ranking, correção de discursivas e muito mais, no padrão das bancas de TRF, TRT e TJ.
Entre no Grupo VIP e tenha acesso antecipado e condições especiais no lançamento.
👉 Clica em Saiba mais."

### Títulos do link nos anúncios
- Plataforma de Questões para Tribunais!

### Landing Page: Headline & Promessa Central
"A nova área de Tribunais está chegando. — E quem chegar primeiro leva vantagem."

### Seções da Landing Page (títulos, na ordem)
- Por que a gente resolveu criar essa área
- Agora com uma área dedicada a Tribunais.
- Todas as ferramentas da 123 Questões
- Questões inéditas, escritas só para esses concursos
- Simulados exclusivos de Tribunais
- Uma comunidade só de quem estuda para Tribunais
- Sua redação corrigida sem precisar esperar dias.
- Você escreve e envia
- A IA analisa seu texto
- Você recebe a devolutiva
- Os primeiros assinantes terão condições e vantagens especiais.
- Condições especiais de lançamento
- Acesso antecipado
- Novos recursos primeiro
- Benefícios exclusivos
- Não deixe para descobrir depois.

### Entregáveis / Formato (termos encontrados na LP)
- Discursiva / redação
- Questões comentadas
- Simulados


========================================

---
id_oferta: 040
anunciante: "Joy Braga Concursos"
url_destino: "https://detoxconcursos.com.br/tribunais/?src=a2d330ebaa55430aaa643cc71bc84863&utm_content=%7B%7Bad.id%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=2078859239389190"
dias_ativo: 16
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno, Questões / simulados"
formatos_dos_anuncios: "vídeo (1)"
botoes: "Saiba mais (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O modelo de cursinho tradicional foi feito pra você desistir. E está funcionando.
800 videoaulas. Apostila de 500 páginas. Simulado de banca que nem é a sua.
Quanto mais tempo você fica lá, melhor pro negócio deles.
Você não precisa de mais conteúdo. Precisa estudar o que a sua banca cobra, do jeito que ela cobra, e ignorar o resto sem culpa.
TRT, STJ, TRF: a janela está aberta. E ela não vai esperar você terminar a aula número 340.
Toca em Saiba mais e veja como estudar pela banca, não pelo cursinho."

### Títulos do link nos anúncios
- O cursinho não quer que você passe

### Landing Page: Headline & Promessa Central
"Detox Tribunais — A revolução das bancas de concurso já está acontecendo"

### Seções da Landing Page (títulos, na ordem)
- Falta pouco pra garantir sua vaga

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 041
anunciante: "Advocacia para Concursos - Mattozo & Ribeiro"
url_destino: "https://www.facebook.com/100089931653062/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1934024137978229"
dias_ativo: 16
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf, tribunal regional federal"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "imagem (1)"
botoes: "sem botão (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Conseguimos a confirmação de uma importante vitória em favor de um candidato diagnosticado tardiamente com Transtorno do Espectro Autista (TEA).
Por unanimidade, a 6ª Turma do Tribunal Regional Federal da 1º Região (TRF-1) rejeitou os recursos apresentados pela União e pelo Cebraspe e manteve a sentença que assegurou ao nosso cliente o direito de alterar sua modalidade de inscrição no Concurso Público Nacional Unificado da Justiça Eleitoral para concorrer às vagas reservadas às pessoas com deficiência (PCD).
Ele havia se inscrito na ampla concorrência porque, naquele momento, ainda não possuía diagnóstico conclusivo de autismo. A confirmação ocorreu somente em fevereiro de 2025, quando o período de inscrições já havia terminado. Ainda antes da divulgação do resultado final do concurso, ele pediu administrativamente a alteração da modalidade de concorrência, mas seu requerimento foi negado.
Na Justiça, obtivemos sentença favorável. Com os recursos da União e do Cebraspe, o caso chegou ao TRF-1, que agora confirmou o direito reconhecido em primeira instância. O que pouca gente acreditava, aliás. Mas nossa tese se mostrou pertinente e foi acolhida pela Corte Federal.
A decisão ganhou destaque em reportagem publicada pelo Brasil37, que abordou o caráter inédito do acórdão e a relevância da tese para candidatos que recebem o diagnóstico somente depois das inscrições. Confira um trecho da reportagem:
📍 “Atenta às especificidades do caso concreto, aos princípios da razoabilidade e da proporcionalidade, e, ainda, aplicando-se o princípio pro persona na interpretação das normas, revela-se excepcionalmente possível viabilizar a alteração da inscrição como pessoa com deficiência no certame em questão, conferindo, assim e na espécie, proteção mais ampla ao direito da parte”, registrou a desembargadora Kátia Balbino, relatora, em seu voto.
É mais um resultado de nossa atuação na defesa dos direitos de candidatos PCD e, especialmente, daqueles que recebem diagnósticos após o encerramento das inscrições em concursos públicos.
Leia a reportagem e confira o acórdão na íntegra! O link está na aba ‘Resultados’!
#MattozoERibeiro #ConcursoPúblico #DiagnósticoTardio #PCD"

### Títulos do link nos anúncios
- instagram.com

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 042
anunciante: "Olivie Advocacia"
url_destino: "https://www.facebook.com/61588831809684/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1715318876236791"
dias_ativo: 16
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf, tribunal regional federal"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "imagem (1)"
botoes: "Enviar mensagem (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O Tribunal Regional Federal da 1ª Região (TRF-1) reafirmou o entendimento de que candidatos que obtiveram o diagnóstico tardio de autismo podem buscar o reconhecimento do seu direito às vagas reservadas para Pessoa com Deficiência (PcD) em concursos públicos, mesmo que tenham efetuado a inscrição inicial pela Ampla Concorrência. Se você prestou um concurso público e recebeu o diagnóstico de TEA posteriormente, saiba que é possível submeter a documentação para análise das vias adequadas e verificação da viabilidade do seu direito.
Consulte um advogado especialista para avaliar o seu caso.
Consulte um advogado especialista e tire dúvidas pelo WhatsApp.
Advocacia compromissada com a inclusão e a garantia dos seus direitos."

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 043
anunciante: "Legislação Integrada"
url_destino: "https://www.legislacaointegrada.com.br/trf5/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1023457034050771"
dias_ativo: 13
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf, tribunal regional federal, trf5, trf 5"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 377,00"
fonte_ticket: "checkout"
tipos_produto: "Assinatura / clube / vitalício, Lei seca / legislação"
formatos_dos_anuncios: "carrossel (1)"
botoes: "Saiba mais (1)"
precos_exibidos_na_lp: "R$ 350,00 | R$ 37.765,55 | R$ 394,90 | R$ 377 | R$ 307"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Foi publicado o edital do concurso para Juiz Federal - TRF-5.
São 11 vagas com remuneração de R$ 37.765,55.
Também já está disponível para todos os assinantes do Clube da Lei um plano de leitura 100% focado no edital do concurso!
O plano permite um estudo completo das principais leis cobradas no edital bem como da jurisprudência pertinente em 89 dias.
Lembrando que a letra do material é grande e a formatação em coluna única. Em regra, você precisará de aproximadamente 4 horas para cumprir a meta do dia.
-> ATENÇÃO! Caso você já siga o Plano-base de Magistratura Estadual, o módulo adicional possui apenas 30 dias.
Mais informações em: http://www.legislacaointegrada.com.br/trf5"

### Títulos do link nos anúncios
- TRF 5

### Landing Page: Headline & Promessa Central
"TRF 5 — Tribunal Regional Federal da 5ª Região"

### Seções da Landing Page (títulos, na ordem)
- Tribunal Regional Federal da 5ª Região
- Concurso para Juiz Federal Substituto
- Detalhes do concurso
- Plano de Leitura: Magistratura - TRF-5
- Número aproximado de páginas
- Número de dias
- Média de páginas por dia
- Número de leis contempladas
- Formato dos arquivos
- Informações gerais
- Leis contempladas no Plano de Leitura
- Esse e vários outros planos de leitura estão disponíveis para todos os assinantes do Clube da Lei!
- Gostaria de um estudo dinâmico e organizado para o concurso?
- Você sabia que em torno de 70% das questões de concurso cobram lei seca? Ainda assim você acha o estudo de lei seca monótono e pouco produtivo?
- Nós também! Mas existe um jeito de estudar a lei seca de uma forma dinâmica e integrada !
- Conheça o
- Saiu no site do Planalto, caiu no Legislação Integrada
- Material atualizado semanalmente através de um informativo especialmente formulado.
- Benefícios de fazer parte do Clube
- Chega de perder tempo
- Estude de forma organizada. É só escolher um plano de leitura e seguir!
- Planos de leitura
- Planos de leitura 100% baseados nas carreiras.
- Mais de 180 Leis
- Leis organizadas por metas, com letras grandes, destaques e tabelas.
- Material Atualizado
- O material é semanalmente atualizado e divulgamos um informativo te contando as novidades.
- Legislação Integrada em Questões
- Uma experiência completamente nova. Estudo da Lei Seca através de mais de 3,5 mil questões especialmente formuladas!
- Acesso Ilimitado

### Entregáveis / Formato (termos encontrados na LP)
- PDF


========================================

---
id_oferta: 044
anunciante: "Curso Ênfase"
url_destino: "https://www.facebook.com/cursoenfase/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1935904854235176"
dias_ativo: 11
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf2, trf5"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "carrossel (1)"
botoes: "Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Concurso de juiz em 2027: TJDFT e os seis TRFs aparecem com previsão no Projeto de Lei Orçamentária.
O TRF2 e o TRF5 planejam concurso para juiz todo ano, de 2027 a 2030. Os demais preveem novos certames em 2029 ou 2030. O TRF5 explica o motivo: são 51 cargos de juiz federal substituto vagos, e o número de aprovados fica sempre abaixo do número de vagas.
É previsão, não autorização, e o texto ainda passa pelo Congresso. A lição para quem estuda é outra: concurso de juiz é ciclo, não evento. A base comum às magistraturas federal e estadual está nas oito disciplinas fundamentais, e a porta de entrada é o ENAM.
Salve e envie para quem está na magistratura.
#magistratura #juizfederal #tjdft #concursojuiz #enam
Conteúdo educativo e de análise técnica. Não constitui orientação jurídica para casos concretos."

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 045
anunciante: "América Capital"
url_destino: "https://lp.americacapital.com.br/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1087922147551559"
dias_ativo: 11
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 1
sinal_tracao: "fraco"
foco_direto: sim
termos_foco_encontrados: "trf"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (1)"
botoes: "Fale conosco (1)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"<100
Advogado(a), por que esperar o cronograma do TRF se você pode reinvestir seus honorários hoje?
Sabemos que o fluxo de caixa de um escritório previdenciarista pode ser um desafio. Você vence o processo, mas a liquidez da RPV Federal demora a chegar. Na America Capital, antecipamos seus honorários contratuais e sucumbenciais em até 72 horas.
✅ Sem consulta ao SPC/Serasa.
✅ Processo 100% digital e seguro.
✅ Liquidez imediata para expansão ou marketing.
Transforme sua carteira de RPVs em capital de giro agora. Entre em contato já com nossa equipe!"

### Títulos do link nos anúncios
- Receba seus Honorários de RPV em até 72h

### Landing Page: Headline & Promessa Central
"America Capital | Antecipação de RPVs"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 046
anunciante: "Vade Focus"
url_destino: "https://app.vadefocus.com.br/curso/pe-magistratura-discursiva-2026"
ad_library_url: "https://www.facebook.com/ads/library/?id=1088376647505771"
dias_ativo: 10
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 1
sinal_tracao: "fraco"
foco_direto: sim
termos_foco_encontrados: "trf"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Discursiva / redação"
formatos_dos_anuncios: "imagem (1)"
botoes: "Saiba mais (1)"
precos_exibidos_na_lp: "R$ 597,00 | R$ 997,00 | R$ 99,70"
primeira_coleta_propria: "2026-10-09"
dias_distintos_coletado: 3
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"<100
Cursos completos de sentença cível e criminal para a 2ª etapa do TJPE.
Curso de sentença cível com Dr. Rogério Cunha (TJPR)
Curso de sentença criminal com Dr. Michael Procópio (TRF)
Manual de Sentenças e banco de modelos
Correção humana, sem IA (contratada à parte)
Provas escritas em 6 e 7 de dezembro
10x sem juros de R$ 99,70 ou R$ 997 à vista. Cupom VADE10: 10% off até 20/10."

### Títulos do link nos anúncios
- Cursos de sentença cível e criminal · Manual de Sentenças e banco de modelos · Sentença cível e criminal: TJPE

### Landing Page: Headline & Promessa Central
"Discursiva TJPE · Edital 01/2026 — Um plano detalhado até a data da prova!"

### Seções da Landing Page (títulos, na ordem)
- Conheça o curso
- Quem ensina você
- Trilha de estudos
- O que acontece na 2ª etapa do TJPE
- Um plano possível de executar
- A técnica da resposta discursiva
- Análise da banca + resumos da produção acadêmica
- Cursos teóricos (aulas virtuais)
- Pratique a sentença cível, no padrão do TJPE
- Pratique a sentença penal, no padrão do TJPE
- Simule a prova: 04 simulados completos para o TJPE e + 8 bônus!
- Seja corrigido, sem IA, por quem conhece essa prova
- Datas oficiais
- outubro, 2026
- 12 de outubro
- Também incluído
- Por que VadeFocus
- Metodologia pensada para quem quer passar na prova.
- SEGURO REPROVAÇÃO
- GARANTIA 15 DIAS
- Investimento
- Curso completo
- Ainda está com dúvidas?
- Ainda não saiu o resultado da 1ª fase. Vale a pena comprar agora?
- Já tem data para a 2ª etapa?
- O curso cobre as sentenças ou só a prova discursiva?
- Como é a prova discursiva do TJPE?
- E a prova de sentença?
- O que posso levar para a prova?
- As aulas são gravadas ou ao vivo?

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Discursiva / redação
- PDF
- Resumos
- Simulados
- Videoaulas


========================================

---
id_oferta: 047
anunciante: "oliberal.com"
url_destino: "https://www.facebook.com/oliberal/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1154864303742580"
dias_ativo: 9
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Discursiva / redação"
formatos_dos_anuncios: "carrossel (1)"
botoes: "Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"OPORTUNIDADES
O Tribunal Regional do Trabalho da 8ª Região (TRT-8), que abrange os estados do Pará e do Amapá, publicou o edital de abertura do novo concurso público para o quadro permanente de pessoal. O certame oferece oportunidades para 24 cargos e especialidades, com formação de cadastro de reserva. Os salários iniciais chegam a R$ 16.040,88 para cargos de nível superior. As inscrições serão abertas às 10h do dia 5 de outubro e poderão ser feitas até as 23h59 de 5 de novembro de 2026, pelo horário de Brasília.
O concurso será organizado pela Fundação Carlos Chagas (FCC) e prevê provas objetivas e discursivas para os cargos de Analista Judiciário e Técnico Judiciário. Para a especialidade de Agente da Polícia Judicial, também haverá uma etapa de avaliação física. De acordo com o edital, as provas estão previstas para 17 de janeiro de 2027, nas cidades de Belém, Marabá e Santarém, no Pará, e Macapá, no Amapá.
Saiba mais em Oliberal.com
📝O Liberal
📸Marcelo Seabra / Agência Pará / Arquivo"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

# Parte 2 — Ofertas adjacentes (83)

Apareceram nas buscas, mas não citam os termos do foco. Servem para comparar formatos e preços de outros nichos de concurso; algumas não são de concurso.

---
id_oferta: 048
anunciante: "Gustavo Dias"
url_destino: "https://lp.gdconcursos.com.br/mentoria-df"
ad_library_url: "https://www.facebook.com/ads/library/?id=1847014503140089"
dias_ativo: 9
anuncios_coletados: 3
anuncios_ativos_estimados: 30
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (3)"
botoes: "sem botão (3)"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🔥 A sua aprovação em Concursos Públicos não depende dos Materiais! Depende de direcionamento correto.
Se você tá perdido sem saber como começar ou já estuda mas sente que não evolui, está correndo um sério risco de ficar anos sem a sua aprovação.
A verdade é simples:
❌ Não é falta de esforço
❌ Não é falta de inteligência
✅ É falta de estratégia certa e personalizada pra VOCÊ
Com a Mentoria Premium, você não vai receber acompanhamento genérico ou em grupo.
Você vai ter:
✔️ Um plano de estudos 100% personalizado
✔️ Acompanhamento individual comigo
✔️ Estratégia validada na prática
✔️ Suporte completo (inclusive no emocional)
✔️ Direcionamento até atingir nível de aprovação (85%+)
Sem promessas milagrosas. Sem enrolação.
Apenas o que realmente funciona.
💰 Concursos com salários de até R$20.000 estão ao seu alcance — mas você precisa do caminho certo.
👉 Clique agora para tirar um diagnóstico e conhecer a Mentoria Premium"

### Landing Page: Headline & Promessa Central
"GD Concursos"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 049
anunciante: "Sou Concurseiro"
url_destino: "https://www.facebook.com/souconcurseiroevoupassaroficial/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2192944634623317"
dias_ativo: 9
anuncios_coletados: 15
anuncios_ativos_estimados: 23
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "vídeo (15)"
botoes: "sem botão (15)"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Tem mais de 30, 40 ou 50 anos e já tem ensino superior? O Tribunal de Justiça do Amazonas pode ser a sua transição de carreira."

### Ganchos das variações (1ª linha de cada anúncio)
- Requisitos do concurso do TJ-AM: não tem limite de idade e, para analista, vale qualquer curso superior, inclusive tecnólogo.
- Acabou a faculdade ou vai se formar este ano? O concurso do TJ-AM pode ser o seu próximo passo.
- As disciplinas que você já pode começar a estudar para o concurso do TJ-AM.
- Qualquer curso superior, salário acima de R$ 15 mil e jornada das 8h às 14h: esse é o concurso do TJ-AM.
- FGV, Cebraspe ou FCC: qual banca vai organizar o próximo concurso do TJ-AM?
- Acha que já passou da idade para estudar? No TJ-AM tem gente de 30, 40 e 50 anos se preparando agora.

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 050
anunciante: "Decorando a Lei Seca Cursos Para Concursos E OAB"
url_destino: "https://www.decorandoaleiseca.com.br/assinatura-ilimitada"
ad_library_url: "https://www.facebook.com/ads/library/?id=4550468205196169"
dias_ativo: 16
anuncios_coletados: 4
anuncios_ativos_estimados: 19
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "hotmart"
ticket_principal: "R$ 539,99"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Assinatura / clube / vitalício, Mapas mentais / esquemas, Questões / simulados, Lei seca / legislação"
formatos_dos_anuncios: "imagem (4)"
botoes: "sem botão (3), Ver detalhes (1)"
precos_exibidos_na_lp: "R$ 7.999,90 | 12x de R$ 53 | R$ 539,99 | 12x de R$ 39,65 | 12x de R$ 53,99 | R$ 14 | 12x de R$ 42,67 | R$ 427,49"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Carreiras Jurídicas / OAB"
order_bumps:
  - nome: "Ilimitada Vitalícia Dupla Ao incluir esta opção, o"
    valor: "R$ 447,00"
  - nome: "Ilimitada Vitalícia TRIPLA Ao incluir esta opção, você"
    valor: "R$ 15.999,80"
---
### Copy do Anúncio (Gancho de Entrada)
"Três ferramentas. Um mesmo objetivo: transformar o seu estudo em aprovação. 🎯
Você não precisa apenas ler mais a lei seca. Precisa saber o que memorizar, como revisar e onde concentrar seus esforços.
É exatamente para isso que desenvolvemos três ferramentas que se complementam:
📘 Vade Mecum de Questões: estude a legislação por meio de questões reais, organizadas por artigo. Descubra como cada dispositivo é cobrado e memorize os detalhes que fazem diferença na prova.
🧠 Mapas Mentais: são mais de 2.500 mapas para transformar dispositivos legais em esquemas visuais, facilitando a compreensão, a revisão e a memorização.
📊 Raio-X da Lei Seca: descubra quais artigos são mais cobrados em cada código e lei, com estatísticas baseadas nas principais bancas. Assim, você direciona seu tempo para aquilo que realmente merece sua atenção.
O segredo não é estudar tudo com a mesma intensidade. É estudar com estratégia, revisar com inteligência e treinar o que efetivamente cai.
E com a Ilimitada do DLS, você tem acesso a essas ferramentas em um só lugar, pelo computador, tablet ou celular.
🚀 Sua aprovação começa com a forma como você estuda hoje.
👉 Conheça a Ilimitada do Decorando a Lei Seca e transforme sua preparação."

### Ganchos das variações (1ª linha de cada anúncio)
- Três ferramentas. Um mesmo objetivo: transformar o seu estudo em aprovação. 🎯
- 5 aprovações em um só ano.

### Títulos do link nos anúncios
- Assinatura ILIMITADA | Acesse Todos os Cursos | Decorando a Lei Seca

### Landing Page: Headline & Promessa Central
"Todos os Retas Finais para sempre — Faça parte de uma comunidade gigantesca. Em média, 1 em cada 5 aprovados nos maiores concursos jurídicos do país estudou conosco."

### Seções da Landing Page (títulos, na ordem)
- Plataforma validada por mais de 310.000 usuários
- Casos de sucesso
- Conheça a plataforma por dentro
- Raio-X da Lei Seca por banca
- Bancas já liberadas
- Como usar
- Quem usou, validou o método
- Assinatura Anual
- Ilimitada Vitalícia
- Risco Zero: 7 dias de garantia
- Dúvidas Frequentes

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Mapas mentais
- PDF


========================================

---
id_oferta: 051
anunciante: "Portal & OAB"
url_destino: "https://olympus.cursosdoportal.com.br/o-adm-tj-pb/?utm_source=%7B%7Bsite_source_name%7D%7D&utm_medium=%7B%7Badset.name%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D&utm_term=%7B%7Bplacement%7D%7D&utm_content=%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1046187021716727"
dias_ativo: 9
anuncios_coletados: 11
anuncios_ativos_estimados: 11
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (3), imagem (8)"
botoes: "Ver detalhes (3), sem botão (8)"
precos_exibidos_na_lp: "R$ 7.033,78"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O Tribunal de Justiça da Paraíba (TJPB) avançou na preparação de um novo concurso público com a Fundação Getulio Vargas (FGV) definida como banca organizadora. A seleção prevê inicialmente 50 vagas, com o quantitativo oficial a ser confirmado no edital.
As oportunidades devem contemplar o cargo de Analista Judiciário, incluindo áreas de Tecnologia da Informação e Contadoria, para candidatos de nível superior. A remuneração inicial de referência é de R$ 7.033,78. O concurso segue em preparação, e a data das provas ainda não foi divulgada.
No grupo de estudos, você terá acesso a materiais gratuitos, orientações de estudo, resolução de questões e atualizações sobre cargos, edital, inscrições, provas e todas as etapas do concurso.
Clique em “Saiba Mais” e entre no grupo de WhatsApp para receber materiais gratuitos e acompanhar todas as novidades do concurso do TJPB.
See Details"

### Landing Page: Headline & Promessa Central
"Seu próximo capítulo: TJ/PB. — Dê o primeiro passo com direção e material gratuito no grupo de estudos do Portal Concursos."

### Seções da Landing Page (títulos, na ordem)
- 50 oportunidades previstas
- Uma oportunidade. Um novo caminho.
- Analista Judiciário
- Previsão de 50 vagas para servidores
- Nível superior
- Fundação Getulio Vargas — FGV
- Datas ainda não anunciadas
- Preparação que sai da intenção.
- Materiais gratuitos
- Foco no objetivo
- Preparação em grupo
- Comece antes do edital
- Estudar é individual. Evoluir pode ser coletivo.
- O Portal de quem decidiu ir além.
- O edital ainda está por vir. Sua preparação pode começar hoje.

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma


========================================

---
id_oferta: 052
anunciante: "Central de Concursos"
url_destino: "https://centraldeconcursos.com.br/concursos/concurso-tj-sp-escrevente"
ad_library_url: "https://www.facebook.com/ads/library/?id=28037481829210668"
dias_ativo: 89
anuncios_coletados: 4
anuncios_ativos_estimados: 10
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "vídeo (4)"
botoes: "sem botão (4)"
precos_exibidos_na_lp: "R$ 8.872,54"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O concurso do Tribunal de Justiça de São Paulo (TJ-SP) é uma das maiores oportunidades para quem tem apenas o ensino médio completo. Além de um excelente salário inicial, você conquista estabilidade financeira, benefícios de alimentação, transporte, saúde e um plano de carreira real.
Mas tem um detalhe que muda o jogo: quem espera o edital sair para começar a estudar, já larga atrás. ⏳❌
Chegou a hora de ter uma preparação completa para garantir a sua vaga. Não deixe o seu futuro para depois!
🚀 Quer conquistar a sua estabilidade?
Cadastre-se e conheça a preparação da Central de Concursos."

### Ganchos das variações (1ª linha de cada anúncio)
- O TJ-SP Escrevente é uma grande oportunidade para quem busca estabilidade e carreira pública com nível médio.
- O concurso do Tribunal de Justiça de São Paulo (TJ-SP) é uma das maiores oportunidades para quem tem apenas o ensino médio completo. Além de um excelente salário inicial, você conquista estabilidade financeira, benefício

### Landing Page: Headline & Promessa Central
"Concurso TJ SP - Escrevente · Central de Concursos — Vem aí novo Concurso TJ SP para Escrevente"

### Seções da Landing Page (títulos, na ordem)
- Vem aí novo Concurso TJ SP para Escrevente
- Você conhece essa sensação?
- Estudar sozinho é uma batalha injusta.
- O que muda quando você conquista sua vaga
- Para quem é essa oportunidade?
- Informações do concurso
- Concurso TJ SP - Escrevente
- Preparação completa e direcionada para sua aprovação no concurso.
- Metodologia direta ao ponto
- Especialistas em provas das principais bancas
- Aulas presenciais com especialistas
- Preparação 360º
- Aqui na Central, você escolhe como quer estudar.
- Presencial
- Live (Aulas ao Vivo)
- O que dizem nossos aprovados
- Dê o próximo passo na sua preparação para o TJ SP.
- Vamos começar?
- Sua aprovação começa aqui

### Entregáveis / Formato (termos encontrados na LP)
- Simulados


========================================

---
id_oferta: 053
anunciante: "Decorando a Lei Seca Cursos Para Concursos E OAB"
url_destino: "https://www.facebook.com/decorandoaleisecaconcursoseoab/"
ad_library_url: "https://www.facebook.com/ads/library/?id=443284988264992"
dias_ativo: 924
anuncios_coletados: 9
anuncios_ativos_estimados: 9
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Questões / simulados, Lei seca / legislação"
formatos_dos_anuncios: "vídeo (3), imagem (3), carrossel (3)"
botoes: "sem botão (6), Visitar perfil do Instagram (3)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Carreiras Policiais"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O art. 20 do Código Penal é daqueles dispositivos que merecem atenção especial na preparação. 👀📚
Considerando os artigos indicados no cabeçalho das questões analisadas no Vade Mecum de Questões, o dispositivo já apareceu em 31 questões, envolvendo tanto o caput quanto seus §§ 1º, 2º e 3º.
E não se trata de uma cobrança isolada: o art. 20 já foi exigido em provas de Juiz de Direito, Delegado de Polícia, Defensor Público, Promotor de Justiça, Procurador do Estado, Policial Penal, Auditor Fiscal, além da OAB, entre outras carreiras.
As cobranças vão de 2006 a 2026, com questões recentes de bancas como FGV, FCC, VUNESP, CEBRASPE, IDECAN e Instituto AOCP. Em 2026, por exemplo, o dispositivo apareceu nas provas para Agente da PC-SC e Policial Penal da SEJUSP-MG.
📌 Moral da história: erro de tipo, descriminantes putativas, erro determinado por terceiro e erro sobre a pessoa são temas que não podem passar batidos na revisão da Parte Geral do CP.
No Vade Mecum de Questões, você consegue estudar a lei seca já vinculada às questões que efetivamente cobraram cada dispositivo.
👉 Salve este post para revisar o art. 20 antes da prova e envie para quem também está estudando para concursos."

### Ganchos das variações (1ª linha de cada anúncio)
- EDITAL PUBLICADO: TRT-8ª REGIÃO (PA/AP)
- ⚠️ Uma palavra pode mudar completamente o gabarito da questão.
- O Código Penal usa a mesma técnica de redação em dois artigos diferentes, e as bancas cobram a diferença exatamente do mesmo jeito.
- Lançados em abril de 2026
- O art. 20 do Código Penal é daqueles dispositivos que merecem atenção especial na preparação. 👀📚
- JUIZ FEDERAL TRF-5: EDITAL PUBLICADO!

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 054
anunciante: "Ceisc Concursos"
url_destino: "https://ceisc.com.br/cursos/2609-mp-pe-analista-ministerial-area"
ad_library_url: "https://www.facebook.com/ads/library/?id=2083764205550271"
dias_ativo: 52
anuncios_coletados: 4
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Curso em videoaulas, Material em PDF / apostila / caderno, Questões / simulados, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (4)"
botoes: "Ver detalhes (2), Saiba mais (2)"
precos_exibidos_na_lp: "R$ 7.150,91 | R$ 9.007,67 | R$ 1.199,00 | R$ 839,30 | 12x de R$ 69,94"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"A comissão responsável pelo novo edital está formada!
Comece a estudar com direcionamento, em um curso atualizado a cada novidade do edital.
Aqui você conta com:
✅ TAQ — Técnica de Aprendizagem por Questões;
✅ Cronograma de estudos;
✅ Mentorias personalizadas
✅ Simulados exclusivos
✅ Caderno de estudo e progresso
✅ Atualização integral do conteúdo após a publicação do novo edital
E muito mais!
Inicie sua preparação antes do edital e saia na frente para a prova."

### Ganchos das variações (1ª linha de cada anúncio)
- A comissão responsável pelo novo edital está formada!
- Não espere o edital para iniciar seus estudos!
- Oportunidade prevista!
- Os 10 novos cargos de Analista Ministerial reforçam o cenário de oportunidade para quem mira o MP-PE.

### Títulos do link nos anúncios
- MP-PE

### Landing Page: Headline & Promessa Central
"MP-PE | Analista Ministerial – Área Jurídica | Extensivo — Sobre o curso"

### Seções da Landing Page (títulos, na ordem)
- Sobre o curso
- Nesse curso você terá
- Conheça os professores
- Sobre a prova
- Conteúdo Programático
- Perguntas frequentes
- Blog CEISC

### Entregáveis / Formato (termos encontrados na LP)
- Caderno de erros
- Cronograma
- Discursiva / redação
- Mentoria
- Simulados
- Videoaulas


========================================

---
id_oferta: 055
anunciante: "Ceisc Concursos"
url_destino: "https://ceisc.com.br/cursos/2237-concurso-ceisc-tribunais-analista-premium"
ad_library_url: "https://www.facebook.com/ads/library/?id=1342835614275761"
dias_ativo: 46
anuncios_coletados: 4
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "imagem (3), carrossel (1)"
botoes: "Ver detalhes (2), Saiba mais (1), sem botão (1)"
precos_exibidos_na_lp: "R$ 9.007,67 | R$ 2.853,00 | R$ 1.997,10 | 12x de R$ 166,42"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O Carreiras Tribunais é um preparatório extensivo de 12 ou 24 meses focado em concursos de múltiplos órgãos, como TJs, TRFs, MPs, DPEs, PGEs e mais.
Essa é a sua chance de estudar com conteúdos mapeados a partir das principais bancas, como FCC, FGV, Cebraspe, Vunesp e +.
Com o Ceisc, você tem um preparo direcionado com especialistas que já viveram a rotina de concursos.
2026 pode ser o ano de virada na sua carreira profissional.
Escolha estudar com especialistas.
Clique abaixo e inicie já!"

### Ganchos das variações (1ª linha de cada anúncio)
- Se você já decidiu seguir carreira nos Tribunais, precisa de uma preparação direcionada com um time referência.
- O Carreiras Tribunais é um preparatório extensivo de 12 ou 24 meses focado em concursos de múltiplos órgãos, como TJs, TRFs, MPs, DPEs, PGEs e mais.
- Você sabe quais oportunidades quer alcançar. Agora, precisa se preparar para cada uma delas!
- Estudar para Tribunais exige mais do que conteúdo: demanda método, organização e constância.

### Títulos do link nos anúncios
- Equipe de Especialistas
- Ceisc Tribunais Analista | Premium

### Landing Page: Headline & Promessa Central
"Ceisc Tribunais Analista | Premium"

### Seções da Landing Page (títulos, na ordem)
- Sobre o curso
- Nesse curso você terá
- Conheça os professores
- Assista a um panorama das vagas em 2026 e 2027
- Sobre a prova
- Conteúdo Programático
- Este curso inclui:

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Discursiva / redação
- Mentoria
- Simulados
- Videoaulas


========================================

---
id_oferta: 056
anunciante: "Decorando a Lei Seca Cursos para Concursos LTDA"
url_destino: "https://pay.hotmart.com/V105573917A?off=k5lhuvlx&checkoutMode=10&offDiscount=BLUEANDORANGE"
ad_library_url: "https://www.facebook.com/ads/library/?id=3611047645738873"
dias_ativo: 16
anuncios_coletados: 4
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "hotmart"
ticket_principal: "R$ 499,99"
fonte_ticket: "checkout"
tipos_produto: "Assinatura / clube / vitalício, Material em PDF / apostila / caderno, Mapas mentais / esquemas, Questões / simulados, Lei seca / legislação, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (4)"
botoes: "Ver detalhes (4)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps:
  - nome: "Ilimitada Vitalícia Dupla Ao incluir esta opção, o"
    valor: "R$ 497,00"
  - nome: "Ilimitada Vitalícia TRIPLA Ao incluir esta opção, você"
    valor: "R$ 15.999,80"
---
### Copy do Anúncio (Gancho de Entrada)
"Entre agora na campanha mais forte já aberta para a Ilimitada e garanta acesso vitalício ao ecossistema completo do Decorando a Lei Seca: Vade Mecum de Questões, Raio-X da Lei Seca, cronogramas, mapas mentais, legislação em PDF, Decorando a Jurisprudência e futuros lançamentos."

### Títulos do link nos anúncios
- Ilimitada Vitalícia - Blue & Orange Sale

### Landing Page: Headline & Promessa Central
[não capturada — status da LP: direct_checkout]

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 057
anunciante: "Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24"
url_destino: "https://ataticadaaprovacao.com.br/?utm_source=fbads&utm_medium=%7B%7Badset.name%7D%7D&utm_campaign=%7B%7Bad.name%7D%7D&utm_content=%7B%7Bplacement%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1685357465868904"
dias_ativo: 86
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Flashcards, Lei seca / legislação, Discursiva / redação, Cronograma / plano de estudos"
formatos_dos_anuncios: "carrossel (3)"
botoes: "Saiba mais (3)"
precos_exibidos_na_lp: "R$ 189,90 | R$ 279,90 | R$ 179,90 | R$ 199,90 | R$ 269,90 | R$ 229,90"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Fiscal e Controle"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"COMBO AUDITOR FISCAL | 39.988 FLASHCARDS
✅ Administração Financeira e Orçamentária - 995 cards
✅ Contabilidade Geral, Pública, Avançada e de Custos - 3096 cards
✅ Direito Administrativo Avançado - 5635 cards
✅ Direito Constitucional Avançado - 4422 cards
✅ Direito Tributário com Reforma Tributária - 1635 cards
✅ Direito Penal + Legislação Especial - 4260 cards
✅ E mais 12 matérias completas
Mais de 900 vagas na área fiscal previstas
Método comprovado. Revisão científica. Material pronto.
BÔNUS:
→ Resumo em PDF
→ Cronograma do Nomeado
→ Aula ensinando a estudar
→ Discursiva nota 1000
Use: 150FF para desconto adicional
Clique em "Saiba Mais"."

### Ganchos das variações (1ª linha de cada anúncio)
- Prepare-se para o Banco do Brasil!
- COMBO AUDITOR FISCAL | 39.988 FLASHCARDS

### Títulos do link nos anúncios
- Prepare-se para o Banco do Brasil!
- COMBO AUDITOR FISCAL

### Landing Page: Headline & Promessa Central
"Acelere sua aprovação com flashcards inteligentes. — O algoritmo devolve cada card no dia em que você está prestes a esquecê-lo. Você revisa menos, lembra mais e chega na prova com o conteúdo ativo."

### Seções da Landing Page (títulos, na ordem)
- Decks em destaque
- CÂMARA DOS DEPUTADOS: ANALISTA LEGISLATIVO
- CARREIRAS JURÍDICAS
- ANPD: AGÊNCIA NACIONAL DE PROTEÇÃO DE DADOS
- CARREIRAS POLICIAIS
- AUDITOR FISCAL
- BACEN: TÉCNICO DO BANCO CENTRAL (NIVEL MÉDIO)
- CGU AUDITOR FEDERAL DE FINANÇAS E CONTROLE (AFFC)
- COMBO TRIBUNAIS - ÁREA ADMINISTRATIVA E JUDICIÁRIA
- Materiais adicionados recentemente
- RECEITA FEDERAL: ANALISTA-TRIBUTÁRIO DA RECEITA FEDERAL
- TCE GO: Técnico de Controle Externo
- SEFAZ ALAGOAS AL AUDITOR 2026
- SEFAZ SC 2026 Auditor Estadual de Finanças Públicas
- Prof. Rodrigo Marengo
- Principais aprovações de alunos
- O poder dos flashcards para sua aprovação
- Memorização ativa
- Economiza tempo
- Resultados perceptíveis
- Navegue por categorias
- Concursos
- Matérias básicas
- Matérias isoladas
- Histórias de aprovação
- Perguntas frequentes
- Comece agora sua jornada para aprovação

### Entregáveis / Formato (termos encontrados na LP)
- Anki
- Flashcards
- PDF


========================================

---
id_oferta: 058
anunciante: "Gazeta dos Concursos"
url_destino: "https://lp.aprovacaoagil.com.br/vsl-white-trt-noticia"
ad_library_url: "https://www.facebook.com/ads/library/?id=1006548205812121"
dias_ativo: 79
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno, Lei seca / legislação"
formatos_dos_anuncios: "vídeo (3)"
botoes: "Saiba mais (3)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"A maior leva de TRTs da última década está entrando na fila. 14 provas até o final de 2027 — uma atrás da outra.
Técnico entra em R$11.500 iniciais, topo passa de R$20 mil. Analista de Direito, R$18 mil iniciais. Jornada de 35 horas por semana, teletrabalho.
Só que enxurrada de edital não te salva se você começa pelo lado errado. 500 horas de videoaula e 15 mil páginas de PDF não dão tempo.
O caminho é virar a ordem: questão comentada, gabarito destrinchado, lei seca e súmula do TST. Foi assim que a Diana fechou entre as 10 primeiras na objetiva do TRT-SP na reta final.
Assiste o vídeo e clica no botão — a ordem completa pra chegar nessa enxurrada pronto."

### Ganchos das variações (1ª linha de cada anúncio)
- Qual o melhor concurso de tribunal pra você começar hoje?
- Qual concurso te bota mais rápido em R$11.500 iniciais com qualquer graduação — inclusive tecnólogo?
- A maior leva de TRTs da última década está entrando na fila. 14 provas até o final de 2027 — uma atrás da outra.

### Títulos do link nos anúncios
- Melhor tribunal pra começar hoje
- O caminho mais rápido pra R$11.500
- A enxurrada de TRTs começou

### Landing Page: Headline & Promessa Central
"Título"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 059
anunciante: "Matheus Santos - Eu concursado"
url_destino: "https://seraprovado.com/mentoria-matheussantos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1059387566661056"
dias_ativo: 75
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento"
formatos_dos_anuncios: "vídeo (3)"
botoes: "Ver detalhes (3)"
precos_exibidos_na_lp: "R$ 10.000,00 | R$ 8 | R$ 15 | 12x de R$ 249,28 | R$ 2497 | 12x de R$ 399,03 | R$ 3997"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Muita gente estuda há anos e continua sem passar. Quase nunca é falta de esforço. É falta de direção.
Na Mentoria Lumia, o Prof. Matheus Santos monta um plano individual para cada caso: foco no seu concurso, o que estudar em cada semana e, principalmente, o que cortar.
Mais de 100 aprovações em concursos de Tribunais, Polícias e federais.
As vagas são limitadas e a entrada é por aplicação.
HTTPS://SERAPROVADO.COM/MENTORIA-MATHEUSSANTOS/
De anos estudando a nomeado"

### Landing Page: Headline & Promessa Central
"Mentoria Prof. Matheus - seraprovado.com — Implemente com meu acompanhamento individual o método que já levou concurseiros do “estudando há anos sem passar” pra servidor público concursado, com salário de + R$ 10.000,00 por mês."

### Seções da Landing Page (títulos, na ordem)
- A Lumia não é uma mentoria comum.
- HISTÓRIAS REAIS E VIDAS TRANSFORMADAS
- Você tomou a decisão de
- virar servidor público?
- Talvez agora mesmo você esteja:
- Você é aprovado quando estuda muito o que cai, não todo o edital
- O que é o Programa Lumia?
- O que está incluso na Mentoria Lumia:
- Quem lidera o programa?
- Prof. Matheus Santos
- Pra quem é a
- Mentoria Lumia?
- Pra concurseiros decididos
- Pra quem está começando
- Pra quem já estuda há tempo
- Pra quem quer aprovação com previsibilidade
- Mais alguns motivos pra você aplicar:
- Acesso ao método validado por +100 aprovados
- Suporte de verdade, não genérico
- Implantação rápida
- Aprovação com previsibilidade
- Plano pra quem TRABALHA
- Investimento
- Após sua aplicação ser aprovada, conversamos sobre o plano que melhor encaixa no seu cenário. Os formatos disponíveis hoje são:
- A próxima pessoa a sair do "estudando há anos sem passar" pra servidor público concursado pode ser você.

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Mentoria
- Simulados
- Videoaulas


========================================

---
id_oferta: 060
anunciante: "Revolução Concursos"
url_destino: "https://www.facebook.com/61576683587518/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1423969583205016"
dias_ativo: 48
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Questões / simulados"
formatos_dos_anuncios: "carrossel (2), vídeo (1)"
botoes: "Visitar perfil do Instagram (2), sem botão (1)"
primeira_coleta_propria: "2026-10-09"
dias_distintos_coletado: 3
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Comenta SIMULADO aqui embaixo que eu te mando o link pra você começar a estudar de graça agora. 🦊
Agosto chegou recheado de oportunidade, mas tem uma coisa que não espera por ninguém: o prazo de inscrição. ⏳
Reuni concursos que estão com as inscrições abertas agora, de várias áreas e salários, uns pra nível médio e outros pra superior.
Alguns fecham já nos próximos dias, então se você tava esperando o momento certo pra começar, ele é agora. Depois que o prazo passa, não tem como voltar atrás.
Corre, se inscreve no seu e já começa a estudar pra chegar preparado.
Salva esse post e segue a @revolucao.concursos pra não ficar de fora do mundo dos concursos. 🦊"

### Ganchos das variações (1ª linha de cada anúncio)
- Comenta SIMULADO aqui embaixo que eu te mando o link pra você começar a estudar de graça agora. 🦊
- Comenta REV aqui embaixo que a gente te manda o simulado gratuito com IA pra você começar a estudar agora. 🦊

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 061
anunciante: "Esmafe RS"
url_destino: "https://www.esmafe.org.br/curso/1015-intensivo-exame-nacional-da-magistratura-enam"
ad_library_url: "https://www.facebook.com/ads/library/?id=1811347033230662"
dias_ativo: 13
anuncios_coletados: 2
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "carrossel (2)"
botoes: "Saiba mais (1), Enviar mensagem pelo WhatsApp (1)"
precos_exibidos_na_lp: "R$ 1.610,00 | R$ 540,70 | R$ 1.622,10 | R$ 1.666,19 | R$ 612,25 | R$ 1.836,75 | R$ 349,24 | R$ 2.095,44"
primeira_coleta_propria: "2026-10-09"
dias_distintos_coletado: 3
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Carreiras Policiais"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"9 magistrados em exercício. 4 deles já aprovados no ENAM.
Esse é o corpo docente do Curso Intensivo ENAM 2026 da ESMAFE/RS — a escola pioneira em magistratura federal no Brasil.
Deslize e conheça quem vai estar do seu lado na preparação mais importante da sua carreira. 👉
📅 Início: 17 de agosto
🔒 Vagas limitadas — 1º lote promocional
Garanta sua vaga 👇
#ENAM2026 #Magistratura #MagistraturaFederal #JuizFederal #ESMAFE #ESMAFERS #ConcursoPublico #DireitoFederal #FGV #CarreiraJuridica"

### Títulos do link nos anúncios
- Conheça quem vai te preparar para o ENAM.

### Landing Page: Headline & Promessa Central
"INTENSIVO EXAME NACIONAL DA MAGISTRATURA (ENAM) | ESMAFE-RS — Conteúdo Programático e Corpo Docente"

### Seções da Landing Page (títulos, na ordem)
- INTENSIVO EXAME NACIONAL DA MAGISTRATURA (ENAM)
- Conteúdo Programático e Corpo Docente
- AULÃO AO VIVO (PÓS EDITAL)
- DIREITO ADMINISTRATIVO
- DIREITO CIVIL
- DIREITO CONSTITUCIONAL
- DIREITO EMPRESARIAL
- DIREITO PENAL
- DIREITO PROCESSUAL CIVIL
- DIREITOS HUMANOS
- NOÇÕES GERAIS DE DIREITO E FORMAÇÃO HUMANÍSTICA
- Tenho Interesse
- 1 - Seus dados
- Nome do Professor
- Iniciar uma conversa pelo WhatsApp

### Entregáveis / Formato (termos encontrados na LP)
- Simulados


========================================

---
id_oferta: 062
anunciante: "Sou Concurseiro"
url_destino: "https://fabiomsam-cloud.github.io/sou-webinario-52b91323/?w=tjam"
ad_library_url: "https://www.facebook.com/ads/library/?id=1645268970311368"
dias_ativo: 9
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Lei seca / legislação"
formatos_dos_anuncios: "vídeo (3)"
botoes: "Saiba mais (3)"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Captura de Lead (Isca Digital / Lista de Espera)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 Tudo sobre concurso do TJ-AM + Plano Perfeito — aula ao vivo com o Prof. Fábio
Participe do Webinário e ganhe o VADE MECUM - Legislação TJ-AM 2026
👉 Clique agora em Saiba Mais e preencha para entrar na sala de aula agora"

### Landing Page: Headline & Promessa Central
"Aula ao vivo — garanta sua vaga"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

## Demais adjacentes (resumo)

| id | Anunciante | Dias | Anúncios | Tração | Ticket (checkout) | Destino |
|---|---|---|---|---|---|---|
| 063 | Memoriza-aí Concursos | 9 | 3 | médio | Não confirmado | https://memorizaai.com.br/trt-8/?src=&utm_source=facebook-ads&utm_medium=%7B%7Ba |
| 064 | Noticiou | 8 | 3 | médio | Não confirmado | https://linkdehoje.online/conteudo-exclusivo/ |
| 065 | Concursos Ceisc | 255 | 2 | médio | Não confirmado | https://ceisc.com.br/cursos/2070-concurso-tj-ba-analista-judiciario-area-judicia |
| 066 | Concursos Ceisc | 194 | 2 | médio | Não confirmado | https://ceisc.com.br/cursos/2067-concurso-tj-sp-club-oficial-de-justica?utm_sour |
| 067 | Pódio Tribunais | 174 | 2 | médio | Não confirmado | https://api.whatsapp.com/send |
| 068 | Prof.carlosgoncalves | 124 | 2 | médio | Não confirmado | https://typebot.co/plataformaanalistadetribunais |
| 069 | Concursos Ceisc | 88 | 2 | médio | Não confirmado | https://ceisc.com.br/cursos/2331-concurso-experiencia-carreiras-2026 |
| 070 | Estratégia Concursos | 87 | 2 | médio | Não confirmado | https://www.facebook.com/EstrategiaConcursos/ |
| 071 | Venâncio & Delgado - Advogados | 61 | 2 | médio | Não confirmado | https://api.whatsapp.com/send |
| 072 | Venâncio & Delgado - Advogados | 61 | 2 | médio | Não confirmado | https://www.facebook.com/venancioedelgadoadvogados/ |
| 073 | Concursos Ceisc | 60 | 2 | médio | Não confirmado | https://ceisc.com.br/cursos/2584-concurso-dpe-pb-tecnico-da-defensoria-publica |
| 074 | Concurseiro Fora da Caixa | 60 | 2 | médio | Não confirmado | https://concurseiroforadacaixa.com.br/collections/todos-os-materiais |
| 075 | Concursos Ceisc | 54 | 2 | médio | Não confirmado | https://ceisc.com.br/cursos/2089-concurso-trt-4-club-analista-judiciario-area-ju |
| 076 | G7 Jurídico | 52 | 2 | fraco | Não confirmado | https://materiais.g7juridico.com.br/pdf-questoes/cadastro |
| 077 | Lucas Viégas | 47 | 2 | médio | Não confirmado | https://foconocontrole.com.br/ |
| 078 | Comunidade de Aprovados com Helena Emerick Abaurre | 46 | 2 | médio | Não confirmado | https://form.respondi.app/9QZkseoW |
| 079 | Decorando a Lei Seca Cursos Para Concursos E OAB | 16 | 2 | médio | R$ 927,50 | https://www.decorandoaleiseca.com.br/ilimitada-vitalicia-dupla |
| 080 | GG Concursos | 10 | 2 | médio | Não confirmado | https://ggconcursos.com.br/cursos/gg-play/gg-play-vitalicio-360 |
| 081 | Giovanna Carranza Desenvolvimento Profissional | 9 | 2 | médio | Não confirmado | https://carranzacursos.com.br/trf8/?utm_source=mta-ads |
| 082 | Helena Emerick Abaurre com Comunidade de Aprovados | 9 | 2 | médio | Não confirmado | https://pay.plataformatutory.com.br/checkout/af51c9d5-01c3-4988-8e18-2fd62561f10 |
| 083 | IPOG - Pernambuco | 8 | 2 | médio | Não confirmado | https://ipog.edu.br/cursos/pos-graduacao/avaliaces-e-pericias-de-engenharia-pos- |
| 084 | Delta Fabio Silva | 8 | 2 | médio | Não confirmado | https://www.facebook.com/deltafabiosilva/ |
| 085 | Mentoria Tribunal do Trabalho | 8 | 2 | médio | Não confirmado | https://www.facebook.com/61566455297489/ |
| 086 | Flávio Britto Advocacia | 8 | 2 | médio | Não confirmado | https://www.facebook.com/flaviobrittoadvocacia/ |
| 087 | Concursos Ceisc | 234 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/https-ceisc-com-br-cursos-2042-concurso-banco-do-bra |
| 088 | Concursos Ceisc | 214 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2274-concurso-mp-mg-extensivo-premium-analista-do-mp |
| 089 | euvoupassei com Aprovação PGE | 184 | 1 | médio | Não confirmado | https://aprovacaopge.com.br/ |
| 090 | Ceisc Concursos | 181 | 1 | médio | Não confirmado | https://lp.ceisc.com.br/evento-concursos-nivel-medio/ |
| 091 | Gaby no Tribunal | 178 | 1 | médio | Não confirmado | https://www.facebook.com/100090566482087/ |
| 092 | Ceisc Concursos | 150 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2429-concurso-mp-sc-analista-juridico-extensivo?utm_ |
| 093 | Discursiva na Prática | 129 | 1 | médio | R$ 1.489,00 | https://discursivanapratica.com.br/assinaturacontrole/?utm_source=facebook&utm_m |
| 094 | Douglas Prado - Servidor 30k | 106 | 1 | médio | Não confirmado | https://odouglasprado.com.br/plano-servidor-30k/ |
| 095 | Fauth e Freitas Sociedade de Advogados com Adriane Fauth | 95 | 1 | médio | Não confirmado | https://www.facebook.com/61573224123970/ |
| 096 | Brabo Editora | 86 | 1 | médio | R$ 397,00 | https://braboeditora.com.br/mestre-em-questoes-tjsp-v8/ |
| 097 | Ludy Sena | 86 | 1 | médio | Não confirmado | https://www.facebook.com/ludysena.perita/ |
| 098 | LH no pódio | 80 | 1 | médio | Não confirmado | https://typebot.co/mentoria-zeroaopodio |
| 099 | Trteiros | 75 | 1 | médio | Não confirmado | https://www.facebook.com/61560675890210/ |
| 100 | Mege | 69 | 1 | médio | Não confirmado | https://concurcity.mege.com.br/explorar |
| 101 | Themas Cartórios | 67 | 1 | médio | Não confirmado | http://www.themas.com.br/ |
| 102 | Professora Amanda Aires | 57 | 1 | médio | Não confirmado | https://www.amandaaires.com.br/curso/%5B2026%5D-economia-para-o-tcu/345 |
| 103 | Concursos Ceisc | 53 | 1 | médio | Não confirmado | https://www.sympla.com.br/produtor/ceisc |
| 104 | Advogado de concurso | 48 | 1 | médio | Não confirmado | https://olivaesouza.com.br/tjsc-objetiva-nivel-superior-conhecimentos-gerais/ |
| 105 | Jus Expert | 48 | 1 | médio | R$ 997,00 | https://pages.jusexpert.com/vsl-grafotecnica-principal |
| 106 | Gustavo Nogueira - Aprovação Ágil | 46 | 1 | médio | Não confirmado | https://lp.aprovacaoagil.com.br/vsl-white-trt-noticia |
| 107 | Jus Expert | 46 | 1 | médio | R$ 997,00 | https://pages.jusexpert.com/vsl-papiloscopia-principal |
| 108 | Capriata Educação | 46 | 1 | médio | Não confirmado | https://capriatacursos.com.br/produto/preparatorio-banco-do-brasil/ |
| 109 | Aprovação ao Além | 43 | 1 | médio | Não confirmado | https://www.facebook.com/61579754455237/ |
| 110 | Ceisc Concursos | 43 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2316-concurso-ceisc-tribunais-tecnico-premium |
| 111 | Concursos Ceisc | 41 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2292-concurso-trt-nacional-club-analista-judiciario- |
| 112 | Verbo Jurídico | 38 | 1 | médio | Não confirmado | https://www.verbojuridico.com.br/pos-graduacoes-a-distancia-ead/pos-graduacao-em |
| 113 | Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24 | 31 | 1 | médio | R$ 297,90 | https://ataticadaaprovacao.com.br/combao/ |
| 114 | Concursos Ceisc | 30 | 1 | médio | Não confirmado | https://lp.ceisc.com.br/material-concurso-trt-4-projeto-nomeacao/ |
| 115 | Concursos Ceisc | 30 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2472-concurso-pge-rs-tecnico-administrativo-extensiv |
| 116 | Evolucional | 25 | 1 | médio | Não confirmado | https://www.facebook.com/evolucional/ |
| 117 | Perito Cibernético | 23 | 1 | médio | Não confirmado | https://www.facebook.com/peritocibernetico/ |
| 118 | Professor Fabiano Pereira | 20 | 1 | médio | Não confirmado | https://aprovatte.com.br/mentoria-start90-2025/ |
| 119 | Mapeando Concursos | 10 | 1 | médio | Não confirmado | https://www.facebook.com/100085860035210/ |
| 120 | Êutika Assessoria Empresarial | 10 | 1 | médio | Não confirmado | https://www.facebook.com/61556190747058/ |
| 121 | Malditafcc | 9 | 1 | médio | Não confirmado | https://www.facebook.com/malditafcc/ |
| 122 | flaviaholandagaeta | 9 | 1 | médio | R$ 1.997,00 | https://lousaeduca.com.br/transacao-tributaria/ |
| 123 | Hugo de Freitas | 9 | 1 | médio | Não confirmado | https://www.facebook.com/hugoconcursos/ |
| 124 | 123passei | 9 | 1 | médio | Não confirmado | https://www.facebook.com/123PasseiOficial/ |
| 125 | Carreiras Educação com Professor Jobson Castelo Branco | 9 | 1 | médio | Não confirmado | https://www.facebook.com/61572024614383/ |
| 126 | Aprovando Concurseiro | 9 | 1 | médio | R$ 57,99 | https://pay.hotmart.com/M107002055F?checkoutMode=10 |
| 127 | Uniforenses Instituto de Pericias Forenses | 8 | 1 | médio | R$ 197,00 | https://nomeacao2.uniforenses.com.br/ |
| 128 | Professor Raphael Reis | 8 | 1 | médio | R$ 450,00 | https://www.professorraphaelreis.com.br/curso/curso-de-redacao-trt-8-tecnico/ |
| 129 | Gran Cursos Online - Concursos Públicos | 8 | 1 | médio | Não confirmado | https://www.grancursosonline.com.br/cursos/por-materia/banco-do-brasil-escritura |
| 130 | Giovana reserva | 8 | 1 | médio | Não confirmado | https://www.facebook.com/61572043193487/ |

# Apêndice — Descartadas por não citarem concurso (94)

Vieram nas buscas (ex.: escritórios que citam o TRF como tribunal), mas o texto não tem nenhum termo de concurso. Confira se algo relevante caiu aqui por engano.

| Anunciante | Dias | Destino |
|---|---|---|
| Precato | 46 | http://fb.me/ |
| SERV FONE | 102 | https://www.facebook.com/servfone.servfone/ |
| Aristocrat Watch | 23 | https://www.aristocrat.com.br/products/mission-to-the-moon-1969 |
| G. Costa Advogados | 76 | http://fb.me/ |
| OC Advogados com anabeatrizzuviolloadv | 38 | https://www.facebook.com/OCAdvoga/ |
| Felipe Sgarbossa Advocacia Criminal | 169 | https://www.facebook.com/felipesgarbossa/ |
| Judit | 59 | https://produto.judit.io/miner-precatorios |
| Mercadão das Máquinas Ipatinga | 30 | https://www.facebook.com/61553303850780/ |
| Rita Bervig | 181 | https://www.facebook.com/100091834883862/ |
| Previdenciarista.com - Direito Previdenciário | 13 | https://previdenciarista.com/jurisprudencias-produto/ |
| Sindjus | 11 | https://sindjus.org/blog/ |
| Comunidade Milhorin | 9 | https://www.facebook.com/milhorincalculos/ |
| marcusf_adv | 250 | https://www.instagram.com/_u/marcus.franca.adv |
| 3 Injectors | 184 | https://apps.apple.com/us/app/3injectors-community/id6752955632 |
| Heraclio Cunha | 54 | https://peritoem7dias.com.br/ |
| Previdenciarista.com - Direito Previdenciário | 28 | https://previdenciarista.com/calculos-previdenciarios-produto/ |
| Completude Psicologia | 24 | https://www.facebook.com/61593947481286/ |
| Sindjus | 10 | https://www.facebook.com/sindjusbrasilia/ |
| TPMED - Treinamento em Perícias Médicas. | 502 | https://www.facebook.com/61556227554547/ |
| Real Dor | 251 | https://www.facebook.com/realdorbr/ |
| Alibaba.com | 199 | https://www.alibaba.com/product-detail/haoge_1601650241550.html?src=cpm_fb&sub_c |
| futstadistico | 188 | https://www.instagram.com/_u/futstadistico |
| Danielle Bartoly | 173 | https://www.facebook.com/61577922862090/ |
| Carolina Bezerra Advocacia | 159 | https://www.facebook.com/61570273217824/ |
| Editora Mizuno | 144 | https://www.editoramizuno.com.br/ |
| Dr Benedito Braga | 143 | https://www.facebook.com/BBragaJr/ |
| Douglas Prado - Servidor 30k com Servidores High Level | 127 | https://www.facebook.com/professorlucrativo/ |
| Evidencia Veículos | 109 | https://www.facebook.com/evidenciatx/ |
| 42pericias | 105 | https://www.42pericias.com.br/ |
| Duarte Advogados Associados | 104 | https://www.facebook.com/61555624388490/ |
| JQM Advocacia Especializada | 103 | https://www.facebook.com/61561436444397/ |
| Fibra Pará | 97 | https://www.facebook.com/fibrapara/ |
| pilateshiitflow com Riven Fitness for Life | 94 | https://www.instagram.com/_u/pilateshiitflow |
| Carreira de Perito | 91 | https://carreiradeperito.com.br/ |
| IBCCRIM | 86 | https://jcc.ibccrim.org.br/ |
| Efraim Vitaliano | 79 | https://www.facebook.com/61578333253215/ |
| Instituto Doutrina Policial 2 | 74 | http://fb.me/ |
| André Nelvam Advocacia | 69 | https://www.facebook.com/61564064676003/ |
| Servita Clinic | 68 | https://www.facebook.com/61582841670718/ |
| Fernandez Pollito Advocacia | 61 | https://www.facebook.com/advocaciapollito/ |
| RAIR Silva | 60 | https://www.facebook.com/jornalistarairsilva/ |
| Viégas Filho | 60 | https://www.facebook.com/100094050184913/ |
| AgroTaborda | 59 | https://www.facebook.com/Agrotaborda/ |
| thainara.assistentesocial | 58 | https://www.instagram.com/_u/thainara.assistentesocial |
| Gabriela Franco | 55 | https://www.facebook.com/61575028750782/ |
| Go Kursos | 53 | https://www.gokursos.com/go-oab---direito-penal---2%C2%AA-fase-30553/p |
| Alibaba.com | 46 | https://www.alibaba.com/product-detail/haoge_11000018246034.html?src=cpm_fb&sub_ |
| Pantheon emagrecimento | 46 | https://www.facebook.com/61567758598809/ |
| CERN - Ranieri Nogueira - Coaching & Mentoring | 42 | https://www.facebook.com/cernmentoria/ |
| Fotógrafos Cristiano e Natieli Strapazzon | 39 | https://www.facebook.com/cristianostrapazzonfotografo/ |
| Erik Navarro Wolkart | 35 | https://www.facebook.com/100070966909521/ |
| use.argos | 33 | https://useargos.com.br/ |
| Matiello Advocacia | 33 | https://www.facebook.com/matielloadvocacia/ |
| DDC - Diego Douglas Consultoria | 30 | https://www.facebook.com/61587874040061/ |
| dr_rodrigo_cerqueira | 28 | https://api.whatsapp.com/send |
| Casa dos Parafusos Franca | 27 | https://www.casadosparafusosfranca.com.br/construcao-civil/mexedores-e-triturado |
| LoyLegal | 23 | https://loytrust.com/lp/2026061/ |
| Metodo.Gafanhoto | 20 | https://metodogafanhoto.com/quizz |
| XGKE Educação | 20 | https://www.facebook.com/61591735205886/ |
| Mais Pilates | 20 | https://www.facebook.com/maispilatesrafaelchedid/ |
| Corrêa Barboza Advocacia | 19 | https://api.whatsapp.com/send |
| Prof. Pontalti | 19 | https://www.facebook.com/prof.pontalti/ |
| hobertlimoeiro | 17 | https://www.facebook.com/100065209612511/ |
| ANAJUSTRA Federal | 17 | http://fb.me/ |
| Voll Studios Recomeçar Sudoeste | 16 | https://www.facebook.com/vollstudiosrecomecar/ |
| Precs.oficial | 16 | https://precs.com.br/central-do-credor/ |
| Casarolli Advogados Prev | 16 | https://www.facebook.com/advluiscasarolli/ |
| RevPrev | 14 | https://api.whatsapp.com/send |
| Alison Jesus Advogados | 14 | https://www.facebook.com/100063574359361/ |
| O Primeiro Parecer | 13 | https://web.trf3.jus.br/noticias/Noticiar/ExibirNoticia/446820-inss-deve-indeniz |
| Mindjus Criminal com Saliba Adv | 11 | https://www.facebook.com/100062961173630/ |
| Martins Coelho Advogados | 11 | https://livredoir.com.br/ |
| Laura Da Silva | 11 | https://www.facebook.com/61561327270523/ |
| Monica Freitas MTE | 10 | https://www.facebook.com/61583807948841/ |
| Dr. Endrigo Piva Pontelli | 10 | https://www.facebook.com/61550186032145/ |
| Bornholdt Advogados | 10 | https://www.facebook.com/BornholdtAdvogados/ |
| Gracielle Lima Assessoria e Consultoria Jurídica | 10 | https://www.facebook.com/61585454075287/ |
| Tapai Advogados | 10 | https://www.facebook.com/TapaiAdvogados/ |
| Giselle Tapai | 10 | https://www.facebook.com/61588752251791/ |
| brenomarxoficial | 10 | https://www.facebook.com/100081178312118/ |
| mhwerneck.adv | 10 | https://www.instagram.com/_u/mhwerneck.adv |
| Sindjus | 10 | https://www.youtube.com/watch?v=ZZeBsAEAbUA |
| Digital Reach | 10 | https://recebabrasil.com.br/recebimentos-judiciais |
| Coagro | 10 | https://www.facebook.com/GrupoCoagro/ |
| ResuNinja | 10 | https://www.resuninja.com/bonus |
| JUSINTEGRA | 10 | https://www.facebook.com/jusintegra/ |
| Daniella Costa Agro | 9 | https://www.facebook.com/61594331413710/ |
| samwelholandaadv | 9 | https://www.instagram.com/_u/samwelholandaadv |
| BSSP Centro Educacional | 9 | https://bsspce.com.br/pos-graduacao-e-mba/mba-pericia-contabil-economica-e-finan |
| Dr. Elpídio Donizetti | 9 | https://elpidiodonizetti.com.br/ |
| achaaguaperfuracoes | 9 | https://www.facebook.com/100070641083310/ |
| Correa Advocacia | 9 | https://www.facebook.com/61574806646142/ |
| Hidromaq Irrigação e Máquinas Agrícolas | 9 | https://www.facebook.com/61573307953422/ |
| Antecipeprecatoriosbr | 8 | https://www.facebook.com/61579343185492/ |
