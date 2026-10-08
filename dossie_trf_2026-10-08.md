# Dossiê ConcursoRadar — Técnico Judiciário — TRF (08/10/2026)

## Métricas da Rodada
- **Buscas na Meta Ad Library:** `concurso TRF`, `tribunal regional federal`, `técnico judiciário`, `técnico judiciário área administrativa`, `TRF1`, `TRF2`, `TRF3`, `TRF4`, `TRF5`, `TRF6`, `concurso tribunal`
- **Filtro:** anúncios ativos no Brasil, no ar há 7+ dias (coleta ampla para achar padrões; a longevidade é analisada nas tabelas)
- **Ofertas do nicho:** 77 (de 164 anúncios; agrupadas por anunciante + página de destino)
- **Descartadas por não citarem concurso:** 50 (listadas no fim para auditoria)
- **Ofertas de foco direto:** 27 | adjacentes: 50
- **Sinal de tração:** 3 forte, 2 fraco, 72 médio
- **Landing pages lidas:** 55 de 77
- **Ticket confirmado no checkout:** 7 de 7 ofertas com checkout detectado (100%)
- **Tempo de processamento:** 613 segundos

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

Base: **164 anúncios de 55 anunciantes**; 37 estão no ar há 45+ dias (veteranos); mediana de 13 dias.

Como ler: **Anunciantes** = quantos produtores distintos usam (popularidade). **Veteranos** = quantos desses anúncios estão no ar há 45+ dias, e **% dos veteranos** = a fatia da categoria entre todos os veteranos. Se a fatia entre veteranos é maior que a fatia geral (% anúncios), a categoria aparece mais entre os que duram. Categoria com 1 ou 2 anunciantes é só um caso isolado.

A coleta junta duas amostras por busca (anúncios com 7+ dias e anúncios com 45+ dias), então a proporção de veteranos no total não é uma taxa de sobrevivência.

## Formato do criativo

Vídeo, imagem única ou carrossel.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| imagem | 25 | 45% | 98 | 60% | 10 | 20 | 54% |
| vídeo | 23 | 42% | 38 | 23% | 12 | 7 | 19% |
| carrossel | 20 | 36% | 28 | 17% | 28 | 10 | 27% |

## Proporção do criativo

Vertical (4:5 ou 9:16), quadrada (1:1) ou horizontal.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| vídeo vertical | 23 | 42% | 38 | 23% | 12 | 7 | 19% |
| imagem vertical | 21 | 38% | 72 | 44% | 10 | 10 | 27% |
| carrossel vertical | 15 | 27% | 19 | 12% | 28 | 7 | 19% |
| imagem quadrada | 7 | 13% | 26 | 16% | 33 | 10 | 27% |
| carrossel quadrada | 7 | 13% | 9 | 5% | 28 | 3 | 8% |

## Duração dos vídeos

Só anúncios em vídeo.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| 1 a 2min | 9 | 39% | 12 | 32% | 10 | 3 | 43% |
| 31s a 1min | 8 | 35% | 17 | 45% | 14 | 1 | 14% |
| Mais de 2min | 4 | 17% | 4 | 11% | 18 | 1 | 14% |
| Até 30s | 2 | 9% | 5 | 13% | 10 | 2 | 29% |

## Botão (CTA)

Rótulo do botão exibido no anúncio.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| sem botão | 27 | 49% | 57 | 35% | 10 | 9 | 24% |
| Saiba mais | 22 | 40% | 59 | 36% | 13 | 15 | 41% |
| Visitar perfil do Instagram | 10 | 18% | 12 | 7% | 35 | 5 | 14% |
| Ver detalhes | 8 | 15% | 24 | 15% | 13 | 5 | 14% |
| Enviar mensagem pelo WhatsApp | 2 | 4% | 6 | 4% | 10 | 0 | 0% |
| Comprar agora | 1 | 2% | 2 | 1% | 36 | 1 | 3% |
| Cadastre-se | 1 | 2% | 2 | 1% | 85 | 2 | 5% |
| Enviar mensagem | 1 | 2% | 1 | 1% | 13 | 0 | 0% |
| Fale conosco | 1 | 2% | 1 | 1% | 8 | 0 | 0% |

## Destino do clique

Para onde o anúncio leva.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Página própria (LP / site) | 37 | 67% | 123 | 75% | 10 | 25 | 68% |
| Página / formulário no Facebook | 21 | 38% | 37 | 23% | 22 | 12 | 32% |
| Checkout direto | 1 | 2% | 4 | 2% | 12 | 0 | 0% |

## Tamanho da copy

Texto principal do anúncio.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Média (200 a 600) | 32 | 58% | 95 | 58% | 16 | 25 | 68% |
| Longa (mais de 600) | 26 | 47% | 56 | 34% | 10 | 11 | 30% |
| Curta (até 200 caracteres) | 6 | 11% | 13 | 8% | 17 | 1 | 3% |

## Tipo de gancho (1ª linha da copy)

Classificação por palavras-chave; um gancho pode cair em mais de um tipo.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos | Exemplo |
|---|---|---|---|---|---|---|---|---|
| Outro | 26 | 47% | 53 | 32% | 30 | 23 | 62% | Três ferramentas. Um mesmo objetivo: transformar o seu estudo em aprovação. 🎯 — Decorando a Lei Seca Cursos Para Concursos E OAB |
| Notícia de concurso / edital | 18 | 33% | 56 | 34% | 9 | 3 | 8% | Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova? — MEQ Concursos |
| Chamada direta ao público | 11 | 20% | 14 | 9% | 16 | 4 | 11% | 🚨 Atenção: foi autorizado um novo concurso do Tribunal de Justiça de GO! — Professor Fabiano Pereira |
| Pergunta | 10 | 18% | 24 | 15% | 9 | 5 | 14% | Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova? — MEQ Concursos |
| Número / lista | 10 | 18% | 19 | 12% | 9 | 0 | 0% | 🚨 10% OFF / Projeto TRF3 2026 – Técnico e Analista — NEAF Concursos Públicos |
| Salário / estabilidade | 7 | 13% | 16 | 10% | 9 | 3 | 8% | ⚖️ O TJ-SP já iniciou os estudos para um próximo concurso, com salários que passam de R$6.000,00. — Monica Freitas MTE |
| Dor / erro do candidato | 6 | 11% | 17 | 10% | 8 | 0 | 0% | Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova? — MEQ Concursos |
| Oferta / desconto / urgência | 6 | 11% | 6 | 4% | 32 | 2 | 5% | 🚨 10% OFF / Projeto TRF3 2026 – Técnico e Analista — NEAF Concursos Públicos |
| Prova social / autoridade | 4 | 7% | 6 | 4% | 29 | 0 | 0% | Estar preparado para ser aprovado em um cargo de Técnico em Tribunal exige um curso completo e focado no que realmente vai cair nas provas. — Ceisc Concursos |
| Contraintuitivo / inimigo comum | 3 | 5% | 3 | 2% | 13 | 0 | 0% | Três anos no cursinho jurídico. Sete apostilões de Direito. E fiquei em cadastro de reserva no primeiro TRT que eu prestei. — Gustavo Nogueira - Aprovação Ágil |
| Promessa de método | 3 | 5% | 3 | 2% | 43 | 1 | 3% | Estude com método! — Concursos Ceisc |

## Elementos da copy

Recursos presentes no texto; não são excludentes.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Usa emojis | 33 | 60% | 86 | 52% | 13 | 24 | 65% |
| Cita valor em R$ | 17 | 31% | 47 | 29% | 9 | 6 | 16% |
| Hashtags | 15 | 27% | 23 | 14% | 14 | 3 | 8% |
| Lista com marcadores (✔, ✅, •) | 13 | 24% | 21 | 13% | 28 | 7 | 19% |
| Link ou 'link na bio' no texto | 7 | 13% | 7 | 4% | 10 | 0 | 0% |
| Gancho em CAIXA ALTA | 5 | 9% | 13 | 8% | 8 | 3 | 8% |
| Cita garantia | 3 | 5% | 3 | 2% | 13 | 0 | 0% |
| Cita bônus | 2 | 4% | 4 | 2% | 56 | 2 | 5% |

## Sinais de público (ICP) citados na copy

