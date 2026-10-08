# Dossiê ConcursoRadar — Justiça Eleitoral — TRE / TSE (08/10/2026)

## Métricas da Rodada
- **Buscas na Meta Ad Library:** `concurso TRE`, `tribunal regional eleitoral`, `concurso TSE unificado`, `justiça eleitoral concurso`, `técnico judiciário`, `TRE SP`, `TRE RJ`, `TRE MG`, `TSE unificado`, `concurso tribunal`
- **Filtro:** anúncios ativos no Brasil, no ar há 7+ dias (coleta ampla para achar padrões; a longevidade é analisada nas tabelas)
- **Ofertas do nicho:** 94 (de 206 anúncios; agrupadas por anunciante + página de destino)
- **Descartadas por não citarem concurso:** 55 (listadas no fim para auditoria)
- **Ofertas de foco direto:** 19 | adjacentes: 75
- **Sinal de tração:** 2 forte, 1 fraco, 91 médio
- **Landing pages lidas:** 63 de 94
- **Ticket confirmado no checkout:** 8 de 10 ofertas com checkout detectado (80%)
- **Tempo de processamento:** 550 segundos

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

Base: **206 anúncios de 77 anunciantes**; 89 estão no ar há 45+ dias (veteranos); mediana de 23 dias.

Como ler: **Anunciantes** = quantos produtores distintos usam (popularidade). **Veteranos** = quantos desses anúncios estão no ar há 45+ dias, e **% dos veteranos** = a fatia da categoria entre todos os veteranos. Se a fatia entre veteranos é maior que a fatia geral (% anúncios), a categoria aparece mais entre os que duram. Categoria com 1 ou 2 anunciantes é só um caso isolado.

A coleta junta duas amostras por busca (anúncios com 7+ dias e anúncios com 45+ dias), então a proporção de veteranos no total não é uma taxa de sobrevivência.

## Formato do criativo

Vídeo, imagem única ou carrossel.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| vídeo | 39 | 51% | 84 | 41% | 57 | 53 | 60% |
| imagem | 32 | 42% | 92 | 45% | 10 | 24 | 27% |
| carrossel | 19 | 25% | 30 | 15% | 28 | 12 | 13% |

## Proporção do criativo

Vertical (4:5 ou 9:16), quadrada (1:1) ou horizontal.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| vídeo vertical | 38 | 49% | 83 | 40% | 57 | 52 | 58% |
| imagem vertical | 26 | 34% | 80 | 39% | 9 | 16 | 18% |
| carrossel vertical | 18 | 23% | 26 | 13% | 33 | 12 | 13% |
| imagem quadrada | 8 | 10% | 12 | 6% | 51 | 8 | 9% |
| carrossel quadrada | 3 | 4% | 4 | 2% | 9 | 0 | 0% |
| vídeo quadrada | 1 | 1% | 1 | 0% | 77 | 1 | 1% |

## Duração dos vídeos

Só anúncios em vídeo.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| 1 a 2min | 18 | 46% | 24 | 29% | 57 | 14 | 26% |
| 31s a 1min | 17 | 44% | 42 | 50% | 57 | 27 | 51% |
| Mais de 2min | 8 | 21% | 9 | 11% | 56 | 6 | 11% |
| Até 30s | 4 | 10% | 9 | 11% | 132 | 6 | 11% |

## Botão (CTA)

Rótulo do botão exibido no anúncio.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| sem botão | 36 | 47% | 81 | 39% | 17 | 28 | 31% |
| Saiba mais | 31 | 40% | 62 | 30% | 15 | 27 | 30% |
| Ver detalhes | 13 | 17% | 35 | 17% | 51 | 23 | 26% |
| Visitar perfil do Instagram | 9 | 12% | 13 | 6% | 89 | 7 | 8% |
| Enviar mensagem pelo WhatsApp | 6 | 8% | 10 | 5% | 10 | 2 | 2% |
| Comprar agora | 2 | 3% | 2 | 1% | 43 | 1 | 1% |
| Enviar mensagem | 1 | 1% | 1 | 0% | 27 | 0 | 0% |
| Fale conosco | 1 | 1% | 1 | 0% | 27 | 0 | 0% |
| Inscreva-se | 1 | 1% | 1 | 0% | 87 | 1 | 1% |

## Destino do clique

Para onde o anúncio leva.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Página própria (LP / site) | 52 | 68% | 153 | 74% | 14 | 61 | 69% |
| Página / formulário no Facebook | 28 | 36% | 47 | 23% | 30 | 22 | 25% |
| WhatsApp | 3 | 4% | 5 | 2% | 125 | 5 | 6% |
| Checkout direto | 1 | 1% | 1 | 0% | 50 | 1 | 1% |

## Tamanho da copy

Texto principal do anúncio.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Média (200 a 600) | 41 | 53% | 110 | 53% | 17 | 44 | 49% |
| Longa (mais de 600) | 36 | 47% | 88 | 43% | 33 | 43 | 48% |
| Curta (até 200 caracteres) | 7 | 9% | 8 | 4% | 13 | 2 | 2% |

## Tipo de gancho (1ª linha da copy)

Classificação por palavras-chave; um gancho pode cair em mais de um tipo.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos | Exemplo |
|---|---|---|---|---|---|---|---|---|
| Outro | 35 | 45% | 58 | 28% | 49 | 30 | 34% | Conheça seus pontos fortes e saiba onde precisa evoluir. — Grupo Revisamed |
| Notícia de concurso / edital | 25 | 32% | 77 | 37% | 10 | 16 | 18% | Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova? — MEQ Concursos |
| Pergunta | 17 | 22% | 48 | 23% | 41 | 24 | 27% | Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova? — MEQ Concursos |
| Dor / erro do candidato | 10 | 13% | 32 | 16% | 9 | 10 | 11% | Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova? — MEQ Concursos |
| Chamada direta ao público | 10 | 13% | 17 | 8% | 17 | 6 | 7% | 🚨 Atenção: foi autorizado um novo concurso do Tribunal de Justiça de GO! — Professor Fabiano Pereira |
| Número / lista | 9 | 12% | 18 | 9% | 19 | 8 | 9% | A Ana Flávia chegou até mim faltando apenas 15 dias para o concurso do Tribunal de Justiça do Rio de Janeiro. — Prof. Ronaldo Santos |
| Salário / estabilidade | 7 | 9% | 17 | 8% | 10 | 6 | 7% | O concurso do Tribunal de Justiça de São Paulo (TJ-SP) é uma das maiores oportunidades para quem tem apenas o ensino médio completo. Além de um excelente salári — Central de Concursos |
| Oferta / desconto / urgência | 7 | 9% | 16 | 8% | 39 | 8 | 9% | "📚🆓 Curso Grátis TJ-SP 2026 - Escrevente Técnico Judiciário! 🆓📚 — Nova Concursos |
| Prova social / autoridade | 6 | 8% | 14 | 7% | 58 | 11 | 12% | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? — Isaque Concursos |
| Promessa de método | 3 | 4% | 12 | 6% | 58 | 12 | 13% | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? — Isaque Concursos |
| Contraintuitivo / inimigo comum | 3 | 4% | 3 | 1% | 77 | 2 | 2% | Três anos no cursinho jurídico. Sete apostilões de Direito. E fiquei em cadastro de reserva no primeiro TRT que eu prestei. — Gustavo Nogueira - Aprovação Ágil |

## Elementos da copy

Recursos presentes no texto; não são excludentes.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Usa emojis | 46 | 60% | 133 | 65% | 30 | 65 | 73% |
| Cita valor em R$ | 20 | 26% | 52 | 25% | 9 | 8 | 9% |
| Hashtags | 19 | 25% | 30 | 15% | 58 | 17 | 19% |
| Lista com marcadores (✔, ✅, •) | 16 | 21% | 44 | 21% | 58 | 29 | 33% |
| Gancho em CAIXA ALTA | 10 | 13% | 18 | 9% | 8 | 3 | 3% |
| Link ou 'link na bio' no texto | 9 | 12% | 13 | 6% | 57 | 8 | 9% |
| Cita bônus | 5 | 6% | 11 | 5% | 58 | 8 | 9% |
| Cita garantia | 3 | 4% | 4 | 2% | 28 | 1 | 1% |

## Sinais de público (ICP) citados na copy

Quem o anúncio diz atender, por palavras-chave. Indica a quem o mercado fala, não quem compra.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos | Exemplo |
|---|---|---|---|---|---|---|---|---|
| Motivado por salário / estabilidade | 23 | 30% | 65 | 32% | 10 | 20 | 22% | Se você quer chegar competitivo para ser aprovado e nomeado nas próximas provas de TRTs, a Imersão Aprova TRT pode ser um divisor de águas para conquistar a tão — Isaque Concursos |
| Esquece o que estuda / revisão | 15 | 19% | 30 | 15% | 38 | 14 | 16% | Mais do que contar acertos, a proposta é usar o treino para tomar decisões melhores, o que revisar, onde investir e como direcionar as próximas horas de estudo. — Grupo Revisamed |
| Dificuldade em discursiva / redação | 10 | 13% | 32 | 16% | 9 | 7 | 8% | Não para estudar mais um pouco. Para sentar, encarar 60 questões seguidas, matérias misturadas, discursiva e o relógio correndo. — MEQ Concursos |
| Trabalha / tem pouco tempo | 9 | 12% | 34 | 17% | 58 | 26 | 29% | Durante essa jornada de estudos, eu estudava de 2h a 3h por dia, já que estudava e trabalhava como CLT. — Isaque Concursos |
| Pré-edital / sair na frente | 9 | 12% | 27 | 13% | 17 | 7 | 8% | 🚨 Atenção: foi autorizado um novo concurso do Tribunal de Justiça de GO! — Professor Fabiano Pereira |
| Nível médio | 9 | 12% | 26 | 13% | 9 | 11 | 12% | Para você ter uma ideia, eu só me formei no ensino médio por meio do ENCCEJA, já que tinha repetido em todas as matérias. — Isaque Concursos |
| Reta final / pós-edital | 7 | 9% | 7 | 3% | 40 | 3 | 3% | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. — Tjteiros |
| Estuda há tempo e não passa | 6 | 8% | 15 | 7% | 72 | 12 | 13% | Você estuda, se prepara, domina o conteúdo… mas ainda trava na hora da redação? 📝 — Professor Hansk |
| Começando do zero | 5 | 6% | 16 | 8% | 58 | 13 | 15% | • Esteja começando os estudos agora; — Isaque Concursos |
| Mãe / família | 4 | 5% | 12 | 6% | 58 | 11 | 12% | Se isso não fosse o bastante, eu tive uma infância/adolescência bem difícil. Sou filho de ex -empregada doméstica e, por isso, não tínhamos condições financeira — Isaque Concursos |
| Nível superior / Direito | 2 | 3% | 2 | 1% | 139 | 2 | 2% | Trata-se de uma oportunidade de nível superior com MUITAS vagas, e uma remuneração inicial muito atrativa. — Concursos Ceisc |
| Erra questões / pegadinhas da banca | 1 | 1% | 3 | 1% | 47 | 2 | 2% | E é justamente nessa diferença que as bancas constroem a pegadinha. — Decorando a Lei Seca Cursos Para Concursos E OAB |
| Perdido no excesso de conteúdo | 1 | 1% | 2 | 1% | 494 | 2 | 2% | O novato nos concursos se sente perdido e muitas vezes tenta desbravar essa selva sozinho, tentando decifrar a matéria em uma linguagem nem sempre adequada para — Caderno do Aprovado - Materiais para Concursos |