Quem o anúncio diz atender, por palavras-chave. Indica a quem o mercado fala, não quem compra.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos | Exemplo |
|---|---|---|---|---|---|---|---|---|
| Motivado por salário / estabilidade | 18 | 33% | 50 | 30% | 9 | 7 | 19% | 📌 Salário inicial de aproximadamente R$ 14.000,00; — Professor Fabiano Pereira |
| Esquece o que estuda / revisão | 12 | 22% | 28 | 17% | 10 | 8 | 22% | Você não precisa apenas ler mais a lei seca. Precisa saber o que memorizar, como revisar e onde concentrar seus esforços. — Decorando a Lei Seca Cursos Para Concursos E OAB |
| Dificuldade em discursiva / redação | 9 | 16% | 25 | 15% | 8 | 4 | 11% | Não para estudar mais um pouco. Para sentar, encarar 60 questões seguidas, matérias misturadas, discursiva e o relógio correndo. — MEQ Concursos |
| Pré-edital / sair na frente | 9 | 16% | 24 | 15% | 16 | 4 | 11% | 🚨 Atenção: foi autorizado um novo concurso do Tribunal de Justiça de GO! — Professor Fabiano Pereira |
| Estuda há tempo e não passa | 6 | 11% | 8 | 5% | 10 | 2 | 5% | Você estuda, se prepara, domina o conteúdo… mas ainda trava na hora da redação? 📝 — Professor Hansk |
| Reta final / pós-edital | 5 | 9% | 5 | 3% | 30 | 2 | 5% | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. — Tjteiros |
| Nível médio | 3 | 5% | 12 | 7% | 9 | 0 | 0% | Observação: o requisito de formação é nível médio, ou seja, qualquer pessoa com ensino médio concluído pode participar. — Pratique Concursos |
| Começando do zero | 3 | 5% | 3 | 2% | 65 | 3 | 8% | No Experiência Carreiras, você conhece na prática como funcionam as principais carreiras públicas, acessa aulas reais dos cursos Ceisc, materiais em PDF e conte — Concursos Ceisc |
| Perdido no excesso de conteúdo | 3 | 5% | 3 | 2% | 65 | 2 | 5% | Garanta seu acesso e descubra por onde começar. — Concursos Ceisc |
| Trabalha / tem pouco tempo | 2 | 4% | 3 | 2% | 42 | 0 | 0% | ✅ Metas adaptadas à sua rotina — Monica Freitas MTE |
| Erra questões / pegadinhas da banca | 2 | 4% | 3 | 2% | 13 | 1 | 3% | E é justamente nessa diferença que as bancas constroem a pegadinha. — Decorando a Lei Seca Cursos Para Concursos E OAB |
| Nível superior / Direito | 1 | 2% | 2 | 1% | 98 | 2 | 5% | Nível superior: Direito — Concursos Ceisc |

## Tipo de produto × ticket

Tipo identificado por palavras-chave na copy, no título do link e na headline (uma oferta pode ter vários). Ticket só entra quando foi lido no checkout.

| Tipo de produto | Anunciantes | Ofertas | Veteranas | Com ticket lido | Mínimo | Mediana | Máximo | Tickets lidos |
|---|---|---|---|---|---|---|---|---|
| Material em PDF / apostila / caderno | 33 | 35 | 14 | 2 | R$ 497 | R$ 498 | R$ 500 | Caderno do Aprovado - Materiais para Concursos R$ 497; Decorando a Lei Seca Cursos para Concursos LTDA R$ 500 |
| Questões / simulados | 17 | 20 | 6 | 2 | R$ 500 | R$ 500 | R$ 500 | Decorando a Lei Seca Cursos Para Concursos E OAB R$ 500; Decorando a Lei Seca Cursos para Concursos LTDA R$ 500 |
| Curso em videoaulas | 14 | 28 | 12 | 2 | R$ 500 | R$ 714 | R$ 928 | Decorando a Lei Seca Cursos Para Concursos E OAB R$ 500; Decorando a Lei Seca Cursos Para Concursos E OAB R$ 928 |
| Isca gratuita / grupo VIP | 13 | 15 | 5 | 1 | R$ 298 | R$ 298 | R$ 298 | Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24 R$ 298 |
| Cronograma / plano de estudos | 9 | 10 | 3 | 1 | R$ 500 | R$ 500 | R$ 500 | Decorando a Lei Seca Cursos para Concursos LTDA R$ 500 |
| Lei seca / legislação | 8 | 10 | 5 | 5 | R$ 377 | R$ 500 | R$ 928 | Legislação Integrada R$ 377; Caderno do Aprovado - Materiais para Concursos R$ 497; Decorando a Lei Seca Cursos Para Concursos E OAB R$ 500; Decorando a Lei Seca Cursos para Concursos LTDA R$ 500; Decorando a Lei Seca Cursos Para Concursos E OAB R$ 928 |
| Discursiva / redação | 8 | 9 | 2 | 0 | — | — | — |  |
| Mentoria / acompanhamento | 7 | 7 | 1 | 0 | — | — | — |  |
| Não identificado | 6 | 6 | 1 | 0 | — | — | — |  |
| Assinatura / clube / vitalício | 5 | 6 | 0 | 6 | R$ 97 | R$ 438 | R$ 928 | Pensar-Concursos R$ 97; Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24 R$ 298; Legislação Integrada R$ 377; Decorando a Lei Seca Cursos Para Concursos E OAB R$ 500; Decorando a Lei Seca Cursos para Concursos LTDA R$ 500; Decorando a Lei Seca Cursos Para Concursos E OAB R$ 928 |
| Mapas mentais / esquemas | 5 | 5 | 1 | 3 | R$ 497 | R$ 500 | R$ 500 | Caderno do Aprovado - Materiais para Concursos R$ 497; Decorando a Lei Seca Cursos Para Concursos E OAB R$ 500; Decorando a Lei Seca Cursos para Concursos LTDA R$ 500 |
| Flashcards | 1 | 1 | 1 | 0 | — | — | — |  |

## Expressões repetidas entre anunciantes

Sequências de 2 ou 3 palavras (sem acento) usadas na copy por 3 ou mais anunciantes distintos.

`clique em saiba` (10), `tribunal regional` (7), `concursos publicos` (6), `tribunal regional federal` (5), `tecnico judiciario` (5), `publicacao do edital` (5), `novo concurso` (5), `link da bio` (5), `garanta sua vaga` (5), `concurso publico` (5), `concurso do tribunal` (5), `alto nivel` (5), `ultimo concurso` (4), `tribunal de contas` (4), `toque em saiba` (4), `salario inicial` (4), `realmente cai` (4), `quem quer` (4), `quem comeca` (4), `ministerio publico` (4), `mapas mentais` (4), `lei seca` (4), `concurso do trt` (4), `analista judiciario` (4), `tribunal de justica` (3), `see details` (3), `remuneracao inicial` (3), `r$ 16` (3), `r$ 11` (3), `quer estudar` (3)

## Arquivo de ganchos (anúncios mais replicados e mais antigos)

| Anunciante | Dias | Cópias | Formato | Botão | Gancho (1ª linha) | Título do link |
|---|---|---|---|---|---|---|
| MEQ Concursos | 8 | 13 | imagem | sem botão | Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova? |  |
| Decorando a Lei Seca Cursos Para Concursos E OAB | 10 | 6 | imagem | sem botão | Três ferramentas. Um mesmo objetivo: transformar o seu estudo em aprovação. 🎯 |  |
| Professor Fabiano Pereira | 17 | 3 | vídeo | sem botão | 🚨 Atenção: foi autorizado um novo concurso do Tribunal de Justiça de GO! |  |
| Metodo.Gafanhoto | 9 | 3 | vídeo | sem botão | INDICAÇÃO CONCURSO PARA MULHERES QUE NÃO TEM BASE NOS ESTUDOS |  |
| Professor Hansk | 9 (baixo volume) | 3 | vídeo | sem botão | Você estuda, se prepara, domina o conteúdo… mas ainda trava na hora da redação? 📝 |  |
| Monica Freitas MTE | 8 | 3 | imagem | sem botão | ⚖️ O próximo concurso do TRF da 3ª Região pode ser uma grande oportunidade para quem quer conquistar uma vaga no serviço público. |  |
| Monica Freitas MTE | 8 | 3 | imagem | sem botão | ⚖️ O TJ-SP já iniciou os estudos para um próximo concurso, com salários que passam de R$6.000,00. |  |
| Monica Freitas MTE | 8 | 3 | imagem | sem botão | ⚖️ O TRF da 3ª Região já iniciou os estudos para um próximo concurso, com salários que podem começar em torno de R$ 10 mil para técnico e R$ 16 mil para analista. |  |
| Gustavo Nogueira - Aprovação Ágil | 8 | 3 | vídeo | sem botão | Três anos no cursinho jurídico. Sete apostilões de Direito. E fiquei em cadastro de reserva no primeiro TRT que eu prestei. |  |
| Tjteiros | 97 | 2 | vídeo | sem botão | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. |  |
| G7 Jurídico | 49 (baixo volume) | 2 | imagem | sem botão | ADI sobre o regime remuneratório da magistratura, novo entendimento sobre taxas estaduais, marco legal do crime organizado, mudanças na legislação eleitoral. Em poucos meses, o STF redesenhou o cenário e o Legislativo en |  |
| NEAF Concursos Públicos | 14 | 2 | vídeo | sem botão | 🚨 10% OFF / Projeto TRF3 2026 – Técnico e Analista |  |
| NEAF Concursos Públicos com tjserei | 14 | 2 | vídeo | sem botão | VOCÊ AINDA NÃO COMEÇOU A ESTUDAR / Técnico e Analista do TRF3? |  |
| Advogado de concurso | 10 | 2 | vídeo | sem botão | 🚨 Fez a prova discursiva do TCE-RS? |  |
| Prof. Ronaldo Santos | 8 | 2 | imagem | sem botão | A Ana Flávia chegou até mim faltando apenas 15 dias para o concurso do Tribunal de Justiça do Rio de Janeiro. |  |
| Decorando a Lei Seca Cursos Para Concursos E OAB | 921 | 1 | vídeo | sem botão | Lançados em março de 2024 |  |
| Caderno do Aprovado - Materiais para Concursos | 616 | 1 | vídeo | sem botão | Lançados em janeiro de 2025 |  |
| Concursos Ceisc | 211 | 1 | imagem | Saiba mais | Lançados em março de 2026 |  |
| Decorando a Lei Seca Cursos Para Concursos E OAB | 186 | 1 | carrossel | Visitar perfil do Instagram | Lançados em abril de 2026 |  |
| euvoupassei com Aprovação PGE | 181 | 1 | carrossel | Saiba mais | Quem disse que só passa quem tem tempo? Sabendo organizar seu tempo de estudo, seja ele qual for, e com um bom material, a aprovação vem ✨ |  |
| Ceisc Concursos | 178 | 1 | imagem | Saiba mais | Muitas pessoas conquistam estabilidade e crescimento profissional por meio dos concursos públicos. |  |
| Decorando a Lei Seca Cursos Para Concursos E OAB | 169 | 1 | carrossel | Visitar perfil do Instagram | O art. 15 do Código Penal voltou a aparecer em prova — dessa vez pela CEBRASPE, no TCE-MG de 2026. |  |
| Ceisc Concursos | 147 | 1 | imagem | Ver detalhes | Lançados em maio de 2026 | Equipe de Especialistas |
| Concursos Ceisc | 134 | 1 | imagem | Ver detalhes | Seu cargo como magistrado pode estar mais próximo. E cada dia importa nessa fase decisiva. | Aprove com Especialistas |
| Concursos Ceisc | 98 | 1 | imagem | Saiba mais | O TRF-3 é uma das grandes oportunidades para quem busca uma carreira na área jurídica! |  |
| Concursos Ceisc | 98 | 1 | imagem | Saiba mais | Quem se prepara antes, chega mais longe! | TRF-3 / Analista Judiciário |
| MEQ Concursos | 89 | 1 | carrossel | Visitar perfil do Instagram | Lançados em julho de 2026 |  |
| Concursos Ceisc | 85 | 1 | imagem | Cadastre-se | Quer estar por dentro dos principais concursos? Nosso curso GRATUITO é ideal para você! | Sua Aprovação Começa Aqui |
| Concursos Ceisc | 85 | 1 | imagem | Cadastre-se | Começar a estudar para concursos com direcionamento certo faz toda a diferença. | Sua Aprovação Começa Aqui |
| Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24 | 83 | 1 | carrossel | Saiba mais | COMBO AUDITOR FISCAL / 39.988 FLASHCARDS | COMBO AUDITOR FISCAL |
| Concursos Ceisc | 78 | 1 | imagem | Saiba mais | Estude com método! |  |
| Concursosmeucurso | 78 | 1 | carrossel | Saiba mais | TRF3, TJSP e TSE/TREs estão entre os concursos mais aguardados do momento, com centenas de cargos previstos e remuneração inicial que pode ultrapassar R$ 18 mil. | Concursos com remuneração de até R$ 18 mil |
| Concursos Ceisc | 77 | 1 | imagem | Ver detalhes | Estudar com direcionamento te poupa tempo e energia. | TRF-3 / Analista Judiciário |
| Concursos Ceisc | 77 | 1 | imagem | sem botão | Uma preparação eficiente para ingressar nos tirbunais exige planejamento, prática e acompanhamento ao longo da jornada. |  |
| Concursos Ceisc | 77 | 1 | imagem | Ver detalhes | A diferença para sua aprovação no TRF-3 pode estar em como você vai se preparar. | TRF-3 / Analista Judiciário |
| Gazeta dos Concursos | 76 | 1 | vídeo | Saiba mais | Qual o melhor concurso de tribunal pra você começar hoje? | Melhor tribunal pra começar hoje |
| Gazeta dos Concursos | 76 | 1 | vídeo | Saiba mais | Qual concurso te bota mais rápido em R$11.500 iniciais com qualquer graduação — inclusive tecnólogo? | O caminho mais rápido pra R$11.500 |
| Atleta dos Concursos - OAB | 76 | 1 | vídeo | sem botão | Eu acredito que eu posso te ajudar. Por quê? |  |
| Caderno do Aprovado - Materiais para Concursos | 65 | 1 | imagem | Ver detalhes | 🚨 O edital do TRF-3 pode sair a qualquer momento! | Combos TRF, TJ e MP – Caderno do Aprovado – Caderno do Aprovado – Materiais de estudos para concursos públicos |
| Concursos Ceisc | 57 | 1 | imagem | Comprar agora | Para conquistar essa nova oportunidade, você precisa se preparar com organização. |  |

---

# Parte 1 — Ofertas de foco direto (27)

---
id_oferta: 001
anunciante: "MEQ Concursos"
url_destino: "https://meqconcursos.com.br/concurso-simulado-meq-2-analista-trt-v2-l/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2566762267130059"
dias_ativo: 9
anuncios_coletados: 12
anuncios_ativos_estimados: 32
anuncios_com_baixo_volume_de_impressoes: 3
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados, Discursiva / redação, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (5), imagem (7)"
botoes: "sem botão (9), Ver detalhes (2), Saiba mais (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"<100
Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova?
Não para estudar mais um pouco. Para sentar, encarar 60 questões seguidas, matérias misturadas, discursiva e o relógio correndo.
É isso que o 2º Concurso Simulado MEQ vai te mostrar, antes que a prova de verdade chegue.
📝 Prova completa no padrão FCC� ⏱️ Tempo cronometrado, correção individual e ranking� 🎯 Para Analista Judiciário (Área Judiciária) e Técnico Judiciário (Área Administrativa)� 💸 100% gratuito
📅 Prova online em 10/10 | Inscrições até 08/10
Clique em "Saiba mais" e garanta sua vaga."

### Ganchos das variações (1ª linha de cada anúncio)
- Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova?
- <100

### Títulos do link nos anúncios
- Clique no botão abaixo e garanta sua vaga.

### Landing Page: Headline & Promessa Central
"Concurso Simulado MEQ 2 – Analista TRT – V2 (L) – MEQ Concursos — Enquanto os editais oficiais não saem, você se prepara simulando condições reais de prova"

### Seções da Landing Page (títulos, na ordem)
- Enquanto os editais oficiais não saem, você se prepara simulando condições reais de prova
- Como o Concurso Simulado funciona
- Prova Objetiva — 60 questões:
- Prova discursiva:
- Cronograma do Concurso
- E os melhores colocados de cada cargo ganham prêmios de verdade
- Perguntas frequentes
- Ainda tem dúvidas?
- Faça sua inscrição gratuita
- Inscrição confirmada!

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Discursiva / redação
- PDF
- Simulados


========================================

---
id_oferta: 002
anunciante: "Portal & OAB"
url_destino: "https://olympus.cursosdoportal.com.br/o-adm-trt-pa/?utm_source=%7B%7Bsite_source_name%7D%7D&utm_medium=%7B%7Badset.name%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D&utm_term=%7B%7Bplacement%7D%7D&utm_content=%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1074976398625545"
dias_ativo: 10
anuncios_coletados: 11
anuncios_ativos_estimados: 11
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados, Cronograma / plano de estudos, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (8), vídeo (3)"
botoes: "sem botão (8), Ver detalhes (3)"
precos_exibidos_na_lp: "R$ 9.776,71 | R$ 16.040,88"
primeira_coleta_propria: "2026-10-07"
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
id_oferta: 003
anunciante: "Portal Concursos"
url_destino: "https://oportalconcursos.com.br/h-adm-trt-mt/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1436015981795868"
dias_ativo: 8
anuncios_coletados: 10
anuncios_ativos_estimados: 10
anuncios_com_baixo_volume_de_impressoes: 2
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (10)"
botoes: "Saiba mais (10)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
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
id_oferta: 004
anunciante: "Monica Freitas MTE"
url_destino: "https://form.respondi.app/yLeg4HU6"
ad_library_url: "https://www.facebook.com/ads/library/?id=2170313573699395"
dias_ativo: 8
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
dias_distintos_coletado: 1
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
id_oferta: 005
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2549-concurso-trf-3-analista-judiciario-area-judiciaria"
ad_library_url: "https://www.facebook.com/ads/library/?id=1355671819846214"
dias_ativo: 98
anuncios_coletados: 6
anuncios_ativos_estimados: 6
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trf, trf 3"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "imagem (6)"
botoes: "Ver detalhes (2), Saiba mais (3), sem botão (1)"
precos_exibidos_na_lp: "R$ 16.040,85 | R$ 10 | R$ 1.199,00 | R$ 769,30 | 12x de R$ 64,11"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
- Quem se prepara antes, chega mais longe!
- A diferença para sua aprovação no TRF-3 pode estar em como você vai se preparar.

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
id_oferta: 006
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://www.facebook.com/simboraconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=9045055822237560"
dias_ativo: 616
anuncios_coletados: 5
anuncios_ativos_estimados: 5
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trf, tribunal regional federal, trf3"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Questões / simulados, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (4), carrossel (1)"
botoes: "sem botão (4), Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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