## Tipo de produto × ticket

Tipo identificado por palavras-chave na copy, no título do link e na headline (uma oferta pode ter vários). Ticket só entra quando foi lido no checkout.

| Tipo de produto | Anunciantes | Ofertas | Veteranas | Com ticket lido | Mínimo | Mediana | Máximo | Tickets lidos |
|---|---|---|---|---|---|---|---|---|
| Material em PDF / apostila / caderno | 38 | 41 | 24 | 3 | R$ 298 | R$ 497 | R$ 1.489 | Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24 R$ 298; Caderno do Aprovado - Materiais para Concursos R$ 497; Discursiva na Prática R$ 1.489 |
| Curso em videoaulas | 19 | 24 | 16 | 3 | R$ 827 | R$ 1.489 | R$ 6.346 | Instituto INAPI R$ 827; Discursiva na Prática R$ 1.489; Ceisc Concursos R$ 6.346 |
| Isca gratuita / grupo VIP | 16 | 20 | 8 | 4 | R$ 298 | R$ 662 | R$ 6.346 | Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24 R$ 298; Isaque Concursos R$ 497; Instituto INAPI R$ 827; Ceisc Concursos R$ 6.346 |
| Questões / simulados | 15 | 18 | 5 | 2 | R$ 827 | R$ 832 | R$ 837 | Instituto INAPI R$ 827; Serviço Social para Concursos R$ 837 |
| Não identificado | 13 | 13 | 4 | 0 | — | — | — |  |
| Mentoria / acompanhamento | 12 | 13 | 9 | 2 | R$ 497 | R$ 667 | R$ 837 | Isaque Concursos R$ 497; Serviço Social para Concursos R$ 837 |
| Discursiva / redação | 11 | 12 | 6 | 2 | R$ 837 | R$ 1.163 | R$ 1.489 | Serviço Social para Concursos R$ 837; Discursiva na Prática R$ 1.489 |
| Cronograma / plano de estudos | 9 | 13 | 9 | 2 | R$ 497 | R$ 667 | R$ 837 | Isaque Concursos R$ 497; Serviço Social para Concursos R$ 837 |
| Lei seca / legislação | 7 | 8 | 6 | 1 | R$ 497 | R$ 497 | R$ 497 | Caderno do Aprovado - Materiais para Concursos R$ 497 |
| Mapas mentais / esquemas | 3 | 3 | 1 | 2 | R$ 497 | R$ 667 | R$ 837 | Caderno do Aprovado - Materiais para Concursos R$ 497; Serviço Social para Concursos R$ 837 |
| Assinatura / clube / vitalício | 2 | 2 | 1 | 2 | R$ 837 | R$ 1.163 | R$ 1.489 | Serviço Social para Concursos R$ 837; Discursiva na Prática R$ 1.489 |
| Flashcards | 1 | 2 | 2 | 0 | — | — | — |  |

## Expressões repetidas entre anunciantes

Sequências de 2 ou 3 palavras (sem acento) usadas na copy por 3 ou mais anunciantes distintos.

`clique em saiba` (15), `tecnico judiciario` (10), `tribunal de justica` (8), `tribunal de contas` (8), `garanta sua vaga` (8), `agora mesmo` (7), `vagas limitadas` (5), `tribunal regional` (5), `tj sp` (5), `novo concurso` (5), `nivel medio` (5), `ensino medio` (5), `concursos de tribunais` (5), `concurso publico` (5), `analista judiciario` (5), `see details` (4), `salario inicial` (4), `quem estuda` (4), `pode sair` (4), `escrevente tecnico judiciario` (4), `edital sair` (4), `concursos publicos` (4), `concurso do tribunal` (4), `alto nivel` (4), `ultimo concurso` (3), `trt pi` (3), `toque no botao` (3), `toque em saiba` (3), `sair para comecar` (3), `r$ 11` (3)

## Arquivo de ganchos (anúncios mais replicados e mais antigos)

| Anunciante | Dias | Cópias | Formato | Botão | Gancho (1ª linha) | Título do link |
|---|---|---|---|---|---|---|
| MEQ Concursos | 9 | 13 | imagem | sem botão | Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova? |  |
| Isaque Concursos | 58 | 4 | vídeo | sem botão | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? |  |
| Nova Concursos | 48 | 3 | imagem | sem botão | "📚🆓 Curso Grátis TJ-SP 2026 - Escrevente Técnico Judiciário! 🆓📚 |  |
| Professor Fabiano Pereira | 17 | 3 | vídeo | sem botão | 🚨 Atenção: foi autorizado um novo concurso do Tribunal de Justiça de GO! |  |
| Grupo Revisamed | 14 (baixo volume) | 3 | imagem | Saiba mais | Conheça seus pontos fortes e saiba onde precisa evoluir. |  |
| Metodo.Gafanhoto | 9 | 3 | vídeo | sem botão | INDICAÇÃO CONCURSO PARA MULHERES QUE NÃO TEM BASE NOS ESTUDOS |  |
| Professor Hansk | 9 (baixo volume) | 3 | vídeo | sem botão | Você estuda, se prepara, domina o conteúdo… mas ainda trava na hora da redação? 📝 |  |
| Gustavo Nogueira - Aprovação Ágil | 8 | 3 | vídeo | sem botão | Dá pra passar em escrevente sem ser do Direito? Dá. E não é porque a prova é fácil — é porque ela não te pede pra recitar a lei. |  |
| Gustavo Nogueira - Aprovação Ágil | 8 | 3 | vídeo | sem botão | Três anos no cursinho jurídico. Sete apostilões de Direito. E fiquei em cadastro de reserva no primeiro TRT que eu prestei. |  |
| Tjteiros | 97 | 2 | vídeo | sem botão | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. |  |
| Central de Concursos | 86 | 2 | vídeo | sem botão | O concurso do Tribunal de Justiça de São Paulo (TJ-SP) é uma das maiores oportunidades para quem tem apenas o ensino médio completo. Além de um excelente salário inicial, você conquista estabilidade financeira, benefício |  |
| Estratégia Concursos | 84 | 2 | vídeo | sem botão | 📢 O professor Herbert Almeida indica: vale a pena estudar para CGU e Tribunal de Contas da União! |  |
| Venâncio & Delgado - Advogados | 58 | 2 | vídeo | sem botão | ⚖️ A banca examinadora pode mudar de entendimento e te eliminar como PCD? Saiba o que o Superior Tribunal de Justiça (STJ) decidiu! |  |
| Serviço Social para Concursos | 29 | 2 | vídeo | sem botão | Quem quer uma vaga no sociojurídico sabe: não dá para estudar de qualquer jeito. |  |
| Tucuju Bizurado Concursos | 17 | 2 | carrossel | Saiba mais | Comente PC AMAPÁ e comece sua preparação agora!! | Checkout Tutory |
| Advogado de concurso | 10 | 2 | vídeo | sem botão | 🚨 Fez a prova discursiva do TCE-RS? |  |
| Prof. Ronaldo Santos | 8 | 2 | imagem | sem botão | A Ana Flávia chegou até mim faltando apenas 15 dias para o concurso do Tribunal de Justiça do Rio de Janeiro. |  |
| Caderno do Aprovado - Materiais para Concursos | 924 | 1 | imagem | sem botão | A matéria para concurso já é grande e os cursinhos ainda complicam mais: centenas de horas de videoaulas e milhares de páginas de PDFs. | Simbora Concursos |
| Simbora Concursos | 924 | 1 | carrossel | Visitar perfil do Instagram | Quando eu comecei a estudar para Tribunais, ficar "nas cabeças" era algo inimaginável... 1º lugar, então? Era coisa de maluco, extraterrestre, etc. |  |
| Caderno do Aprovado - Materiais para Concursos | 785 | 1 | carrossel | Visitar perfil do Instagram | Lançados em agosto de 2024 |  |
| Caderno do Aprovado - Materiais para Concursos | 727 | 1 | carrossel | Visitar perfil do Instagram | Lançados em outubro de 2024 |  |
| Caderno do Aprovado - Materiais para Concursos | 616 | 1 | vídeo | sem botão | Lançados em janeiro de 2025 |  |
| Caderno do Aprovado - Materiais para Concursos | 612 | 1 | carrossel | Visitar perfil do Instagram | Lançados em fevereiro de 2025 |  |
| Escola Flamengo - Unid Santos | 205 | 1 | imagem | Enviar mensagem pelo WhatsApp | Lançados em março de 2026 |  |
| Pódio Tribunais | 198 | 1 | vídeo | sem botão | Você estuda 4, 5 ou até 6 horas por dia e sente que não sai do lugar? |  |
| Concursos Ceisc | 191 | 1 | vídeo | Saiba mais | A sua preparação para o TJ-SP exige foco e direcionamento. |  |
| Concursos Ceisc | 191 | 1 | vídeo | Saiba mais | O edital do concurso do TJ-BA com o cargo de Analista Judiciário pode sair a qualquer momento, e o momento de estudar é agora. 🚀 |  |
| Gaby no Tribunal | 175 | 1 | carrossel | Visitar perfil do Instagram | Qual desses apps & sites você ainda não conhecia? Algum usa no seu dia a dia? Ah, se tiver uma outra indicação pode deixar nos comentários, amo descobrir novos kkkkk 💜 | Gaby Ungareli / TJSP (@gabynotribunal) • Instagram photos and videos |
| Felipe Sgarbossa Advocacia Criminal | 166 | 1 | vídeo | sem botão | 🗣️ Sustentação oral em Revisão Criminal envolvendo a correta delimitação das imputações e a aplicação do conceito de crime único no tráfico de drogas. |  |
| Concursos Ceisc | 132 | 1 | vídeo | Ver detalhes | O Concurso para Escrevente Técnico Judiciário do Tribunal de Justiça de São Paulo deve ter seu edital publicado em 2026. | Aprove com Ceisc |
| Concursos Ceisc | 132 | 1 | vídeo | Ver detalhes | Já pensou ser Escrevente Técnico Judiciário do TJ-SP, atuar no maior tribunal da América Latina e receber mais de R$ 6 mil/mês? | Aprove com Ceisc |
| Discursiva na Prática | 126 | 1 | vídeo | Saiba mais | 🎟 Use o cupom DP10 e entre com 10% de desconto na Assinatura Controle. |  |
| Junior Alcantara | 125 | 1 | vídeo | Enviar mensagem pelo WhatsApp | R$900 - TRATAMENTO COMPLETO PARA DEPENDÊNCIA QUÍMICA, ALCOOLISMO E SAÚDE MENTAL. | CLÍNICA DE REABILITAÇÃO |
| Prof.carlosgoncalves | 121 | 1 | imagem | Saiba mais | 90% dos candidatos a Analista de Tribunal estão cometendo um erro fatal neste exato momento: estudando de forma passiva e sem direção. |  |
| Prof.carlosgoncalves | 118 | 1 | imagem | Saiba mais | Seja honesto com você mesmo: se a prova para Analista de Tribunal fosse no próximo domingo, você estaria pronto para assinar o termo de posse ou seria apenas mais um na lista de reprovados? | Projeto Analista de Tribunais |
| Douglas Prado - Servidor 30k | 103 | 1 | vídeo | Saiba mais | EXCLUSIVO PARA SERVIDORES PÚBLICOS |  |
| Rafael Amaral Adv | 94 | 1 | vídeo | sem botão | Você se preparou, enviou toda a documentação para o PSS do HEMOAM, mas o resultado não foi o que você esperava por um erro da banca? |  |
| Fauth e Freitas Sociedade de Advogados com Adriane Fauth | 92 | 1 | vídeo | sem botão | Concorre como PcD e seu concurso prevê testes físicos ? Veja esse vídeo entenda o novo entendimento do STF! #concurso #concursopúblico #advocacia #pcd #inclusãopcds | Fauth e Freitas Sociedade de Advogados |
| MEQ Concursos | 89 | 1 | carrossel | Visitar perfil do Instagram | Alguns TRTs estão entrando em uma fase decisiva. 👀 |  |
| MEQ Concursos | 89 | 1 | vídeo | sem botão | Tem tribunal com banca em definição, grupo de trabalho formado, concurso prorrogado e validade chegando ao fim. Não é promessa de edital imediato, mas é cenário para acompanhar de perto. |  |