### Títulos do link nos anúncios
- Beto (José Humberto) - Caderno Do Aprovado - TRT/TST/TJ/MP (@cadernoaprovado) • Instagram photos and videos

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 007
anunciante: "Tjteiros"
url_destino: "https://www.facebook.com/61582438800580/"
ad_library_url: "https://www.facebook.com/ads/library/?id=4654373284799285"
dias_ativo: 97
anuncios_coletados: 1
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf3"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "vídeo (1)"
botoes: "sem botão (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
id_oferta: 008
anunciante: "JusConc"
url_destino: "https://www.facebook.com/61555120221977/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1070081985496959"
dias_ativo: 54
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
dias_distintos_coletado: 2
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
id_oferta: 009
anunciante: "Pratique Concursos"
url_destino: "https://ti.pratiqueconcursos.com.br/fcti/main.html"
ad_library_url: "https://www.facebook.com/ads/library/?id=999076996486447"
dias_ativo: 28
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 1
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
dias_distintos_coletado: 2
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
- <100

### Títulos do link nos anúncios
- Super Resumos para Concurso TRT
- Super Resumo - Banco do Brasil

### Landing Page: Headline & Promessa Central
"Aumente suas chances de aprovação nos concursos de TI — Pesquise por concurso, curso ou assunto."

### Seções da Landing Page (títulos, na ordem)
- Nenhum material encontrado
- FCTI - Formação Concursado de TI
- Guia para Concursos (GRÁTIS)
- DATAPREV
- Transpetro
- Super Intensivo SEFAZ SP
- Super Intensivo CGU Pré-Edital
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
id_oferta: 010
anunciante: "NEAF Concursos Públicos"
url_destino: "https://neaf.com.br/trf-3/?utm_source=meta&utm_medium=ads&utm_campaign=lp-trf3-meta-impulsionamento-zini-tr3"
ad_library_url: "https://www.facebook.com/ads/library/?id=1404673661105041"
dias_ativo: 14
anuncios_coletados: 1
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf, trf3, trf 3, tjaa"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Questões / simulados, Cronograma / plano de estudos"
formatos_dos_anuncios: "vídeo (1)"
botoes: "sem botão (1)"
precos_exibidos_na_lp: "R$ 9.776,71 | R$ 16.040,88"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 10% OFF | Projeto TRF3 2026 – Técnico e Analista
A preparação mais completa para quem quer garantir a colocação no concurso do TRF3! ⚖️📚
🔥 O que você vai ter acesso:
✔️ Curso Teórico completo
→ Técnico: ~260h
→ Analista: ~280h
✔️ + de 1100 questões no total para cada cargo (curso teoria e questões + curso de testes)
✔️ Simulado online completo
✔️ Roteiro de estudos para manter constância e evolução
💡 Um projeto pensado do início ao pós-edital, guiando você até a aprovação.
🚀 Garanta seu desconto agora — link na bio!
.
.
#TRF3 #TRF32026 #ConcursoTRF3 #Vunesp #analistaTRF3 #técnicoTRF3 #SouNEAF"

### Landing Page: Headline & Promessa Central
"Como estudar para o concurso do TRF3 sem perder tempo? — A Preparação Definitiva para garantir sua aprovação no Concurso TRF3 como Técnico Administrativo (TJAA) ou Analista Judiciário (AJAJ)."

### Seções da Landing Page (títulos, na ordem)
- Manual Estratégico — TRF3
- Preencha para receber seu material gratuito
- Por que o TRF-3 merece sua atenção?
- Remuneração atrativa
- Carreira federal estável
- Ótimas oportunidades de nomeação
- Lotações em SP e MS
- Possibilidade de teletrabalho
- Crescimento na carreira
- O Projeto TRF-3 NEAF
- Produtos planejados para sua aprovação
- Curso Teórico
- Curso de Questões
- Preparação Discursiva
- Simulados
- Professores especialistas em concursos de Tribunais
- NEAF : tradição, resultados e confiança
- Dúvidas frequentes
- Comece agora sua preparação para o TRF-3.

### Entregáveis / Formato (termos encontrados na LP)
- Discursiva / redação
- Mapas mentais
- PDF
- Questões comentadas
- Resumos
- Simulados


========================================

---
id_oferta: 011
anunciante: "NEAF Concursos Públicos com tjserei"
url_destino: "https://www.neafconcursos.com.br/produtos/category/trf-3_68/?utm_source=meta&utm_medium=ads&utm_campaign=lp-trf3-meta-impulsionamento-zini-tr3"
ad_library_url: "https://www.facebook.com/ads/library/?id=1403230601407102"
dias_ativo: 14
anuncios_coletados: 1
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf, tribunal regional federal, trf3, trf 3"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "vídeo (1)"
botoes: "sem botão (1)"
precos_exibidos_na_lp: "R$ 1.289,00 | R$ 1.017,29 | R$ 960,40"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"VOCÊ AINDA NÃO COMEÇOU A ESTUDAR | Técnico e Analista do TRF3?
Com as notícias recentes de prorrogação do concurso do TRF3, muita gente relaxou e deixou esse concurso para depois, mas como o prof. Alessandro Ferraz já explicou antes, esse concurso está muito mais próximo do que você imagina! E o conteúdo do edital é bem extenso e precisa de muito tempo de estudo!
Neste vídeo, te mostramos a melhor ordem e forma de começar a estudar para o Concurso do Tribunal Regional Federal!
💡 PASSOU DA HORA de começar sua preparação com qualidade para o TRF3! 🚀
.
.
#salárioTRF3 #PRORROGAÇÃO #ConcursoTRF3 #TRF3 #TRF #AnalistaTRF3 #TécnicoTRF3"

### Landing Page: Headline & Promessa Central
"Curso para Concurso do TRF 3 Online | NEAF — Por que escolher o NEAF Concursos?"

### Seções da Landing Page (títulos, na ordem)
- Por que escolher o NEAF Concursos?
- Qualidade comprovada
- Resultados consistentes
- Tradição e credibilidade

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 012
anunciante: "Hugo de Freitas"
url_destino: "https://www.facebook.com/hugoconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1567356078474323"
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
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "carrossel (2)"
botoes: "Visitar perfil do Instagram (1), sem botão (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O TJ-SP quase nunca avisa antes. Dessa vez, avisou. 👀
Em agosto, o próprio tribunal confirmou que estuda novos concursos de Escrevente Técnico Judiciário (2ª a 10ª RAJ) e de Oficial de Justiça (todo o estado). A Vunesp já tem contrato ativo até junho de 2027, e os cadastros atuais do interior vencem entre 11 e 24 de junho de 2027.
Resumindo: o edital ainda não saiu, mas a preparação precisa começar agora. Ensino médio, R$ 6.043,54 iniciais e 40h semanais.
Quer estudar exatamente o que a Vunesp cobra há 20 anos? Comenta TJ que eu te mando o link do Protocolo TJSP no direct. 📩
#concursotjsp #tjsp #escreventetjsp #escreventetecnicojudiciario #oficialdejustica #vunesp #concursopublico #concurseiro #concursos2026 #concursos2027 #ensinomedio #hugoconcursos"

### Ganchos das variações (1ª linha de cada anúncio)
- O TJ-SP quase nunca avisa antes. Dessa vez, avisou. 👀
- Concurso TJ SP de Escrevente pode sair em breve.

### Títulos do link nos anúncios
- Hugo de Freitas | Concurso Público (@hugoconcursos) • Instagram photos and videos

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 013
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/categorias/concursos?subcategorie=trf-1-magis&utm_source=facebook&utm_medium=cpc&utm_campaign=vendas_trf_1_juiz_federal"
ad_library_url: "https://www.facebook.com/ads/library/?id=888699670925217"
dias_ativo: 134
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
precos_exibidos_na_lp: "R$ 599,00 | R$ 419,30 | 12x de R$ 34,94 | R$ 377,37 | R$ 1.797,00 | R$ 1.078,20 | 12x de R$ 89,85 | R$ 970,38"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
"Confira nossos cursos preparatórios de Concursos e fique um passo mais perto de conquistar o seu sonho."

### Seções da Landing Page (títulos, na ordem)
- Cursos de Concursos
- Confira nossos cursos preparatórios de Concursos e fique um passo mais perto de conquistar o seu sonho.

### Entregáveis / Formato (termos encontrados na LP)
- Mentoria


========================================