---

# Parte 1 — Ofertas de foco direto (19)

---
id_oferta: 001
anunciante: "MEQ Concursos"
url_destino: "https://meqconcursos.com.br/concurso-simulado-meq-2-analista-trt-v2-l/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1546020470659112"
dias_ativo: 9
anuncios_coletados: 17
anuncios_ativos_estimados: 64
anuncios_com_baixo_volume_de_impressoes: 3
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados, Discursiva / redação, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (5), imagem (12)"
botoes: "sem botão (14), Ver detalhes (2), Saiba mais (1)"
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
anunciante: "Isaque Concursos"
url_destino: "https://projetotrt.com.br/imersao1v1/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1556242356236977"
dias_ativo: 62
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
dias_distintos_coletado: 2
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
id_oferta: 003
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
id_oferta: 004
anunciante: "Portal Concursos"
url_destino: "https://oportalconcursos.com.br/h-adm-trt-mt/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1436015981795868"
dias_ativo: 8
anuncios_coletados: 11
anuncios_ativos_estimados: 11
anuncios_com_baixo_volume_de_impressoes: 2
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (11)"
botoes: "Saiba mais (11)"
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
id_oferta: 005
anunciante: "Nova Concursos"
url_destino: "https://aprovacao.novaconcursos.com.br/curso-gratis-tj-sp-escrevente-ads-ca2"
ad_library_url: "https://www.facebook.com/ads/library/?id=1621019016255950"
dias_ativo: 49
anuncios_coletados: 6
anuncios_ativos_estimados: 8
anuncios_com_baixo_volume_de_impressoes: 1
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Questões / simulados, Cronograma / plano de estudos, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (4), vídeo (2)"
botoes: "Ver detalhes (5), sem botão (1)"
precos_exibidos_na_lp: "R$ 297,00 | R$ 0,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"<100
"📚🆓 Curso Grátis TJ-SP 2026 - Escrevente Técnico Judiciário! 🆓📚
Prepare-se para o TJ-SP 2026 com nosso curso grátis! 🌟
✅ 24 Aulas abrangentes para dominar o conteúdo do TJ-SP 2026.
📅 Plano de Estudos projetado para apenas 1 hora por dia - encaixe nos seus horários.
👨‍🏫 Tutoria Especializada com Professores experientes para esclarecer todas as suas dúvidas.
📝 Questões atualizadas para você praticar e se preparar da melhor maneira.
Inscreva-se agora mesmo e comece sua jornada rumo ao sucesso no TJ-SP 2026! 🚀"

### Ganchos das variações (1ª linha de cada anúncio)
- "📚🆓 Curso Grátis TJ-SP 2026 - Escrevente Técnico Judiciário! 🆓📚
- <100

### Títulos do link nos anúncios
- Garante sua Vaga!

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
id_oferta: 006
anunciante: "Nova Concursos"
url_destino: "https://aprovacao.novaconcursos.com.br/curso-gratis-tj-sp-escrevente-ads-great"
ad_library_url: "https://www.facebook.com/ads/library/?id=2193053974942953"
dias_ativo: 9
anuncios_coletados: 5
anuncios_ativos_estimados: 5
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Questões / simulados, Cronograma / plano de estudos, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (5)"
botoes: "Ver detalhes (5)"
precos_exibidos_na_lp: "R$ 297,00 | R$ 0,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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

### Títulos do link nos anúncios
- Garante sua Vaga!

### Landing Page: Headline & Promessa Central
"INSCRIÇÕES GRATUITAS LIBERADA 🔥 — De: R$ 297,00"

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
id_oferta: 007
anunciante: "Ceisc Concursos"
url_destino: "https://lp.ceisc.com.br/projeto-nomeacao-tj-sp/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2095494471007965"
dias_ativo: 87
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "sympla"
ticket_principal: "R$ 6.345,94"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (3)"
botoes: "Ver detalhes (2), Inscreva-se (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
- Os cargos de Escrevente Técnico e Oficial de Justiça do Tribunal de Justiça de São Paulo exercem papéis essenciais para solucionar o alto volume de processos que tramitam na instituição.
- Seu objetivo é ser Oficial de Justiça ou Escrevente Técnico Judiciário do maior tribunal da América Latina?
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
id_oferta: 008
anunciante: "Caderno Mapeado"
url_destino: "https://cadernomapeado.com.br/tce-ma-cmlm/?src=&utm_source=facebook-ads&utm_medium=%7B%7Badset.name%7D%7D&utm_content=%7B%7Bad.name%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D&utm_term=%7B%7Bplacement%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1718780919341886"
dias_ativo: 58
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tse"
plataforma_checkout: "eduzz"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Lei seca / legislação"
formatos_dos_anuncios: "vídeo (3)"
botoes: "Ver detalhes (3)"
precos_exibidos_na_lp: "R$ 20.940,20 | R$ 20.000 | R$ 97,00 | R$ 0,00 | R$ 59,00 | R$ 57,00 | R$ 77,00 | R$ 27,90"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"💥Concurso do TCE-MA (Tribunal de Contas do Estado do Maranhão) 💥Estabilidade e remuneração inicial que ultrapassa os R$20 mil. Essa é a sua chance de garantir a sua vaga no concurso mais aguardado de 2026!
E sabe o que é melhor? VOCÊ PODE SER APROVADO EM APENAS 30 DIAS DE ESTUDO.
Já parou para imaginar o seu nome na lista de aprovados?
O quanto isso transformaria a sua vida?
Agora, visualize: você como servidor público, com a tão sonhada estabilidade financeira e conquistando o futuro que merece.
Nós temos o material certo para você!
Esse método já foi testado e aprovado por quem alcançou resultados reais, incluindo muitos que garantiram suas vagas no último concurso do TSE! Agora é a sua vez de realizar esse sonho.
🔓 E ainda tem mais!
Ao garantir hoje a sua Legislação Mapeada para o concurso do TCE-MA, receberá 2 BÔNUS EXCLUSIVOS para turbinar sua preparação.
Ser concursado está no topo das suas metas para 2026, certo? Então, é hora de tirar esse sonho do papel e começar a estudar AGORA!
Não perca mais tempo com métodos ultrapassados que não funcionam. Clique em SAIBA MAIS agora mesmo e inicie sua jornada rumo à aprovação!"