---
id_oferta: 014
anunciante: "Concursosmeucurso"
url_destino: "https://meucurso.com.br/cursos/concursos-publicos"
ad_library_url: "https://www.facebook.com/ads/library/?id=1542521100851019"
dias_ativo: 78
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
precos_exibidos_na_lp: "R$ 350 | R$ 699,00 | 12x de R$ 29,08 | R$ 349,00 | 12x de R$ 40,78 | R$ 489,30 | R$ 999,00 | 12x de R$ 66,58"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
- Exigência de depósito prévio para internação emergencial é ilegal: análise do caso no TJSP
- Consumo de álcool no intervalo intrajornada e a justa causa: caso do frentista no TRT-18
- Procuradorias FCC | Resolução de Questões - online
- Procuradoria do Estado de São Paulo | Peças Práticas
- Regular Procuradorias Estaduais e Municipais
- Procuradorias Municipais e Estaduais | Peças Práticas
- Procuradorias | Assinatura
- ENAM | Assinatura
- TSE/ TREs - Unificado | Assinatura
- Tribunais | Assinatura
- Formação Essencial | Assinatura
- 6º ENAM 2026.2 - Online - início 08/09
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
id_oferta: 015
anunciante: "Atleta dos Concursos - OAB"
url_destino: "https://www.facebook.com/61582789201469/"
ad_library_url: "https://www.facebook.com/ads/library/?id=958630850523730"
dias_ativo: 76
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
dias_distintos_coletado: 2
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
id_oferta: 016
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://cadernodoaprovado.com/trf-tj-mp/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1495335635637749"
dias_ativo: 65
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 497,00"
fonte_ticket: "checkout"
tipos_produto: "Material em PDF / apostila / caderno, Mapas mentais / esquemas, Lei seca / legislação"
formatos_dos_anuncios: "imagem (1)"
botoes: "Ver detalhes (1)"
precos_exibidos_na_lp: "R$ 7.150,91 | R$ 891,00 | 12x de R$ 41,42 | R$ 4.715,48 | R$ 14.852,66 | R$ 1.188,00 | 12x de R$ 53,92 | R$ 9.052,51"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
id_oferta: 017
anunciante: "Golden Cursos Jurídicos"
url_destino: "https://www.facebook.com/100083153801246/"
ad_library_url: "https://www.facebook.com/ads/library/?id=4430567703874887"
dias_ativo: 57
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
dias_distintos_coletado: 2
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
id_oferta: 018
anunciante: "Rô Santtana - OAB"
url_destino: "https://rosanttana.com.br/captacao/lp-discursiva-oab.html"
ad_library_url: "https://www.facebook.com/ads/library/?id=1643357417410487"
dias_ativo: 51
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tribunal regional federal, trf1"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Discursiva / redação"
formatos_dos_anuncios: "carrossel (1)"
botoes: "Saiba mais (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
- Preencha os dados abaixo e nossa equipe analisa o seu caso.
- Quero analisar meu caso

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 019
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2465-concurso-trf-1-juiz-federal-prova-oral-online"
ad_library_url: "https://www.facebook.com/ads/library/?id=1649903090184658"
dias_ativo: 20
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf, trf 1"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "imagem (1)"
botoes: "Ver detalhes (1)"
precos_exibidos_na_lp: "R$ 37.765,55 | R$ 10 | R$ 3.859,00 | R$ 2.894,25 | 12x de R$ 241,19"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"TRF-1 em foco?
O Ceisc, responsável pela aprovação de milhares de concurseiros, une-se à expertise da JusFederal na preparação para a Magistratura Federal.
Aprofunde sua performance na fase oral com referências nacionais na área.
➡️ Clique em “Saiba mais e garanta sua vaga!"

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
id_oferta: 020
anunciante: "Hugo de Freitas com 123 Questões"
url_destino: "https://go.123questoes.com.br/lp/tribunais/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1781444589524819"
dias_ativo: 15
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
dias_distintos_coletado: 2
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
id_oferta: 021
anunciante: "Joy Braga Concursos"
url_destino: "https://detoxconcursos.com.br/tribunais/?src=a2d330ebaa55430aaa643cc71bc84863&utm_content=%7B%7Bad.id%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=2078859239389190"
dias_ativo: 13
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
dias_distintos_coletado: 2
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
id_oferta: 022
anunciante: "Advocacia para Concursos - Mattozo & Ribeiro"
url_destino: "https://www.facebook.com/100089931653062/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1934024137978229"
dias_ativo: 13
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
dias_distintos_coletado: 2
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
id_oferta: 023
anunciante: "Olivie Advocacia"
url_destino: "https://www.facebook.com/61588831809684/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1715318876236791"
dias_ativo: 13
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
dias_distintos_coletado: 2
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
id_oferta: 024
anunciante: "Legislação Integrada"
url_destino: "https://www.legislacaointegrada.com.br/trf5/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1023457034050771"
dias_ativo: 10
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
dias_distintos_coletado: 2
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
id_oferta: 025
anunciante: "Professor Raphael Reis"
url_destino: "https://www.facebook.com/profraphaelreis/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2314358442678937"
dias_ativo: 8
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trf"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Questões / simulados, Discursiva / redação"
formatos_dos_anuncios: "imagem (1)"
botoes: "sem botão (1)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
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

### Títulos do link nos anúncios
- instagram.com

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 026
anunciante: "Curso Ênfase"
url_destino: "https://www.facebook.com/cursoenfase/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1935904854235176"
dias_ativo: 8
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
dias_distintos_coletado: 1
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
id_oferta: 027
anunciante: "América Capital"
url_destino: "https://lp.americacapital.com.br/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1087922147551559"
dias_ativo: 8
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
dias_distintos_coletado: 1
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

# Parte 2 — Ofertas adjacentes (50)

Apareceram nas buscas, mas não citam os termos do foco. Servem para comparar formatos e preços de outros nichos de concurso; algumas não são de concurso.

---
id_oferta: 028
anunciante: "Pratique Concursos"
url_destino: "https://ti.pratiqueconcursos.com.br/fcti/tce-go.html"
ad_library_url: "https://www.facebook.com/ads/library/?id=1427104632716607"
dias_ativo: 9
anuncios_coletados: 10
anuncios_ativos_estimados: 10
anuncios_com_baixo_volume_de_impressoes: 5
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "imagem (10)"
botoes: "Saiba mais (10)"
precos_exibidos_na_lp: "R$ 24 | R$ 200 | R$ 147 | R$ 747 | R$ 247 | R$ 397 | R$ 150 | R$ 39,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"<100
Recentemente, foi publicado o novo edital do concurso público de Técnico de Controle Externo na Especialidade de Tecnologia da Informação do Tribunal de Contas do Estado de Goias (TCE GO) com 13 vagas e salário inicial de R$ 11.862.
Observação: o requisito de formação é nível médio, ou seja, qualquer pessoa com ensino médio concluído pode participar.
A prova vai ocorrer no dia 17/01/2027 e cada dia de preparação faz a diferença.
Para te ajudar a se preparar em alto nível preparamos um Super Intensivo 100% focado no cargo de TI do edital, feito por quem foi aprovado em concursos de TI.
O Super Intensivo TCE GO tem a estrutura completa para você aumentar as chances de aprovação no concurso do TCE GO.
Clique em saiba mais e aproveite a promoção para fazer sua matrícula hoje mesmo."

### Ganchos das variações (1ª linha de cada anúncio)
- <100
- Recentemente, foi publicado o novo edital do concurso público de Técnico de Controle Externo na Especialidade de Tecnologia da Informação do Tribunal de Contas do Estado de Goias (TCE GO) com 13 vagas e salário inicial d

### Landing Page: Headline & Promessa Central
"Aumente suas chances de aprovação no concurso de TI do TCE GO — O edital já foi publicado e cada semana até a prova conta. Comece hoje com o método que já ajudou +50 concurseiros a serem aprovados em concursos de TI"

### Seções da Landing Page (títulos, na ordem)
- O que o edital nos diz sobre a prova
- Conheça o professor
- +50 alunos já aprovaram com a Pratique Concursos
- Conheça o Super Intensivo 100% focado no concurso de TI do TCE GO
- Veja o material antes de decidir
- A trilha na prática: seu plano de execução já vem pronto
- 100% Focado no Cargo de TI do edital
- Por que estudar com o Super Intensivo TCE GO ?
- Mais depoimentos enviados por alunos :
- Veja o valor de tudo o que você leva hoje
- Garantia de 7 dias
- 🎯 Comece Sua Preparação Para o Concurso TCE GO!
- Formação Concursado de TI (FCTI)
- Perguntas Frequentes
- P.S. Uma última coisa.

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Discursiva / redação
- Flashcards
- Mapas mentais
- PDF
- Resumos
- Videoaulas


========================================

---
id_oferta: 029
anunciante: "Decorando a Lei Seca Cursos Para Concursos E OAB"
url_destino: "https://www.decorandoaleiseca.com.br/assinatura-ilimitada"
ad_library_url: "https://www.facebook.com/ads/library/?id=1436644861892476"
dias_ativo: 13
anuncios_coletados: 2
anuncios_ativos_estimados: 7
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "hotmart"
ticket_principal: "R$ 499,99"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Assinatura / clube / vitalício, Mapas mentais / esquemas, Questões / simulados, Lei seca / legislação"
formatos_dos_anuncios: "imagem (2)"
botoes: "sem botão (1), Ver detalhes (1)"
precos_exibidos_na_lp: "R$ 7.999,90 | 12x de R$ 49 | R$ 499,99 | 12x de R$ 42,67 | R$ 427,49 | 12x de R$ 49,99 | R$ 697,00 | R$ 7.194,60"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
"A maior Black da história — A banca não testa apenas seu conhecimento; ela testa sua atenção às pegadinhas. Com o nosso método, você treina leitura, repetição e revisão no mesmo ciclo."