### Títulos do link nos anúncios
- TCE MA - Edital Publicado!

### Landing Page: Headline & Promessa Central
"Perguntas Frequentes — Sim. Todo material é atualizado conforme edital publicado."

### Seções da Landing Page (títulos, na ordem)
- Cronograma de 30 dias
- Caderno Mapeado
- Legislação mapeada
- Técnicas de aprendizagem
- Foco na Cebraspe
- +90.000 alunos
- Cronograma 30 dias
- Revisão Mapeada
- Aprenda a Ler a Lei
- Raio X da Banca CEBRASPE
- O que nossos alunos estão falando sobre os nossos materiais ?
- Comece agora e seja aprovado no concurso do TCE MA!
- Escolha o seu cargo
- Quer se preparar somente com os Conhecimentos Gerais?
- Leve todos os materiais em uma condição exclusiva
- Além do material completo, confira TUDO que você vai receber:
- Garantia incondicional

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Mapas mentais
- Videoaulas


========================================

---
id_oferta: 009
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2092-concurso-tj-sp-club-escrevente-tecnico-judiciario?utm_source=meta_ads&utm_medium=cpc&utm_campaign=vendas_tj_sp_escrevente"
ad_library_url: "https://www.facebook.com/ads/library/?id=864887869547603"
dias_ativo: 132
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
precos_exibidos_na_lp: "R$ 6 | R$ 6.345,94 | R$ 10 | R$ 1.797,00 | R$ 1.078,20 | 12x de R$ 89,85"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
id_oferta: 010
anunciante: "MEQ Concursos"
url_destino: "https://www.facebook.com/61586241338760/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1684375369487437"
dias_ativo: 89
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "carrossel (1), vídeo (1)"
botoes: "Visitar perfil do Instagram (1), sem botão (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Tem tribunal com banca em definição, grupo de trabalho formado, concurso prorrogado e validade chegando ao fim. Não é promessa de edital imediato, mas é cenário para acompanhar de perto.
Quem estuda para Técnico Judiciário ou Analista Judiciário precisa observar agora os próximos concursos de TRT e organizar a preparação antes da publicação do edital.
Encaminhe para um amigo concurseiro e não esquece…
Dia 15/07 temos um encontro marcado com o workshop gratuito 5 Pilares do Estudo para TRT.
Link na bio. 😌"

### Ganchos das variações (1ª linha de cada anúncio)
- Alguns TRTs estão entrando em uma fase decisiva. 👀
- Tem tribunal com banca em definição, grupo de trabalho formado, concurso prorrogado e validade chegando ao fim. Não é promessa de edital imediato, mas é cenário para acompanhar de perto.

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 011
anunciante: "Isaque Concursos"
url_destino: "https://projetotrt.com.br/vsl1v1/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1023281740551609"
dias_ativo: 62
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "onprofit"
ticket_principal: "R$ 497,00"
fonte_ticket: "checkout"
tipos_produto: "Mentoria / acompanhamento, Cronograma / plano de estudos"
formatos_dos_anuncios: "vídeo (2)"
botoes: "Saiba mais (2)"
parcelas: "12x R$ 42,99"
precos_exibidos_na_lp: "12x de R$ 43 | R$ 9.776,71 | R$ 90,00 | R$ 11.928 | R$ 0 | R$ 997 | R$ 100 | R$ 497"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
- Tenha tudo que você precisa para estudar em alto nível para qualquer TRT do Brasil com o Projeto TRT🔥
- Tenha organização e direcionamento para

### Títulos do link nos anúncios
- TRT: Estude em Alto Nível
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
id_oferta: 012
anunciante: "Instituto INAPI"
url_destino: "https://cursos.inapionline.com.br/pre-trt-pi"
ad_library_url: "https://www.facebook.com/ads/library/?id=1054686240270707"
dias_ativo: 52
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 827,00"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Questões / simulados, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (1), vídeo (1)"
botoes: "Ver detalhes (1), Saiba mais (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
id_oferta: 013
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
id_oferta: 014
anunciante: "Simbora Concursos"
url_destino: "https://www.facebook.com/simboraconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=3157233831074462"
dias_ativo: 924
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tre, tse"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "carrossel (1)"
botoes: "Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Quando eu comecei a estudar para Tribunais, ficar "nas cabeças" era algo inimaginável... 1º lugar, então? Era coisa de maluco, extraterrestre, etc.
Olhando para trás, sinto orgulho por ter abaixado a cabeça, não para se conformar e desistir, mas para lutar pelo meu espaço, pela minha vez.
Olhando para frente, sinto ainda mais orgulho por ver vocês alcançando lugares cada vez mais altos.
No TRT-21 foram vários alunos aprovados, e agora no TRT-11 simplesmente a primeiríssima lugar.
Não sei o que dizer... apenas sentir.
Por aqui sigo trabalhando na intenção de sempre melhorar a minha entrega. A única certeza é que não vamos parar por aqui. Vamos buscar mais... Bora junto?
#trt11 #tre #tse #concursotse #concursotre #concursotseunificado #tseunificado #treunificado #concursotribunais #tribunais #concursopublico #concursopúblico #concursos #concursospublicos #concursospúblicos #concursosdetribunais #trt #concursotrt #concursosdetrts #trt7 #trtce #concursotrtce #concursotrt7 #trt6 #trtpe #trt20 #trtsergipe #trt24 #trtms"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 015
anunciante: "Junior Alcantara"
url_destino: "http://wa.me/5511934328043"
ad_library_url: "https://www.facebook.com/ads/library/?id=1425722342913421"
dias_ativo: 125
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tre"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Cronograma / plano de estudos"
formatos_dos_anuncios: "vídeo (1)"
botoes: "Enviar mensagem pelo WhatsApp (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Captura de Lead (WhatsApp / Grupo VIP)"
heuristica_nicho_estimado: "Área da Saúde"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"R$900 - TRATAMENTO COMPLETO PARA DEPENDÊNCIA QUÍMICA, ALCOOLISMO E SAÚDE MENTAL.
Junior Alcantara - CRT/FEMOTEBR: 0384/21
wa.me/5511934328043
*CRONOGRAMA DE TRATAMENTO*
📍 EQUIPE TÉCNICA E DISCIPLINAR
✅ ENFERMEIRA
✅ TÉC ENFERMAGEM
✅ PSICÓLOGA
✅ PSIQUIATRA
✅ TERAPÊUTAS
✅ COORDENADORES DISCIPLINARES (24 HORAS)
📍 ALIMENTAÇÕES DIÁRIAS (4)
✅ CAFÉ DA MANHÃ
✅ ALMOÇO
✅ CAFÉ DA TARDE
✅ JANTAR
📍 ATIVIDADES
✅ EDUCAÇÃO FISICA
✅ RELAXAMENTO/MEDITAÇÃO
✅ P.P.R
✅ TRE
✅ N.A.
✅ AVALIAÇÕES MENSAIS
TEÓRICA E COMPORTAMENTAIS
📍 Plano e Proposta de Tratamento
📍 Etapa (1º e 2º Mês)
✅ Aspecto Físico, desintoxicação e adaptação ao convívio;
conhecimento do programa; Reeducação alimentar, bem como aspectos físicos fragilizados pelo motivo do uso compulsivo da droga e do álcool.
📍 2ª Etapa (3º e 4º Mês)
✅ Aspecto psicológico (autoconhecimento de seu eu interior e de sua doença) Terapias e psicologia aplicada.
📍 3ª Etapa (5º e 6º Mês)
✅ Aspecto Espiritual (valorizar as pequenas coisas e desta maneira valorizar a vida) Fé em um poder superior.
✅ Os princípios fundamentais que regem nossa instituição são:
O AMOR, DISCIPLINA, RESPONSABILIDADE, ESPIRITUALIDADE,
LIBERDADE e TRABALHO, visando à melhoria da qualidade de vida do dependente e sua família.
✅ A Dependência Química é uma doença: progressiva, incurável e fatal, logo a recuperação é progressiva, contínua e traz vida em plenitude. Não existe uma cura, médico ou remédios, pois ela é incurável. O que podemos fazer é tratar e estacionar.
O modelo de internação que seguimos é o de conscientização.
Baseado na filosofia de doze passos de Alcoólicos Anônimos (AA) e Narcóticos Anônimos (NA), estamos alcançando excelentes resultados.
✅ Oferecemos ao residente, dentro de nossas dependências o programa de doze passos, espiritualidade, terapia Racional Emotiva:
programa de prevenção a recaída, arte terapia, vídeo terapia, laborterapia, atendimento psicológico individual e em grupo, quatro refeições diárias e demais necessidades para a recuperação do internado .
*Atividades Terapêuticas*
📍 Espiritualidade
✅ Realizada após o café da manhã é a primeira reunião do dia.
Cantamos louvores no início da reunião, depois é lido um capítulo da Bíblia Sagrada e aberto para que o grupo comente ao término o facilitador da reunião faz as considerações finais e cantamos novamente pedindo ao nosso poder superior (DEUS) orientação em nosso dia.
📍 Reunião de sentimentos:
✅ Esta reunião tem por objetivo, fazer com que a residente partilhe os sentimentos identificados no decorrer do dia. É muito importante esta reunião de partilha, pois a residente aprende a identificar e expressar seus sentimentos, tornando-se conhecido para o restante do grupo, e ouvindo sua própria voz falando de si. Este também ouve as individualidades do outro. Tudo isso com a possibilidade de ouvir retorno dos companheiros. O retorno é uma forma de avaliação,
e de ser ajudada por parte dos companheiros aos sentimentos que vive o partilhador, sempre com intuito de crescimento na recuperação.
É através dos retornos que os companheiros, a partir de suas experiências sugerem alternativas. Sempre quando alguém partilha seus sentimentos,
eles coincidem com os sentimentos de outras companheiras ali presentes, formando-se assim, elos de união e objetivos comuns.
📍 Psicoterapia Individual :
✅ Este atendimento possibilita com que a residente entre em contato com suas dificuldades e consiga alternativas viáveis ao seu equilíbrio emocional, promovendo o desbloqueio de núcleos de conflitos que geram situações tensionais.
Propicia um espaço de reflexão, buscando estratégias de enfrentamento para situações de risco, tão necessárias na vida de um dependente químico.
📍 Reunião de 12 Passos:
✅ Reuniões ministradas com o objetivo de oferecer para as residentes, aprendizado e reflexão sobre os passos, princípios espirituais e toda a literatura de Narcóticos Anônimos.
📍 Laborterapia: (Terapia do Trabalho)
✅ Atividade realizada no período da manhã. Nossos objetivos com a Laborterapia,
além da “não ociosidade”, são inúmeros; por exemplo: Trabalhar os sentimentos (mágoa, orgulho, frustração, perda, raiva, amor, etc.);
✅ Descobrir e desenvolver habilidades;
✅ Elevar sua autoestima;
✅ Produzir, tendo a possibilidade de ver o fruto da produção;
✅ Aceitar limites e regras;
✅ Ter disciplina;
✅ Perceber suas responsabilidades;
✅ Assimilar a ajuda mútua;
✅ Desenvolver a percepção e a preocupação com o outro;
📍 Concentração e Atenção;
✅ Desenvolver noção de começo, meio e fim de uma atividade;
✅ Aprimoramento de conduta e caráter;
✅ Organização;
✅ Reabilitação física;
✅ Entre outros.
* Os trabalhos são executados em grupos, divididos.
📍 TRE – Terapia Racional Emotiva:
✅ São reuniões semanais que ensinam o dependente a como lidar com os sentimentos. Estudamos: A Raiva, A Vergonha, Rei Bebê, O Luto, Pensamento Destrutivo e outros temas.
Estes estudos são muito importantes na recuperação.
📍 P.P.R – Programa de prevenção a recaída:
✅ Essa reunião é muito importante, mostramos para os residentes algumas ferramentas que devem ser utilizadas após o período de internação. São os “EVITES E OS PROCURES”.
EX: PROCURE um hobby, ir à sala de anônimos, uma religião, bom novas amizades, etc. EVITE velhos amigos, velhos hábitos, velhas ideias, etc.
A recuperação começa na internação e continua a vida toda, oferecemos ferramentas para que nossos pacientes consigam viver em sobriedade e aprendendo a viver um dia de cada vez. Só por hoje funciona na prática.
Junior Alcantara CRT/FEMOTERBR 0384/21
wa.me/5511934328043
@institutoalcantaras
#dependenciaquimica #clinicaterapeutica #soporhohe #clinicaderecuperacao #clinicadereabilitacao #sph #juntossomosmaisfortes #crack #cocaina #k2 #k9 #maconha #alcool #alcoolismoédoença #saudemental #soporhojefunciona #Deusnocomando #aa #na #sp"

### Títulos do link nos anúncios
- CLÍNICA DE REABILITAÇÃO

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 016
anunciante: "Eujeannribeiro"
url_destino: "https://www.facebook.com/61590459793840/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1105077948719754"
dias_ativo: 40
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tse, tjaa"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno, Questões / simulados"
formatos_dos_anuncios: "imagem (1)"
botoes: "sem botão (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Lançados em agosto de 2026
Última resolução Pós-edital TSE Unificado Todas as resoluções Na prova: 91% bruto - 82% líquido
16º lugar /RN TJAA Poucas questões resolvidas, mas fechando bem as lacunas de conhecimento. A prova refletiu exatamente como estava no Tec. Não precisei de PDF longo, videoaulas imensas, só questões e um docx Revisava de forma simples e sem firulas A nomeação vem!"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 017
anunciante: "Tribunal Regional Eleitoral de Santa Catarina"
url_destino: "https://linktr.ee/tribunalregionaleleitoraldesc?utm_source=linktree_profile_share&ltsid=493740a3-46c0-4ab3-b13d-7834ee719d97&utm_medium=social&utm_content=link_in_bio&fbclid=PAcGRvZgJleHRuA2FlbQIxMQBzcnRjBmFwcF9pZA85MzY2MTk3NDMzOTI0NTkAAae8-tmV39LZcelWqAv6pVt8Py2ghpelAMJXxevZCLdJZbbKTjJJBliiSX0AAw_aem_vgmFFLWuAa6EgoVKyI-qVQ"
ad_library_url: "https://www.facebook.com/ads/library/?id=1073809275368257"
dias_ativo: 20
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tribunal regional eleitoral"
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
"Categorias
Tamanho estimado do público:
50 mil a 100 mil
Valor gasto (BRL):
R$200 a R$299
450 mil a 500 mil
Patrocinado • Pago por Tribunal Regional Eleitoral de Santa Catarina
✍️ Tem uma ideia sobre democracia, diálogo e respeito que merece ser ouvida?
Estudantes do ensino médio de escolas públicas e privadas de Santa Catarina podem participar do IV Concurso de Redação da EJESC, com o tema “Diálogo e Paz: um caminho para a celebração da Democracia”.
🔗 Confira o edital, as regras e o texto-base na página da EJESC.
📲 Inscrições e envio das redações pela Plataforma de Educação a Distância da EJESC."

### Títulos do link nos anúncios
- @trescjusbr Official: TikTok, Instagram, X | Linktree

### Landing Page: Headline & Promessa Central
"@trescjusbr — To help keep our community authentic, we're showing information about accounts on Linktree."

### Seções da Landing Page (títulos, na ordem)
- Explore other Linktrees
- About this account
- More from Linktree

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 018
anunciante: "Advocacia para Concursos - Mattozo & Ribeiro"
url_destino: "https://www.facebook.com/100089931653062/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1934024137978229"
dias_ativo: 13
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "justica eleitoral"
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
id_oferta: 019
anunciante: "Escola Até a Aprovação Policiais"
url_destino: "https://www.facebook.com/eaapoliciais/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1837036453960474"
dias_ativo: 8
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tre"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno"
formatos_dos_anuncios: "vídeo (1)"
botoes: "sem botão (1)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Muita gente erra porque vive estudando só para o edital da vez.
Compra um curso de reta final, faz a prova, não passa e acha que precisa começar tudo do zero no próximo concurso.
Mas quem acumula aprovações entende uma coisa: existe uma espinha dorsal nos concursos de tribunais.
TJ, TRT, TRE e outras oportunidades têm uma base comum que pode ser construída com método, constância e direção.
Quando você para de estudar no improviso e começa a levar a preparação a sério, a aprovação deixa de ser uma tentativa isolada e passa a ser uma consequência.
Aproveite que a Escola Até a Aprovação está com as matrículas abertas e com R$ 500 de desconto.
Garanta sua vaga e dê o próximo passo rumo à aprovação. link na bio."

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

# Parte 2 — Ofertas adjacentes (75)

Apareceram nas buscas, mas não citam os termos do foco. Servem para comparar formatos e preços de outros nichos de concurso; algumas não são de concurso.

---
id_oferta: 020
anunciante: "Professor Fabiano Pereira"
url_destino: "https://aprovatte.com.br/mentoria-start90-2025/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2185573738667418"
dias_ativo: 17
anuncios_coletados: 5
anuncios_ativos_estimados: 14
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento"
formatos_dos_anuncios: "vídeo (5)"
botoes: "sem botão (5)"
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
id_oferta: 021
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
id_oferta: 022
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://www.facebook.com/simboraconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=436273172079349"
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
tipos_produto: "Material em PDF / apostila / caderno, Cronograma / plano de estudos"
formatos_dos_anuncios: "carrossel (5), vídeo (3), imagem (1)"
botoes: "Visitar perfil do Instagram (5), sem botão (4)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Talvez você já tenha escutado várias histórias assim:
“Demorei a passar, mas depois que veio a primeira aprovação, vieram várias... uma atrás da outra.”
Pois é, chega um momento em que a gente “aprende a estudar”. Você estabelece uma rotina, entende o que funciona para a sua realidade, encontra um método que consegue manter... e vai “pegando o jeito”. A partir daí, os resultados começam a aparecer.
E, nos concursos de Tribunais, temos ainda duas grandes vantagens:
👉 1. O núcleo de matérias é muito parecido entre os concursos.
Com algumas adaptações no ciclo/cronograma, você consegue fazer a prova de um Tribunal X, depois aproveitar boa parte da preparação para um Tribunal Y, e assim sucessivamente.
Eu nunca fui muito de conciliar vários concursos. Preferia aproveitar as oportunidades de forma sequencial: focava 100% em um e, depois da prova, aproveitava a bagagem construída e direcionava o foco para o próximo. E assim eu fui... aumentando minha maturidade nas disciplinas e ficando cada vez melhor nelas.
Mesmo que a aprovação não venha no primeiro concurso, essa bagagem não se perde. Pelo contrário: você já chega muito mais preparado que a maioria na próxima oportunidade.
Muita gente me pergunta o “segredo” para eu ter conseguido uma aprovação em 1º lugar e até gabaritar uma prova. Na prática, foi apenas a premiação por toda essa bagagem acumulada.
👉 2. As listas dos concursos de Tribunais costumam rodar bastante.
Muita gente que passa em boas posições também está fazendo outras provas e colocando o nome em outras listas.
A pessoa passa em um Tribunal e depois é chamada em outro mais perto de casa. Passa para Técnico e depois é chamada para Analista. Isso gera uma grande rotatividade.
Ex: dos 10 primeiros colocados no meu concurso do TRT-PI, a maioria já deixou o cargo por outro melhor ou mais perto de casa.
Por isso eu sempre reforço: coloque o seu nome na lista. E não precisa ser necessariamente no Top 10. A lista vai andando, pessoas vão saindo, novas vagas vão surgindo e, ao longo da validade do concurso, muita gente que já nem tinha esperança acaba sendo surpreendida com a convocação.
Faça a sua parte e deixe o tempo fazer a dele. =)"