### Seções da Landing Page (títulos, na ordem)
- Como funciona na prática
- Cumpra a meta de leitura da lei seca do dia
- Treine no mesmo dia através do Vade Mecum de Questões
- Revise com Mapas Mentais + Decorando a Jurisprudência
- O que muda na prática:
- Conheça a plataforma por dentro
- Raio-X da Lei Seca por banca
- Bancas já liberadas
- Como usar
- Plataforma validada por mais de 310.000 usuários
- Casos de sucesso
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
id_oferta: 030
anunciante: "Decorando a Lei Seca Cursos Para Concursos E OAB"
url_destino: "https://www.facebook.com/decorandoaleisecaconcursoseoab/"
ad_library_url: "https://www.facebook.com/ads/library/?id=443284988264992"
dias_ativo: 921
anuncios_coletados: 6
anuncios_ativos_estimados: 6
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Questões / simulados, Lei seca / legislação"
formatos_dos_anuncios: "carrossel (3), vídeo (2), imagem (1)"
botoes: "Visitar perfil do Instagram (3), sem botão (3)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
- Lançados em abril de 2026
- O art. 20 do Código Penal é daqueles dispositivos que merecem atenção especial na preparação. 👀📚
- JUIZ FEDERAL TRF-5: EDITAL PUBLICADO!
- Lançados em março de 2024
- ⚠️ Uma palavra pode mudar completamente o gabarito da questão.
- O art. 15 do Código Penal voltou a aparecer em prova — dessa vez pela CEBRASPE, no TCE-MG de 2026.

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 031
anunciante: "Professor Fabiano Pereira"
url_destino: "https://aprovatte.com.br/mentoria-start90-2025/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1022817774146362"
dias_ativo: 17
anuncios_coletados: 2
anuncios_ativos_estimados: 6
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento"
formatos_dos_anuncios: "vídeo (2)"
botoes: "sem botão (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 Atenção: foi autorizado um novo concurso do Tribunal de Justiça de GO!
📌 Salário inicial de aproximadamente R$ 14.000,00;
📌 Estabilidade;
👉 O maior diferencial de quem conquista as primeiras colocações não é “ter sorte”, mas sim iniciar a preparação com antecedência.
Não é coincidência: os primeiros colocados nos principais concursos de tribunais do Brasil estudaram conosco.
Se você também quer estar entre os aprovados, aperte agora o botão SAIBA MAIS e receba todas as informações sobre a minha Mentoria, que é focada no concurso do TJ GO. 🚀"

### Landing Page: Headline & Promessa Central
"Mentoria Start90 2025 – Aprovatte"

### Seção "Para Quem NÃO É" (declarado na LP)
- Tenho absoluta convicção da qualidade do curso, tanto que estou tirando o peso da decisão dos seus ombros. Não há risco algum para você!

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Mapas mentais
- Mentoria
- PDF
- Resumos
- Videoaulas


========================================

---
id_oferta: 032
anunciante: "Professor Hansk"
url_destino: "https://hanskcarvalho.com/melhor-que-blackfriday-pago/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1335871585123913"
dias_ativo: 9
anuncios_coletados: 2
anuncios_ativos_estimados: 6
anuncios_com_baixo_volume_de_impressoes: 1
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Discursiva / redação, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (2)"
botoes: "sem botão (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Você estuda, se prepara, domina o conteúdo… mas ainda trava na hora da redação? 📝
Nos dias 13 e 14 de outubro, às 20h, eu vou te mostrar uma estrutura prática e replicável para construir uma redação competitiva em provas de concurso.
No Redação Salva Aprovação, você vai aprender a organizar suas ideias, construir argumentos, entender o que as bancas esperam e acompanhar a construção de uma redação completa na prática.
🎯 Evento 100% gratuito e online.
👉 Clique em Saiba Mais e faça sua inscrição gratuita."

### Landing Page: Headline & Promessa Central
"Melhor que blackfriday | Pago – Hansk Carvalho — 13 e 14 de Outubro | Terça e Quarta | 20hrs"

### Seções da Landing Page (títulos, na ordem)
- 13 e 14 de Outubro | Terça e Quarta | 20hrs
- AULA REDAÇÃO SALVA APROVAÇÃO CONCURSOS BLACK FRIDAY ANTECIPADA
- NESTE EVENTO GRATUITO, VOCÊ VAI DESCOBRIR:
- Introdução Desbloqueada
- Esqueleto da Redação Aprovada
- Banco de Argumentos
- Organização de Ideias
- Raio-X da Banca
- Por que a maioria reprova na discursiva
- Redação completa ao vivo
- O plano completo para ser aprovado na discursiva do seu concurso
- PARA QUEM É O REDAÇÃO SALVA APROVAÇÃO?
- Não sabe por onde começar quando vê o tema da redação na prova
- Sente insegurança ou ansiedade só de pensar em escrever sob pressão
- Já fez curso de redação antes e na hora da prova travou do mesmo jeito
- Demora mais de 37 minutos para terminar um texto e sai sem saber se ficou bom
- Já perdeu classificação ou foi eliminado por causa da nota na discursiva
- Estuda o conteúdo com disciplina mas deixa a redação para depois e sabe que isso é um risco
- Vai fazer concurso policial, educação, saúde, tribunais, bancos, Metrô DF ou INSS e sabe que a discursiva pode ser o que vai te separar dos demais
- Está cansado de adiar e quer chegar na prova com um método claro, replicável e que funciona para qualquer banca
- QUEM VAI TE GUIAR

### Entregáveis / Formato (termos encontrados na LP)
- Discursiva / redação


========================================

---
id_oferta: 033
anunciante: "Pensar-Concursos"
url_destino: "https://pensarconcursos.com/memorex-vitalicio-promo/"
ad_library_url: "https://www.facebook.com/ads/library/?id=28896744059917176"
dias_ativo: 17
anuncios_coletados: 5
anuncios_ativos_estimados: 5
anuncios_com_baixo_volume_de_impressoes: 4
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "hotmart"
ticket_principal: "R$ 97,00"
fonte_ticket: "checkout"
tipos_produto: "Assinatura / clube / vitalício"
formatos_dos_anuncios: "imagem (4), carrossel (1)"
botoes: "Saiba mais (5)"
precos_exibidos_na_lp: "R$ 697,00 | R$ 97 | R$ 997,00 | R$ 197 | R$ 36"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"<100
Carrossel de prova social com relatos individuais de quem utilizou o Memorex. Os depoimentos mostram percepções sobre organização, compreensão e desempenho sem prometer resultados iguais."

### Ganchos das variações (1ª linha de cada anúncio)
- Explore materiais organizados por área, concurso, matéria e banca. Tudo reunido para facilitar sua busca e acelerar o início da revisão.
- <100

### Títulos do link nos anúncios
- 276 conteúdos em uma biblioteca vitalícia
- Diferentes concursos. Uma única biblioteca.
- Veja a prova real
- Direto, organizado e fácil de compreender
- A revisão certa encontra você na prova

### Landing Page: Headline & Promessa Central
"Assinatura Vitalícia Memorex - Por Tempo Limitado — ⚡PROMO RELÂMPAGO⚡"

### Seções da Landing Page (títulos, na ordem)
- ⚡PROMO RELÂMPAGO⚡
- MEMOREX VITALÍCIO
- Menor Preço da História
- NUNCA MAIS gaste com materiais de resumo para Concursos Públicos na vida
- OFERTA EXCLUSIVA, SÓ HOJE
- Acesso Vitalício de TODOS os Resumos Memorex’s para você economizar tempo e ser aprovado nos melhores Concursos Públicos de 2026
- MEMOREX VITALÍCIO ESSENCIAL
- MEMOREX VITALÍCIO PREMIUM
- Método Memorex
- Não importa qual concurso você vá fazer, na Assinatura tem um Memorex perfeito para você! 💙
- ÁREA ADMINISTRATIVA
- ÁREA TRIBUNAIS, DEFENSORIA E MINISTÉRIO PÚBLICO
- ÁREA POLICIAL
- CONCURSO NACIONAL UNIFICADO
- ÁREA BANCÁRIA
- ÁREA EDUCAÇÃO E MUNICIPAL
- ÁREA FISCAL E LEGISLATIVA
- MATÉRIAS ISOLADAS
- São + de 200 Memorex’s e acesso a todos os nossos lançamentos futuros dos principais concursos e carreiras
- OLHA SÓ COMO SÃO NOSSOS MATERIAIS POR DENTRO
- Cada Memorex é composto por Dicas Esquematizadas, Coloridas, Diretas e Certeiras dos temas que vão cair na sua prova do concurso
- TÁ NO MEMOREX? CAI NA PROVA!
- Multiplique suas Chances de Ser Aprovado no Concurso Público com o MEMOREX
- Estudo Otimizado
- Memorização Acelerada
- Revisão Direcionada
- Economia de Tempo
- Saia na Frente
- EXPERIMENTE POR 07 DIAS
- QUEM SOMOS

### Entregáveis / Formato (termos encontrados na LP)
- Discursiva / redação
- Mapas mentais
- PDF
- Questões comentadas
- Resumos
- Simulados


========================================

---
id_oferta: 034
anunciante: "Ser Aprovado"
url_destino: "https://www.facebook.com/seraprovadoconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2504298076719444"
dias_ativo: 10
anuncios_coletados: 5
anuncios_ativos_estimados: 5
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Material em PDF / apostila / caderno"
formatos_dos_anuncios: "carrossel (2), imagem (3)"
botoes: "Enviar mensagem pelo WhatsApp (5)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O concurso do Tribunal de Justiça do Amazonas pode acontecer em 2027, com 400 vagas previstas e salários de até R$ 17 mil.
Quem começa agora estuda com calma, constrói uma base sólida e chega na prova revisando, não correndo atrás.
Na Mentoria Online TJAM você estuda com direção e acompanhamento desde o primeiro dia.
Chama nosso time no WhatsApp e tire suas dúvidas sobre a mentoria.
WHATSAPP
Mentoria Online TJAM"