### Ganchos das variações (1ª linha de cada anúncio)
- Talvez você já tenha escutado várias histórias assim:
- 📚 Conheça o Caderno do Aprovado e prepare-se em alto nível para os próximos concursos de tribunais.
- Comente PLANILHA para receber gratuitamente a minha planilha de conteúdo verticalizado indicando quais são os assuntos mais relevantes para estudar nesse período pré-edital.
- Lançados em fevereiro de 2025
- Lançados em janeiro de 2025
- Lançados em outubro de 2024

### Títulos do link nos anúncios
- Beto (José Humberto) - Caderno Do Aprovado - TRT/TST/TJ/MP (@cadernoaprovado) • Instagram photos and videos
- Simbora Concursos

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 023
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
id_oferta: 024
anunciante: "Matheus Santos - Eu concursado"
url_destino: "https://seraprovado.com/mentoria-matheussantos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1059387566661056"
dias_ativo: 72
anuncios_coletados: 5
anuncios_ativos_estimados: 5
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento"
formatos_dos_anuncios: "vídeo (5)"
botoes: "Ver detalhes (5)"
precos_exibidos_na_lp: "R$ 10.000,00 | R$ 8 | R$ 15 | 12x de R$ 249,28 | R$ 2497 | 12x de R$ 399,03 | R$ 3997"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
id_oferta: 025
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
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
id_oferta: 026
anunciante: "Estratégia Concursos"
url_destino: "https://www.facebook.com/EstrategiaConcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=977003848724493"
dias_ativo: 84
anuncios_coletados: 3
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "imagem (2), vídeo (1)"
botoes: "Saiba mais (2), sem botão (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"📢 O professor Herbert Almeida indica: vale a pena estudar para CGU e Tribunal de Contas da União!
Aproveite o melhor preço da Semana Nacional para começar agora mesmo e fortalecer a sua preparação. 🚀📚
🔗Clique no link da bio."

### Ganchos das variações (1ª linha de cada anúncio)
- Acesse aulas e materiais de estudo no Grupo de Estudos do TJ RR no Whatsapp.
- Acesse aulas e materiais de estudo no Grupo de Estudos do TCE AP no Whatsapp.
- 📢 O professor Herbert Almeida indica: vale a pena estudar para CGU e Tribunal de Contas da União!

### Títulos do link nos anúncios
- Grupo de Estudos TJ RR
- Grupo de Estudos TCE AP

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 027
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
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
id_oferta: 028
anunciante: "Pódio Tribunais"
url_destino: "https://cronosconcursos.com.br/tribunais/?utm_source=meta&utm_medium=ig-ads&utm_campaign=rmkt-tribunais"
ad_library_url: "https://www.facebook.com/ads/library/?id=770404689243103"
dias_ativo: 198
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Cronograma / plano de estudos"
formatos_dos_anuncios: "vídeo (3)"
botoes: "sem botão (3)"
precos_exibidos_na_lp: "3x de R$ 369,36 | R$ 1.035 | 6x de R$ 354,64 | R$ 1.890,31 | 12x de R$ 341,58 | R$ 3.302,70 | 3x de R$ 760,12 | R$ 2.130"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Você estuda 4, 5 ou até 6 horas por dia e sente que não sai do lugar?
Se esforço fosse o suficiente, você já estaria aprovado.
O problema não é a quantidade de horas, é a falta de direção.
Na Mentoria da Cronos Concursos, você recebe um cronograma semanal 100% individualizado, feito sob medida para sua rotina, suas dificuldades e o concurso que deseja.
Nossos alunos destacam a organização, a plataforma intuitiva e a estratégia focada no que realmente importa como os grandes diferenciais. E você aprende tudo isso diretamente com quem já esteve em seu lugar: Oficiais de Justiça!
👉 Você só precisa sentar e estudar o que já foi criado para você.
✅ Clique agora e conheça a mentoria que vai mudar sua rotina de estudos."

### Landing Page: Headline & Promessa Central
"Mentoria para Tribunais — Preparação especializada para concursos de Tribunais com método validado e professores aprovados nos concursos mais recentes."

### Seções da Landing Page (títulos, na ordem)
- Nossos Alunos Aprovados
- Maíra Azevedo
- Matheus Pereira
- Isabelle Pádua
- Elisa Batista
- Isabella Fracalossi
- Flávia Limmer
- Vitor Hugo
- Rennan Galindo
- Railson Oliveira
- Ricardo Portinoi
- Jamille Saloum
- Rafael Guardiani
- Germana Dantas
- Beatriz Lamartine
- Vídeos de Depoimentos
- Conteúdos em Destaque
- O que está incluso na mentoria?
- Cronogramas Personalizados
- Metas Direcionadas
- Estratégias Avançadas
- Técnicas de Revisão
- Atendimento Personalizado
- Materiais de Estudo
- Dicas de Concursados
- Análise de Editais
- Comunidade de Alunos
- Prints de Depoimentos
- Seu aliado para aprovação em concursos
- Curso do Zero até a Aprovação

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Discursiva / redação
- Mentoria
- Resumos
- Videoaulas


========================================

---
id_oferta: 029
anunciante: "Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24"
url_destino: "https://ataticadaaprovacao.com.br/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1685357465868904"
dias_ativo: 83
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
botoes: "sem botão (2), Saiba mais (1)"
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
- PRF: Flashcards Completos para Administrativo e Agente.
- Transparência da UE
- COMBO AUDITOR FISCAL | 39.988 FLASHCARDS

### Títulos do link nos anúncios
- Prepare-se para a Polícia Rodoviária Federal!
- BACEN Técnico: 12.570 flashcards organizados.
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
id_oferta: 030
anunciante: "Decorando a Lei Seca Cursos Para Concursos E OAB"
url_destino: "https://www.facebook.com/decorandoaleisecaconcursoseoab/"
ad_library_url: "https://www.facebook.com/ads/library/?id=3563184787172231"
dias_ativo: 57
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Questões / simulados, Lei seca / legislação, Discursiva / redação"
formatos_dos_anuncios: "carrossel (1), imagem (2)"
botoes: "Visitar perfil do Instagram (1), sem botão (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Carreiras Policiais"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"⚠️ Uma palavra pode mudar completamente o gabarito da questão.
Nos arts. 26 e 28 do Código Penal, a lógica é muito semelhante:
🟡 Inteiramente incapaz → pode haver isenção de pena.
🔵 Sem plena capacidade / não inteiramente capaz → a consequência é a redução da pena.
E é justamente nessa diferença que as bancas constroem a pegadinha.
No exemplo do art. 28, § 2º, a questão troca a redução da pena pela isenção prevista para outra hipótese.
No art. 26, ocorre a mesma armadilha: o agente não inteiramente capaz é semi-imputável, razão pela qual a pena pode ser reduzida — e não simplesmente afastada.
📌 Regra para memorizar:
inteiramente incapaz → isenta
capacidade reduzida → reduz a pena
Esse tipo de comparação ajuda a perceber não apenas o que a lei diz, mas como as bancas tentam distorcer sua redação na prova.
🏆 No Vade Mecum de Questões, você pode treinar a lei seca artigo por artigo e identificar as pegadinhas que mais aparecem nas questões."

### Ganchos das variações (1ª linha de cada anúncio)
- O art. 30 do Código Penal é daqueles dispositivos curtos, mas que a banca adora explorar em prova objetiva.
- ⚠️ Uma palavra pode mudar completamente o gabarito da questão.

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 031
anunciante: "Alan Matos"
url_destino: "https://concursotcdf.editorainovedigital.com/"
ad_library_url: "https://www.facebook.com/ads/library/?id=27845572378433570"
dias_ativo: 51
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "vídeo (3)"
botoes: "Saiba mais (3)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🔎 Mais segurança na revisão para quem vai encarar a prova do Tribunal de Contas do Distrito Federal.
Consulte 260 mapas visuais com todas as matérias do edital e saiba o que a banca costuma cobrar em cada tema.
Material 100% alinhado ao Edital 2026 e ao padrão certo/errado do Cebraspe.
Clique abaixo e conheçais"

### Títulos do link nos anúncios
- Mapa da Aprovação Concurso TCDF2026

### Landing Page: Headline & Promessa Central
"Mapa da Aprovação Concurso TCDF 2026 · 260 Mapas Ilustrados do Edital"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 032
anunciante: "Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24"
url_destino: "https://ataticadaaprovacao.com.br/combao/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1088210254181707"
dias_ativo: 29
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "kiwify"
ticket_principal: "R$ 297,90"
fonte_ticket: "checkout"
tipos_produto: "Material em PDF / apostila / caderno, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (1), carrossel (2)"
botoes: "sem botão (3)"
parcelas: "12x de R$ 30,81"
precos_exibidos_na_lp: "R$ 15 | R$ 25 | R$ 11 | R$ 27 | R$ 16 | R$ 13 | R$ 5"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Antes de perguntar no direct: as 5 objeções sobre o Combão, respondidas.
"Já tenho PDF demais." — O problema não é falta de material, é formato. Acumular não revisa. O resumo é pra reler: 1 tópico por página, 27 matérias.
"Resumo não dá profundidade." — Abre o sumário de Contabilidade: CPC por CPC, um tópico cada. Profundidade com critério não é volume sem filtro.
"Daqui a 6 meses desatualiza." — Toda edição sai com carimbo do mês e nota de "o que mudou". A revisão mensal faz parte do produto.
"E se eu não gostar?" — 7 dias de reembolso integral. Um e-mail resolve.
"R$ 297,90 é caro." — 12x de R$ 30,81 no cartão, ou R$ 11 por matéria, pra sempre: sem mensalidade, sem renovação, atualizações incluídas. Uma apostila avulsa de uma matéria custa mais e não atualiza nunca.
A sexta — "funciona mesmo?" — não respondo eu: o carrossel responde, com nome e cargo de quem já passou.
Ainda tem dúvida? Baixa a amostra gratuita — páginas reais, sem cadastro. E se já decidiu: cupom 15OFF no checkout.
See Details"