### Títulos do link nos anúncios
- Concurso do TJAM

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 035
anunciante: "Ceisc Concursos"
url_destino: "https://ceisc.com.br/cursos/2609-mp-pe-analista-ministerial-area"
ad_library_url: "https://www.facebook.com/ads/library/?id=2083764205550271"
dias_ativo: 49
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
precos_exibidos_na_lp: "R$ 7.150,91 | R$ 10 | R$ 1.199,00 | R$ 779,35 | 12x de R$ 64,95"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
id_oferta: 036
anunciante: "Ceisc Concursos"
url_destino: "https://ceisc.com.br/cursos/2237-concurso-ceisc-tribunais-analista-premium"
ad_library_url: "https://www.facebook.com/ads/library/?id=1342835614275761"
dias_ativo: 43
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
precos_exibidos_na_lp: "R$ 10 | R$ 2.853,00 | R$ 1.854,45 | 12x de R$ 154,54"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
id_oferta: 037
anunciante: "Decorando a Lei Seca Cursos para Concursos LTDA"
url_destino: "https://pay.hotmart.com/V105573917A?off=k5lhuvlx&checkoutMode=10&offDiscount=BLUEANDORANGE"
ad_library_url: "https://www.facebook.com/ads/library/?id=3611047645738873"
dias_ativo: 13
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
dias_distintos_coletado: 2
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
id_oferta: 038
anunciante: "Advogado de concurso"
url_destino: "https://olivaesouza.com.br/tce-rs-discursiva/"
ad_library_url: "https://www.facebook.com/ads/library/?id=861868490346562"
dias_ativo: 10
anuncios_coletados: 2
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Discursiva / redação"
formatos_dos_anuncios: "vídeo (2)"
botoes: "sem botão (2)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 Fez a prova discursiva do TCE-RS?
📋 A nota recebida não conta toda a história. É preciso entender como a banca chegou até ela.
🔎 O espelho de correção, os critérios previstos no edital e a pontuação atribuída em cada item precisam ser analisados.
⚠️ Pontos que não foram considerados, critérios aplicados de forma inadequada ou inconsistências na correção podem justificar um questionamento.
⚖️ Faça uma análise técnica da sua prova discursiva e entenda se existem fundamentos para contestar a correção."

### Landing Page: Headline & Promessa Central
"Foi prejudicado na discursiva do TCE RS? Entenda quando cabe ação judicial — Erros de correção, aplicação inadequada dos critérios de avaliação e descumprimento das regras do edital podem justificar a discussão judicial."

### Seções da Landing Page (títulos, na ordem)
- Situações que podem justificar ação judicial na discursiva do TCE RS
- Quando a Justiça pode analisar a correção da discursiva?
- Os tribunais admitem a análise judicial quando existem indícios de ilegalidade na correção, tais como:
- Descumprimento do edital
- Ausência de fundamentação adequada da nota
- Inobservância dos critérios objetivos de correção
- Erros materiais na avaliação
- Violação dos princípios da isonomia e da legalidade
- Cada situação exige análise individualizada para verificar se estão presentes elementos capazes de justificar a adoção de medidas judiciais.
- Por que uma análise especializada faz diferença?
- A análise envolve:
- Edital do concurso
- Espelho de correção
- Justificativa da nota atribuída
- Critérios de avaliação utilizados pela banca
- Entendimento dos tribunais sobre casos semelhantes
- Como funciona a análise do caso?
- O processo é simples:
- 1. Você envia sua prova discursiva e os documentos relacionados à correção
- 2. É realizada uma análise técnica da avaliação aplicada pela banca
- 3. São identificados possíveis indícios de ilegalidade ou inconsistência
- 4. Você recebe orientação sobre os próximos passos possíveis
- Cada concurso possui regras específicas, por isso a análise individual do caso é fundamental.
- Por que é importante agir rapidamente?
- Preencha os dados abaixo para que nossa equipe possa analisar seu caso

### Entregáveis / Formato (termos encontrados na LP)
- Discursiva / redação


========================================

---
id_oferta: 039
anunciante: "Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24"
url_destino: "https://ataticadaaprovacao.com.br/?utm_source=fbads&utm_medium=%7B%7Badset.name%7D%7D&utm_campaign=%7B%7Bad.name%7D%7D&utm_content=%7B%7Bplacement%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1685357465868904"
dias_ativo: 83
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 1
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
dias_distintos_coletado: 2
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
- <100
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
id_oferta: 040
anunciante: "Metodo.Gafanhoto"
url_destino: "https://metodogafanhoto.com/quizz117"
ad_library_url: "https://www.facebook.com/ads/library/?id=4403462513241151"
dias_ativo: 9
anuncios_coletados: 1
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "vídeo (1)"
botoes: "sem botão (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"INDICAÇÃO CONCURSO PARA MULHERES QUE NÃO TEM BASE NOS ESTUDOS"

### Landing Page: Headline & Promessa Central
"Método Gafanhoto"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 041
anunciante: "Gustavo Nogueira - Aprovação Ágil"
url_destino: "https://pages.aprovacaoagil.com.br/vsl/trt/v01"
ad_library_url: "https://www.facebook.com/ads/library/?id=1762089464999221"
dias_ativo: 8
anuncios_coletados: 1
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Questões / simulados"
formatos_dos_anuncios: "vídeo (1)"
botoes: "sem botão (1)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Três anos no cursinho jurídico. Sete apostilões de Direito. E fiquei em cadastro de reserva no primeiro TRT que eu prestei.
Recebi a lista de nomeados no ônibus voltando do trabalho.
Não foi falta de esforço — eu abria a apostila de Direito do Trabalho às 22h todo dia depois do serviço, o caderno vivia cheio. O problema é que ninguém nunca me explicou que eu tava tentando decorar 1.500 artigos ANTES de encarar uma questão.
Quando eu inverti isso, três meses depois eu já passava de 80% em simulado.
Assiste o vídeo e entende como funciona o caminho inverso."

### Landing Page: Headline & Promessa Central
"Aprovação Ágil"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 042
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2331-concurso-experiencia-carreiras-2026"
ad_library_url: "https://www.facebook.com/ads/library/?id=1692155855334789"
dias_ativo: 85
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (2)"
botoes: "Cadastre-se (2)"
precos_exibidos_na_lp: "R$ 10 | R$ 1.799,00 | 12x de R$ 149,92 | R$ 1.619,10 | R$ 4.390,00 | 12x de R$ 365,83 | R$ 3.951,00 | R$ 1.197,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Começar a estudar para concursos com direcionamento certo faz toda a diferença.
O Curso Experiência Carreiras 2026 foi criado para quem deseja conhecer as principais carreiras públicas antes de escolher sua preparação.
Durante 7 dias, você terá acesso gratuito a aulas reais, materiais exclusivos e orientações de professores especialistas para entender como funcionam os concursos e dar os primeiros passos com mais confiança.
Garanta seu acesso gratuito e descubra qual carreira seguir!"

### Ganchos das variações (1ª linha de cada anúncio)
- Quer estar por dentro dos principais concursos? Nosso curso GRATUITO é ideal para você!
- Começar a estudar para concursos com direcionamento certo faz toda a diferença.

### Títulos do link nos anúncios
- Sua Aprovação Começa Aqui

### Landing Page: Headline & Promessa Central
"Experiência Carreiras 2026 — Sobre o curso"

### Seções da Landing Page (títulos, na ordem)
- Sobre o curso
- Nesse curso você terá
- Conheça os professores

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

## Demais adjacentes (resumo)