### Ganchos das variações (1ª linha de cada anúncio)
- Antes de perguntar no direct: as 5 objeções sobre o Combão, respondidas.
- 27 matérias escritas por um autor só, no mesmo padrão: 1 tópico por página, caixa Memorize, caixa Atenção e jurisprudência com número de julgado.
- Quem usa, aprova — frases reais de alunos, publicadas com autorização, do jeito que chegaram.

### Títulos do link nos anúncios
- Depoimentos reais de alunos

### Landing Page: Headline & Promessa Central
"Estude para concurso 2x mais rápido — 27 matérias — do Direito à AFO, Contabilidade e RLM · acesso vitalício"

### Seções da Landing Page (títulos, na ordem)
- Os resumos são para você que
- Você vai impulsionar seus estudos
- Didática
- Organização
- Memorização
- Quatro destaques, cada um com uma função na revisão
- Junto com os resumos, você leva 4 bônus
- Caderno de Lei Seca
- Caderno de Jurisprudência
- Caderno de Erros
- Guia de como estudar pra concurso público
- Todas as matérias. Um único combão.
- Combão Todas as Matérias
- Saia na frente da concorrência
- Agilidade nos estudos
- Memorize e Atenção
- Edições revisadas
- Jurisprudência na fonte
- Veja como é por dentro antes de comprar
- Nove questões. Tudo está na amostra.
- Concurseiros de verdade
- Perguntas frequentes
- O que está acontecendo nos concursos
- Saiu o edital
- No radar — vão sair
- Improbidade: STF conclui o julgamento das ADIs 7.156 e 7.236
- PEC da Segurança Pública tramita no Senado
- CPC 51 aprovado: o que muda na Contabilidade a partir de 2027
- Como montar um ciclo de estudos que cabe na sua rotina
- Revisão espaçada: o que revisar e quando

### Entregáveis / Formato (termos encontrados na LP)
- Caderno de erros
- Cronograma
- Discursiva / redação
- Mapas mentais
- PDF
- Resumos


========================================

---
id_oferta: 033
anunciante: "Grupo Revisamed"
url_destino: "https://mediccurso.com.br/medprovas-lp/?utm_medium=%7B%7Badset.name%7D%7D_-_%7B%7Bcampaign.name%7D%7D_-_FBads_-_%7B%7Bsite_source_name%7D%7D_%7B%7Bplacement%7D%7D_-_%7B%7Bad.name%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D&utm_source=FBads&utm_term=%7B%7Bsite_source_name%7D%7D_%7B%7Bplacement%7D%7D&utm_content=%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1751551852597957"
dias_ativo: 14
anuncios_coletados: 1
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 1
sinal_tracao: "fraco"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados"
formatos_dos_anuncios: "imagem (1)"
botoes: "Saiba mais (1)"
precos_exibidos_na_lp: "3x de R$ 198 | R$ 198 | 12x de R$ 131 | 6x de R$ 158 | R$ 158"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Conheça seus pontos fortes e saiba onde precisa evoluir.
Quando você treina com provas de Residência Médica, começa a enxergar com mais clareza o que já domina, e, principalmente, quais conteúdos ainda merecem atenção.
No MedProvas, você encontra provas de diferentes instituições e processos seletivos para transformar cada resolução em informação útil para o seu estudo.
Mais do que contar acertos, a proposta é usar o treino para tomar decisões melhores, o que revisar, onde investir e como direcionar as próximas horas de estudo.
Treine com MedProvas e chegue à prova sabendo melhor como está a sua preparação.
Clique em saiba mais."

### Landing Page: Headline & Promessa Central
"Banco de questões de residência médica , ENARE e ENAMED — 100 mil questões reais de provas anteriores , com gabarito e comentários em texto e em vídeo. Monte simulados por banca, por ano e por tema, e descubra onde você perde ponto antes que a prova descubra."

### Seções da Landing Page (títulos, na ordem)
- O que tem dentro do MedProvas
- Provas de residência médica na íntegra, comentadas e por simulado
- Provas completas
- Provas comentadas
- Simulados personalizados
- Busca avançada
- Inteligência artificial para questões
- Provas anteriores do ENARE, ENAMED e Revalida, banca por banca
- Revalida
- Provas das principais instituições do Brasil
- O MedProvas é para você que:
- O que os estudantes dizem do MedProvas
- Como o MedProvas ajuda na preparação
- Garantia de 7 dias grátis.
- Planos e valores do MedProvas
- Garantia de 7 dias em todos os planos
- Quer uma preparação completa para Residência Médica e ENAMED?
- Medic Curso R1

### Entregáveis / Formato (termos encontrados na LP)
- Mapas mentais
- PDF
- Questões comentadas
- Resumos
- Simulados
- Videoaulas


========================================

---
id_oferta: 034
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

## Demais adjacentes (resumo)

| id | Anunciante | Dias | Anúncios | Tração | Ticket (checkout) | Destino |
|---|---|---|---|---|---|---|
| 035 | Gustavo Nogueira - Aprovação Ágil | 8 | 3 | médio | Não confirmado | https://pages.aprovacaoagil.com.br/vsl/tjsp/v01 |
| 036 | Gustavo Nogueira - Aprovação Ágil | 8 | 3 | médio | Não confirmado | https://pages.aprovacaoagil.com.br/vsl/trt/v01 |
| 037 | Concursos Ceisc | 191 | 2 | médio | Não confirmado | https://ceisc.com.br/cursos/2067-concurso-tj-sp-club-oficial-de-justica?utm_sour |
| 038 | Pódio Tribunais | 171 | 2 | médio | Não confirmado | https://api.whatsapp.com/send |
| 039 | Felipe Sgarbossa Advocacia Criminal | 166 | 2 | médio | Não confirmado | https://www.facebook.com/felipesgarbossa/ |
| 040 | Prof.carlosgoncalves | 121 | 2 | médio | Não confirmado | https://typebot.co/plataformaanalistadetribunais |
| 041 | Tjteiros | 97 | 2 | médio | Não confirmado | https://www.facebook.com/61582438800580/ |
| 042 | Central de Concursos | 86 | 2 | médio | Não confirmado | https://centraldeconcursos.com.br/concursos/concurso-tj-sp-escrevente?utm_source |
| 043 | Venâncio & Delgado - Advogados | 58 | 2 | médio | Não confirmado | https://api.whatsapp.com/send |
| 044 | Venâncio & Delgado - Advogados | 58 | 2 | médio | Não confirmado | https://www.facebook.com/venancioedelgadoadvogados/ |
| 045 | Concursos Ceisc | 51 | 2 | médio | Não confirmado | https://ceisc.com.br/cursos/2089-concurso-trt-4-club-analista-judiciario-area-ju |
| 046 | Serviço Social para Concursos | 29 | 2 | médio | R$ 837,00 | https://ssparaconcursos.com.br/clube-assistente-social-sociojuridico/?utm_source |
| 047 | Tucuju Bizurado Concursos | 17 | 2 | médio | Não confirmado | https://pay.plataformatutory.com.br/checkout/e5143ac2-626f-4616-9ab0-f146202578c |
| 048 | Victor Ribeiro | 10 | 2 | médio | Não confirmado | https://fureafila.com.br/comomemorizartudo/ |
| 049 | Prof. Ronaldo Santos | 8 | 2 | médio | Não confirmado | https://rslinguaportuguesa.com/aplicacao-fgv/?utm_source=facebook&utm_medium=cpc |
| 050 | Escola Flamengo - Unid Santos | 205 | 1 | médio | Não confirmado | https://www.facebook.com/61573410848498/ |
| 051 | Concursos Ceisc | 191 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2070-concurso-tj-ba-analista-judiciario-area-judicia |
| 052 | Gaby no Tribunal | 175 | 1 | médio | Não confirmado | https://www.facebook.com/100090566482087/ |
| 053 | Discursiva na Prática | 126 | 1 | médio | R$ 1.489,00 | https://discursivanapratica.com.br/assinaturacontrole/?utm_source=facebook&utm_m |
| 054 | Douglas Prado - Servidor 30k | 103 | 1 | médio | Não confirmado | https://odouglasprado.com.br/plano-servidor-30k/ |
| 055 | Rafael Amaral Adv | 94 | 1 | médio | Não confirmado | https://www.facebook.com/cleytonrafaelamaral/ |
| 056 | Fauth e Freitas Sociedade de Advogados com Adriane Fauth | 92 | 1 | médio | Não confirmado | https://www.facebook.com/61573224123970/ |
| 057 | nomaderachel com Focus Concursos Públicos | 83 | 1 | médio | Não confirmado | https://focusconcursos.com.br/ |
| 058 | Ludy Sena | 83 | 1 | médio | Não confirmado | https://www.facebook.com/ludysena.perita/ |
| 059 | Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24 | 78 | 1 | médio | Não confirmado | https://metastatus.com/ads-transparency |
| 060 | LH no pódio | 77 | 1 | médio | Não confirmado | https://typebot.co/mentoria-zeroaopodio |
| 061 | Gazeta dos Concursos | 76 | 1 | médio | Não confirmado | https://lp.aprovacaoagil.com.br/vsl-white-trt-noticia |
| 062 | Trteiros | 72 | 1 | médio | Não confirmado | https://www.facebook.com/61560675890210/ |
| 063 | Mege | 66 | 1 | médio | Não confirmado | https://concurcity.mege.com.br/explorar |
| 064 | Caderno do Aprovado - Materiais para Concursos | 65 | 1 | médio | R$ 497,00 | https://cadernodoaprovado.com/trf-tj-mp/ |
| 065 | Themas Cartórios | 64 | 1 | médio | Não confirmado | http://www.themas.com.br/ |
| 066 | Concurseiro Fora da Caixa | 57 | 1 | médio | Não confirmado | https://concurseiroforadacaixa.com.br/collections/todos-os-materiais |
| 067 | Bruna Vieira | 56 | 1 | médio | Não confirmado | https://5k.taciotj.online/ |
| 068 | Professora Amanda Aires | 54 | 1 | médio | Não confirmado | https://www.amandaaires.com.br/curso/%5B2026%5D-economia-para-o-tcu/345 |
| 069 | Rô Santtana - OAB | 51 | 1 | médio | Não confirmado | https://rosanttana.com.br/captacao/lp-discursiva-oab.html |
| 070 | Concursos Ceisc | 50 | 1 | médio | Não confirmado | https://www.sympla.com.br/produtor/ceisc |
| 071 | IPOG Salvador | 49 | 1 | médio | Não confirmado | https://ipog.edu.br/cursos/pos-graduacao/psicologia-juridica-com-enfase-em-peric |
| 072 | Nomade Rachel com Focus Concursos Públicos | 48 | 1 | médio | Não confirmado | https://focusconcursos.com.br:443/ |
| 073 | Progresso Concursos | 37 | 1 | médio | Não confirmado | https://progressoconcursos.com.br/produto/resumo-bizurado-do-que-mais-cai-em-pro |
| 074 | Concursos Ceisc | 27 | 1 | médio | Não confirmado | https://lp.ceisc.com.br/material-concurso-trt-4-projeto-nomeacao/ |
| 075 | Treinar na Oficina | 27 | 1 | médio | Não confirmado | https://www.facebook.com/61575606707746/ |
| 076 | Treinar na Oficina | 27 | 1 | médio | Não confirmado | https://www.ev8auto.com.br/osciloscopio-e-multimetro |
| 077 | Elevato Brasil Cursos e Treinamentos | 27 | 1 | médio | Não confirmado | https://www.facebook.com/brunovanuciseg/ |
| 078 | Centro Brasileiro de Ginástica Olímpica | 25 | 1 | médio | Não confirmado | http://fb.me/ |
| 079 | _rrautomoveis_ | 24 | 1 | médio | Não confirmado | https://rrautomoveis1.com.br/ |
| 080 | Local Imóveis Alto de Pinheiros | 17 | 1 | médio | Não confirmado | http://fb.me/ |
| 081 | Fas Lex Treinamentos E Licitações Ltda | 13 | 1 | médio | Não confirmado | https://escalla.pro/ |
| 082 | UniEVANGÉLICA | 10 | 1 | médio | Não confirmado | https://selecao.unievangelica.edu.br/direito |
| 083 | Método Supera.con | 10 | 1 | médio | Não confirmado | https://www.facebook.com/61555198180484/ |
| 084 | aprovados.dpero2025 | 10 | 1 | médio | Não confirmado | https://imediato.ncnews.com.br/2026/07/10/aprovados-em-concurso-da-dpe-ro-denunc |
| 085 | Malditafcc | 9 | 1 | médio | Não confirmado | https://www.facebook.com/malditafcc/ |
| 086 | IF Tecnologia | 9 | 1 | médio | Não confirmado | https://meuestudo-concursos.netlify.app/?utm_source=instagram&utm_medium=turbina |
| 087 | Portal & OAB | 8 | 1 | médio | Não confirmado | https://olympus.cursosdoportal.com.br/o-mil-smtt-aracaju/?utm_source=%7B%7Bsite_ |
| 088 | Professor Raphael Reis | 8 | 1 | médio | Não confirmado | https://www.facebook.com/profraphaelreis/ |
| 089 | Unipds | 8 | 1 | médio | Não confirmado | https://unipds.com.br/unipds-ia-funil/#hero |
| 090 | Migalhas | 8 | 1 | médio | Não confirmado | https://eventos.migalhas.com.br/evento/738/namoro-qualificado-e-uniao-estavel-ca |
| 091 | Professor Raphael Reis | 8 | 1 | médio | Não confirmado | https://www.professorraphaelreis.com.br/ |
| 092 | Tese Concursos | 8 | 1 | médio | Não confirmado | https://www.facebook.com/TESECONCURSOS/ |
| 093 | Curso Ênfase | 8 | 1 | médio | Não confirmado | https://www.facebook.com/cursoenfase/ |
| 094 | Sensei da Aprovação - Concursos Públicos | 8 | 1 | médio | Não confirmado | https://senseidaaprovacao.com.br/projetosenseicuritiba |

# Apêndice — Descartadas por não citarem concurso (55)

Vieram nas buscas (ex.: escritórios que citam o TRF como tribunal), mas o texto não tem nenhum termo de concurso. Confira se algo relevante caiu aqui por engano.

| Anunciante | Dias | Destino |
|---|---|---|
| mauroautomoveisrj | 224 | https://www.facebook.com/mauroautomoveisrj/ |
| DARKNESS NATION | 16 | https://www.darkness.com.br/melhor-pre-treino-evora-xt/p?sabor=Orange%20Storm&ta |
| Rita Bervig | 178 | https://www.facebook.com/100091834883862/ |
| Pablo | 19 | https://pablochaer.com.br/treinamento/?utm_source=%7B%7Bplacement%7D%7D&utm_medi |
| Scientific Research & Co - Pelve | 8 | https://scientificresearch.com.br/incontinencia-urinaria/ |
| Aquática American Park | 110 | https://sobre.aquaticaamericanpark.com.br/eventos |
| Emais | 16 | https://emais.com/terrenos/eplenum-reserve?utm_source=meta-ads&utm_medium=cpc&ut |
| Editora Mizuno | 252 | https://www.editoramizuno.com.br/ |
| Mega Loja Do Bras - Casa Branca | 126 | https://www.facebook.com/61554214040361/ |
| Cetrus - Educação Médica | 99 | http://fb.me/ |
| Heraclio Cunha | 51 | https://peritoem7dias.com.br/ |
| Kadosh Comunicação Visual | 27 | https://www.facebook.com/kadoshcomvisual/ |
| FlipWash | 24 | https://www.facebook.com/flipwash/ |
| Vitafor Nutrientes com Vitafor Science | 15 | https://www.facebook.com/vitafor/ |
| DARKNESS NATION | 15 | https://www.darkness.com.br/pre-treino |
| Good Shape Rj | 8 | https://www.facebook.com/goodshaperj25/ |
| Tribunal Regional Eleitoral de Mato Grosso | 412 | https://www.facebook.com/tremtoficial/ |
| Jeean Bernardes Estética Avançada | 284 | https://www.facebook.com/jeeanbernardes/ |
| Loja do Mecânico | 183 | https://www.facebook.com/lojadomecanico/ |
| Danielle Bartoly | 170 | https://www.facebook.com/61577922862090/ |
| Douglas Prado - Servidor 30k com Servidores High Level | 124 | https://www.facebook.com/professorlucrativo/ |
| REDI Acoustics | 113 | https://app.rediacoustics.com/ |
| Fibra Pará | 94 | https://www.facebook.com/fibrapara/ |
| Farmácias Farmassim | 90 | https://www.facebook.com/farmassim/ |
| Ana Fonseca Saúde Feminina | 78 | https://www.facebook.com/anafonsecasaudefeminina/ |
| Scientific Research & Co - Pelve | 66 | https://scientificresearch.com.br/curso-avancado-de-hiperplasia-prostatica-benig |
| Gel Mudanças e Transportes | 65 | https://www.facebook.com/61577458875831/ |
| Aquática American Park | 64 | https://www.facebook.com/aquaticaamericanpark/ |
| Academia Pinheiros | 60 | https://academiapinheiros.site/academia-pinheiros/ |
| Marcelo Mansano de Moraes | 59 | http://fb.me/ |
| RAIR Silva | 57 | https://www.facebook.com/jornalistarairsilva/ |
| Viégas Filho | 57 | https://www.facebook.com/100094050184913/ |
| thainara.assistentesocial | 55 | https://www.instagram.com/_u/thainara.assistentesocial |
| Gabriela Franco | 52 | https://www.facebook.com/61575028750782/ |
| Closet da BK | 51 | https://www.facebook.com/61556917691160/ |
| Go Kursos | 50 | https://www.gokursos.com/go-oab---direito-penal---2%C2%AA-fase-30553/p |
| Strong Car Services | 36 | https://www.facebook.com/strongcarservices/ |
| Expressa Veículos | 29 | https://www.facebook.com/expressaveiculos/ |
| Alibaba.com | 29 | https://www.alibaba.com/product-detail/haoge_11000005855956.html?src=cpm_fb&sub_ |
| Cetrus Grupo | 22 | http://fb.me/ |
| maskmaisoficial | 22 | https://www.facebook.com/maskmaisoficial/ |
| Dr Daniel Kruschewsky | 18 | https://www.facebook.com/drdanielkruschewsky/ |
| Cross Life Veloso - Osasco | 14 | https://www.facebook.com/61559104595340/ |
| Tre Amici Pizza | 13 | https://app.cardapioweb.com/tre_amici_pizzaria_e_restaurante?s=pub |
| Simone Freitas Imóveis | 13 | https://www.facebook.com/simonefreitasimoveisvr/ |
| Cleidimar Sousa | 12 | https://aceleradordenomeacao.com.br/mentoria-em-grupo |
| Halohealth | 12 | https://www.halodevice.com.br/products/halo-band |
| Felipe Almeida | 10 | https://www.facebook.com/felipealmeidaseudividendo/ |
| dominio.esportes | 10 | https://www.grupostarfit.com.br/ |
| Previdas Saúde | 9 | https://provamedica3.previdas.com.br/?src=&utm_source=meta&utm_medium=%7B%7Badse |
| Elite Barber Shop | 9 | https://www.facebook.com/61574507885102/ |
| Farmácias Nissei | 8 | https://www.farmaciasnissei.com.br/lam-quinzena-outubro-cabelos |
| Sungrow | 8 | https://www.facebook.com/CleanPowerForAll/ |
| Beatriz Queiroz Semijóias | 8 | https://www.facebook.com/61579067742432/ |
| Equipe Jacqueline Lima | 8 | https://www.facebook.com/equipejacquelinelima/ |