| id | Anunciante | Dias | Anúncios | Tração | Ticket (checkout) | Destino |
|---|---|---|---|---|---|---|
| 043 | Gazeta dos Concursos | 76 | 2 | médio | Não confirmado | https://lp.aprovacaoagil.com.br/vsl-white-trt-noticia |
| 044 | Concursos Ceisc | 57 | 2 | médio | Não confirmado | https://ceisc.com.br/cursos/2584-concurso-dpe-pb-tecnico-da-defensoria-publica |
| 045 | G7 Jurídico | 49 | 2 | fraco | Não confirmado | https://materiais.g7juridico.com.br/pdf-questoes/cadastro |
| 046 | Decorando a Lei Seca Cursos Para Concursos E OAB | 13 | 2 | médio | R$ 927,50 | https://www.decorandoaleiseca.com.br/ilimitada-vitalicia-dupla |
| 047 | Victor Ribeiro | 10 | 2 | médio | Não confirmado | https://fureafila.com.br/como-memorizar-tudo/ |
| 048 | Estratégia Concursos | 10 | 2 | médio | Não confirmado | https://www.facebook.com/EstrategiaConcursos/ |
| 049 | Prof. Ronaldo Santos | 8 | 2 | médio | Não confirmado | https://rslinguaportuguesa.com/aplicacao-fgv/?utm_source=facebook&utm_medium=cpc |
| 050 | Concursos Ceisc | 211 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2274-concurso-mp-mg-extensivo-premium-analista-do-mp |
| 051 | euvoupassei com Aprovação PGE | 181 | 1 | médio | Não confirmado | https://aprovacaopge.com.br/ |
| 052 | Ceisc Concursos | 178 | 1 | médio | Não confirmado | https://lp.ceisc.com.br/evento-concursos-nivel-medio/ |
| 053 | Ceisc Concursos | 147 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2429-concurso-mp-sc-analista-juridico-extensivo?utm_ |
| 054 | MEQ Concursos | 89 | 1 | médio | Não confirmado | https://www.facebook.com/61586241338760/ |
| 055 | Concurseiro Fora da Caixa | 57 | 1 | médio | Não confirmado | https://concurseiroforadacaixa.com.br/collections/todos-os-materiais |
| 056 | Concursos Ceisc | 51 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2089-concurso-trt-4-club-analista-judiciario-area-ju |
| 057 | Gustavo Nogueira - Aprovação Ágil | 43 | 1 | médio | Não confirmado | https://lp.aprovacaoagil.com.br/vsl-white-trt-noticia |
| 058 | Ceisc Concursos | 40 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2316-concurso-ceisc-tribunais-tecnico-premium |
| 059 | Aprovação ao Além | 40 | 1 | médio | Não confirmado | https://www.facebook.com/61579754455237/ |
| 060 | Concursos Ceisc | 38 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2292-concurso-trt-nacional-club-analista-judiciario- |
| 061 | Verbo Jurídico | 35 | 1 | médio | Não confirmado | https://www.verbojuridico.com.br/pos-graduacoes-a-distancia-ead/pos-graduacao-em |
| 062 | Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24 | 28 | 1 | médio | R$ 297,90 | https://ataticadaaprovacao.com.br/combao/ |
| 063 | Concursos Ceisc | 27 | 1 | médio | Não confirmado | https://lp.ceisc.com.br/material-concurso-trt-4-projeto-nomeacao/ |
| 064 | Concursos Ceisc | 27 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2472-concurso-pge-rs-tecnico-administrativo-extensiv |
| 065 | Concursos Ceisc | 24 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2443-concurso-pge-rs-analista-juridico-extensivo |
| 066 | Evolucional | 22 | 1 | médio | Não confirmado | https://www.facebook.com/evolucional/ |
| 067 | Memorização Bruno Campos Concursos | 21 | 1 | médio | Não confirmado | https://www.facebook.com/100088833677510/ |
| 068 | Perito Cibernético | 20 | 1 | médio | Não confirmado | https://www.facebook.com/peritocibernetico/ |
| 069 | Treine Subjetivas | 11 | 1 | médio | Não confirmado | https://treinesubjetivas.com.br/ |
| 070 | UniEVANGÉLICA | 10 | 1 | médio | Não confirmado | https://selecao.unievangelica.edu.br/direito |
| 071 | Método Supera.con | 10 | 1 | médio | Não confirmado | https://www.facebook.com/61555198180484/ |
| 072 | aprovados.dpero2025 | 10 | 1 | médio | Não confirmado | https://imediato.ncnews.com.br/2026/07/10/aprovados-em-concurso-da-dpe-ro-denunc |
| 073 | Malditafcc | 9 | 1 | médio | Não confirmado | https://www.facebook.com/malditafcc/ |
| 074 | IF Tecnologia | 9 | 1 | médio | Não confirmado | https://meuestudo-concursos.netlify.app/?utm_source=instagram&utm_medium=turbina |
| 075 | Professor Raphael Reis | 8 | 1 | médio | Não confirmado | https://www.professorraphaelreis.com.br/ |
| 076 | Tese Concursos | 8 | 1 | médio | Não confirmado | https://www.facebook.com/TESECONCURSOS/ |
| 077 | Sensei da Aprovação - Concursos Públicos | 8 | 1 | médio | Não confirmado | https://senseidaaprovacao.com.br/projetosenseicuritiba |

# Apêndice — Descartadas por não citarem concurso (50)

Vieram nas buscas (ex.: escritórios que citam o TRF como tribunal), mas o texto não tem nenhum termo de concurso. Confira se algo relevante caiu aqui por engano.

| Anunciante | Dias | Destino |
|---|---|---|
| TRAPP BRASIL | 125 | https://www.trapp.com.br/produto/trf-400-super/ |
| SERV FONE | 99 | https://www.facebook.com/servfone.servfone/ |
| G. Costa Advogados | 73 | http://fb.me/ |
| Judit | 56 | https://produto.judit.io/miner-precatorios |
| OC Advogados com anabeatrizzuviolloadv | 31 | https://www.facebook.com/OCAdvoga/ |
| Aristocrat Watch | 17 | https://www.aristocrat.com.br/products/mission-to-the-moon-1969 |
| Previdenciarista.com - Direito Previdenciário | 10 | https://previdenciarista.com/jurisprudencias-produto/ |
| marcusf_adv | 247 | https://www.instagram.com/_u/marcus.franca.adv |
| 3 Injectors | 181 | https://apps.apple.com/us/app/3injectors-community/id6752955632 |
| Felipe Sgarbossa Advocacia Criminal | 77 | https://www.facebook.com/felipesgarbossa/ |
| Galvani Advocacia | 45 | https://www.facebook.com/galvaniadvocaciacambe/ |
| Previdenciarista.com - Direito Previdenciário | 25 | https://previdenciarista.com/calculos-previdenciarios-produto/ |
| Alibaba.com | 196 | https://www.alibaba.com/product-detail/haoge_1601651875444.html?src=cpm_fb&sub_c |
| futstadistico | 185 | https://www.instagram.com/_u/futstadistico |
| Carolina Bezerra Advocacia | 156 | https://www.facebook.com/61570273217824/ |
| TRRI equipamentos fitness | 146 | https://www.facebook.com/61574319540021/ |
| Dr Benedito Braga | 140 | https://www.facebook.com/BBragaJr/ |
| Evidencia Veículos | 106 | https://www.facebook.com/evidenciatx/ |
| pilateshiitflow com Riven Fitness for Life | 91 | https://www.instagram.com/_u/pilateshiitflow |
| Prime Broker Precatórios | 88 | https://www.facebook.com/61582791240814/ |
| Efraim Vitaliano | 76 | https://www.facebook.com/61578333253215/ |
| RAIR Silva | 57 | https://www.facebook.com/jornalistarairsilva/ |
| AgroTaborda | 56 | https://www.facebook.com/Agrotaborda/ |
| Clínica Ampiezza | 51 | https://www.facebook.com/Ampiezza/ |
| Alibaba.com | 43 | https://www.alibaba.com/product-detail/haoge_1601257754975.html?src=cpm_fb&sub_c |
| Pantheon emagrecimento | 43 | https://www.facebook.com/61567758598809/ |
| CERN - Ranieri Nogueira - Coaching & Mentoring | 39 | https://www.facebook.com/cernmentoria/ |
| Fotógrafos Cristiano e Natieli Strapazzon | 36 | https://www.facebook.com/cristianostrapazzonfotografo/ |
| Erik Navarro Wolkart | 32 | https://www.facebook.com/100070966909521/ |
| use.argos | 30 | https://useargos.com.br/ |
| Tributo em 1 minuto. - Alexandre Ávila | 29 | https://hotmart.com/pt-br/marketplace/produtos/codigos-do-tempo-decadencia-e-pre |
| dr_beretta | 26 | https://www.facebook.com/dr.beretta/ |
| dr_rodrigo_cerqueira | 25 | https://api.whatsapp.com/send |
| Casa dos Parafusos Franca | 24 | https://www.casadosparafusosfranca.com.br/ferramentas-em-geral/balanceadora-de-r |
| LoyLegal | 20 | https://loytrust.com/lp/2026061/ |
| Metodo.Gafanhoto | 17 | https://metodogafanhoto.com/quizz |
| XGKE Educação | 17 | https://www.facebook.com/61591735205886/ |
| Mais Pilates | 17 | https://www.facebook.com/maispilatesrafaelchedid/ |
| Corrêa Barboza Advocacia | 16 | https://api.whatsapp.com/send |
| Precs.oficial | 13 | https://precs.com.br/central-do-credor/ |
| Casarolli Advogados Prev | 13 | https://www.facebook.com/advluiscasarolli/ |
| RevPrev | 11 | https://api.whatsapp.com/send |
| Alison Jesus Advogados | 11 | https://www.facebook.com/100063574359361/ |
| Fono Joyce Emydio | 10 | https://www.facebook.com/61571502493887/ |
| Walquer, Advogado. Advocacia Corporativa. | 10 | https://www.facebook.com/100086713127082/ |
| Felipe Almeida | 10 | https://www.facebook.com/felipealmeidaseudividendo/ |
| Clinicaespacoter Connected Page | 9 | https://api.whatsapp.com/send |
| Mindjus Criminal com Saliba Adv | 8 | https://www.facebook.com/100062961173630/ |
| Laura Da Silva | 8 | https://www.facebook.com/61561327270523/ |
| Rita Bervig | 8 | https://www.facebook.com/100091834883862/ |
