# Dossiê ConcursoRadar — Justiça Eleitoral — TRE / TSE (10/10/2026)

## Métricas da Rodada
- **Buscas na Meta Ad Library:** `concurso TRE`, `tribunal regional eleitoral`, `concurso TSE unificado`, `justiça eleitoral concurso`, `técnico judiciário`, `TRE SP`, `TRE RJ`, `TRE MG`, `TSE unificado`, `concurso tribunal`
- **Filtro:** anúncios ativos no Brasil, no ar há 7+ dias (coleta ampla para achar padrões; a longevidade é analisada nas tabelas)
- **Ofertas do nicho:** 104 (de 227 anúncios; agrupadas por anunciante + página de destino)
- **Descartadas por não citarem concurso:** 74 (listadas no fim para auditoria)
- **Ofertas de foco direto:** 29 | adjacentes: 75
- **Sinal de tração:** 4 forte, 2 fraco, 98 médio
- **Landing pages lidas:** 68 de 104
- **Ticket confirmado no checkout:** 16 de 19 ofertas com checkout detectado (84%)
- **Tempo de processamento:** 703 segundos

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

Base: **227 anúncios de 81 anunciantes**; 110 estão no ar há 45+ dias (veteranos); mediana de 32 dias.

Como ler: **Anunciantes** = quantos produtores distintos usam (popularidade). **Veteranos** = quantos desses anúncios estão no ar há 45+ dias, e **% dos veteranos** = a fatia da categoria entre todos os veteranos. Se a fatia entre veteranos é maior que a fatia geral (% anúncios), a categoria aparece mais entre os que duram. Categoria com 1 ou 2 anunciantes é só um caso isolado.

A coleta junta duas amostras por busca (anúncios com 7+ dias e anúncios com 45+ dias), então a proporção de veteranos no total não é uma taxa de sobrevivência.

## Formato do criativo

Vídeo, imagem única ou carrossel.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| vídeo | 39 | 48% | 110 | 48% | 39 | 55 | 50% |
| imagem | 32 | 40% | 78 | 34% | 38 | 39 | 35% |
| carrossel | 25 | 31% | 39 | 17% | 30 | 16 | 15% |

## Proporção do criativo

Vertical (4:5 ou 9:16), quadrada (1:1) ou horizontal.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| vídeo vertical | 37 | 46% | 107 | 47% | 46 | 54 | 49% |
| imagem vertical | 29 | 36% | 65 | 29% | 25 | 28 | 25% |
| carrossel vertical | 22 | 27% | 32 | 14% | 43 | 16 | 15% |
| imagem quadrada | 5 | 6% | 13 | 6% | 59 | 11 | 10% |
| carrossel quadrada | 5 | 6% | 7 | 3% | 10 | 0 | 0% |
| vídeo quadrada | 2 | 2% | 3 | 1% | 8 | 1 | 1% |

## Duração dos vídeos

Só anúncios em vídeo.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| 31s a 1min | 17 | 44% | 59 | 54% | 19 | 27 | 49% |
| 1 a 2min | 16 | 41% | 23 | 21% | 59 | 14 | 25% |
| Até 30s | 8 | 21% | 20 | 18% | 10 | 8 | 15% |
| Mais de 2min | 7 | 18% | 8 | 7% | 68 | 6 | 11% |

## Botão (CTA)

Rótulo do botão exibido no anúncio.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| sem botão | 37 | 46% | 95 | 42% | 10 | 34 | 31% |
| Saiba mais | 33 | 41% | 67 | 30% | 54 | 42 | 38% |
| Ver detalhes | 13 | 16% | 32 | 14% | 56 | 20 | 18% |
| Visitar perfil do Instagram | 11 | 14% | 17 | 7% | 47 | 9 | 8% |
| Enviar mensagem pelo WhatsApp | 5 | 6% | 5 | 2% | 29 | 2 | 2% |
| Comprar agora | 4 | 5% | 6 | 3% | 8 | 1 | 1% |
| Solicitar agora | 2 | 2% | 2 | 1% | 49 | 1 | 1% |
| Enviar mensagem | 1 | 1% | 1 | 0% | 29 | 0 | 0% |
| Fale conosco | 1 | 1% | 1 | 0% | 29 | 0 | 0% |
| Inscreva-se | 1 | 1% | 1 | 0% | 89 | 1 | 1% |

## Destino do clique

Para onde o anúncio leva.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Página própria (LP / site) | 53 | 65% | 150 | 66% | 42 | 75 | 68% |
| Página / formulário no Facebook | 30 | 37% | 68 | 30% | 17 | 28 | 25% |
| WhatsApp | 4 | 5% | 6 | 3% | 93 | 6 | 5% |
| Checkout direto | 2 | 2% | 3 | 1% | 8 | 1 | 1% |

## Tamanho da copy

Texto principal do anúncio.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Média (200 a 600) | 45 | 56% | 96 | 42% | 53 | 61 | 55% |
| Longa (mais de 600) | 40 | 49% | 105 | 46% | 29 | 47 | 43% |
| Curta (até 200 caracteres) | 8 | 10% | 26 | 11% | 8 | 2 | 2% |

## Tipo de gancho (1ª linha da copy)

Classificação por palavras-chave; um gancho pode cair em mais de um tipo.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos | Exemplo |
|---|---|---|---|---|---|---|---|---|
| Outro | 38 | 47% | 74 | 33% | 47 | 38 | 35% | 🔥 A sua aprovação em Concursos Públicos não depende dos Materiais! Depende de direcionamento correto. — Gustavo Dias |
| Notícia de concurso / edital | 31 | 38% | 80 | 35% | 8 | 22 | 20% | Saiu o edital do TRT 8 — comece sua preparação agora — Thállius Moraes com Esquadrão de Elite |
| Pergunta | 18 | 22% | 39 | 17% | 60 | 23 | 21% | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? — Isaque Concursos |
| Chamada direta ao público | 10 | 12% | 17 | 7% | 19 | 7 | 6% | O TJ-SP Escrevente é uma grande oportunidade para quem busca estabilidade e carreira pública com nível médio. — Central de Concursos |
| Dor / erro do candidato | 9 | 11% | 15 | 7% | 66 | 8 | 7% | Você estuda 4, 5 ou até 6 horas por dia e sente que não sai do lugar? — Pódio Tribunais |
| Salário / estabilidade | 8 | 10% | 18 | 8% | 8 | 8 | 7% | O TJ-SP Escrevente é uma grande oportunidade para quem busca estabilidade e carreira pública com nível médio. — Central de Concursos |
| Oferta / desconto / urgência | 8 | 10% | 17 | 7% | 78 | 15 | 14% | 🎉 Desconto Exclusivo para Você! 🎉 — Editora Solução |
| Prova social / autoridade | 7 | 9% | 14 | 6% | 60 | 11 | 10% | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? — Isaque Concursos |
| Número / lista | 6 | 7% | 8 | 4% | 94 | 5 | 5% | Você estuda 4, 5 ou até 6 horas por dia e sente que não sai do lugar? — Pódio Tribunais |
| Promessa de método | 4 | 5% | 14 | 6% | 60 | 13 | 12% | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? — Isaque Concursos |
| Contraintuitivo / inimigo comum | 2 | 2% | 2 | 1% | 502 | 2 | 2% | A matéria para concurso já é grande e os cursinhos ainda complicam mais: centenas de horas de videoaulas e milhares de páginas de PDFs. — Caderno do Aprovado - Materiais para Concursos |

## Elementos da copy

Recursos presentes no texto; não são excludentes.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Usa emojis | 52 | 64% | 125 | 55% | 53 | 74 | 67% |
| Cita valor em R$ | 29 | 36% | 66 | 29% | 8 | 13 | 12% |
| Lista com marcadores (✔, ✅, •) | 23 | 28% | 59 | 26% | 39 | 29 | 26% |
| Hashtags | 14 | 17% | 27 | 12% | 60 | 16 | 15% |
| Gancho em CAIXA ALTA | 11 | 14% | 14 | 6% | 8 | 3 | 3% |
| Link ou 'link na bio' no texto | 7 | 9% | 12 | 5% | 59 | 8 | 7% |
| Cita bônus | 5 | 6% | 12 | 5% | 57 | 9 | 8% |
| Cita garantia | 4 | 5% | 5 | 2% | 87 | 3 | 3% |

## Sinais de público (ICP) citados na copy

Quem o anúncio diz atender, por palavras-chave. Indica a quem o mercado fala, não quem compra.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos | Exemplo |
|---|---|---|---|---|---|---|---|---|
| Motivado por salário / estabilidade | 33 | 41% | 82 | 36% | 10 | 28 | 25% | 💰 Concursos com salários de até R$20.000 estão ao seu alcance — mas você precisa do caminho certo. — Gustavo Dias |
| Esquece o que estuda / revisão | 14 | 17% | 32 | 14% | 35 | 15 | 14% | Mais do que contar acertos, a proposta é usar o treino para tomar decisões melhores, o que revisar, onde investir e como direcionar as próximas horas de estudo. — Grupo Revisamed |
| Pré-edital / sair na frente | 12 | 15% | 23 | 10% | 47 | 13 | 12% | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. — Tjteiros |
| Reta final / pós-edital | 12 | 15% | 21 | 9% | 8 | 6 | 5% | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. — Tjteiros |
| Trabalha / tem pouco tempo | 11 | 14% | 34 | 15% | 60 | 25 | 23% | Durante essa jornada de estudos, eu estudava de 2h a 3h por dia, já que estudava e trabalhava como CLT. — Isaque Concursos |
| Nível médio | 11 | 14% | 22 | 10% | 60 | 17 | 15% | Para você ter uma ideia, eu só me formei no ensino médio por meio do ENCCEJA, já que tinha repetido em todas as matérias. — Isaque Concursos |
| Dificuldade em discursiva / redação | 10 | 12% | 17 | 7% | 31 | 8 | 7% | O edital do TRT 8 (PA/AP) foi publicado. Prepare-se para Analista e Técnico com um curso completo: videoaulas, questões, cronogramas, Lei Seca, redação e muito  — Thállius Moraes com Esquadrão de Elite |
| Nível superior / Direito | 9 | 11% | 20 | 9% | 8 | 4 | 4% | Trata-se de uma oportunidade de nível superior com MUITAS vagas, e uma remuneração inicial muito atrativa. — Concursos Ceisc |
| Começando do zero | 7 | 9% | 22 | 10% | 56 | 12 | 11% | • Esteja começando os estudos agora; — Isaque Concursos |
| Estuda há tempo e não passa | 7 | 9% | 14 | 6% | 66 | 11 | 10% | Lógico que na maioria das vezes estive no cenário de REPROVADO (que é o mais NORMAL) 😅😅😅 — Caderno do Aprovado - Materiais para Concursos |
| Mãe / família | 5 | 6% | 12 | 5% | 62 | 11 | 10% | Se isso não fosse o bastante, eu tive uma infância/adolescência bem difícil. Sou filho de ex -empregada doméstica e, por isso, não tínhamos condições financeira — Isaque Concursos |
| Perdido no excesso de conteúdo | 4 | 5% | 9 | 4% | 8 | 2 | 2% | Se você tá perdido sem saber como começar ou já estuda mas sente que não evolui, está correndo um sério risco de ficar anos sem a sua aprovação. — Gustavo Dias |
| Erra questões / pegadinhas da banca | 3 | 4% | 5 | 2% | 49 | 3 | 3% | Não tem pegadinha, esse preparatório é gratuito. — Ceisc Concursos |

## Tipo de produto × ticket

Tipo identificado por palavras-chave na copy, no título do link e na headline (uma oferta pode ter vários). Ticket só entra quando foi lido no checkout.

| Tipo de produto | Anunciantes | Ofertas | Veteranas | Com ticket lido | Mínimo | Mediana | Máximo | Tickets lidos |
|---|---|---|---|---|---|---|---|---|
| Material em PDF / apostila / caderno | 40 | 44 | 26 | 5 | R$ 97 | R$ 397 | R$ 1.489 | Marcelomapas R$ 97; Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24 R$ 298; Brabo Editora R$ 397; Caderno do Aprovado - Materiais para Concursos R$ 497; Discursiva na Prática R$ 1.489 |
| Curso em videoaulas | 21 | 28 | 21 | 5 | R$ 247 | R$ 827 | R$ 6.346 | Thállius Moraes com Esquadrão de Elite R$ 247; Brabo Editora R$ 397; Instituto INAPI R$ 827; Discursiva na Prática R$ 1.489; Ceisc Concursos R$ 6.346 |
| Questões / simulados | 17 | 22 | 11 | 6 | R$ 58 | R$ 322 | R$ 837 | Aprovando Concurseiro R$ 58; Aprovando Concurseiro R$ 58; Thállius Moraes com Esquadrão de Elite R$ 247; Brabo Editora R$ 397; Instituto INAPI R$ 827; Serviço Social para Concursos R$ 837 |
| Isca gratuita / grupo VIP | 16 | 20 | 12 | 5 | R$ 298 | R$ 827 | R$ 6.346 | Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24 R$ 298; Isaque Concursos R$ 497; Instituto INAPI R$ 827; Jus Expert R$ 997; Ceisc Concursos R$ 6.346 |
| Cronograma / plano de estudos | 15 | 20 | 12 | 4 | R$ 247 | R$ 497 | R$ 837 | Thállius Moraes com Esquadrão de Elite R$ 247; Isaque Concursos R$ 497; Isaque Concursos R$ 497; Serviço Social para Concursos R$ 837 |
| Mentoria / acompanhamento | 13 | 15 | 11 | 3 | R$ 497 | R$ 497 | R$ 837 | Isaque Concursos R$ 497; Isaque Concursos R$ 497; Serviço Social para Concursos R$ 837 |
| Não identificado | 13 | 13 | 7 | 1 | R$ 397 | R$ 397 | R$ 397 | Decorando a Lei Seca Cursos Para Concursos E OAB R$ 397 |
| Lei seca / legislação | 11 | 13 | 6 | 5 | R$ 58 | R$ 97 | R$ 497 | Aprovando Concurseiro R$ 58; Aprovando Concurseiro R$ 58; Marcelomapas R$ 97; Thállius Moraes com Esquadrão de Elite R$ 247; Caderno do Aprovado - Materiais para Concursos R$ 497 |
| Discursiva / redação | 10 | 11 | 6 | 3 | R$ 247 | R$ 837 | R$ 1.489 | Thállius Moraes com Esquadrão de Elite R$ 247; Serviço Social para Concursos R$ 837; Discursiva na Prática R$ 1.489 |
| Mapas mentais / esquemas | 3 | 4 | 1 | 3 | R$ 97 | R$ 497 | R$ 837 | Marcelomapas R$ 97; Caderno do Aprovado - Materiais para Concursos R$ 497; Serviço Social para Concursos R$ 837 |
| Assinatura / clube / vitalício | 3 | 3 | 2 | 2 | R$ 837 | R$ 1.163 | R$ 1.489 | Serviço Social para Concursos R$ 837; Discursiva na Prática R$ 1.489 |
| Flashcards | 1 | 2 | 2 | 0 | — | — | — |  |

## Expressões repetidas entre anunciantes

Sequências de 2 ou 3 palavras (sem acento) usadas na copy por 3 ou mais anunciantes distintos.

`tecnico judiciario` (15), `clique em saiba` (12), `tribunal regional` (10), `tj sp` (10), `nivel superior` (9), `analista judiciario` (9), `tribunal de justica` (8), `8a regiao` (8), `regional do trabalho` (7), `r$ 16` (7), `nivel medio` (7), `garanta sua vaga` (7), `escrevente tecnico judiciario` (7), `ensino medio` (7), `novo concurso` (6), `edital publicado` (6), `agora mesmo` (6), `tribunal de contas` (5), `trabalho da 8a` (5), `see details` (5), `remuneracao inicial` (5), `r$ 16 040` (5), `pos edital` (5), `pode sair` (5), `pa ap` (5), `estudar agora` (5), `edital sair` (5), `concursos publicos` (5), `concursos de tribunais` (5), `concurso publico` (5)

## Arquivo de ganchos (anúncios mais replicados e mais antigos)

| Anunciante | Dias | Cópias | Formato | Botão | Gancho (1ª linha) | Título do link |
|---|---|---|---|---|---|---|
| Gustavo Dias | 8 | 10 | imagem | sem botão | 🔥 A sua aprovação em Concursos Públicos não depende dos Materiais! Depende de direcionamento correto. |  |
| Isaque Concursos | 64 | 4 | vídeo | sem botão | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? |  |
| Thállius Moraes com Esquadrão de Elite | 8 | 4 | imagem | sem botão | Saiu o edital do TRT 8 — comece sua preparação agora |  |
| Editora Solução | 134 | 3 | imagem | sem botão | 🎉 Desconto Exclusivo para Você! 🎉 |  |
| Central de Concursos | 79 | 3 | vídeo | sem botão | O TJ-SP Escrevente é uma grande oportunidade para quem busca estabilidade e carreira pública com nível médio. |  |
| Nova Concursos | 50 | 3 | imagem | sem botão | "📚🆓 Curso Grátis TJ-SP 2026 - Escrevente Técnico Judiciário! 🆓📚 |  |
| Gustavo Nogueira - Aprovação Ágil | 10 | 3 | vídeo | sem botão | Dá pra passar em escrevente sem ser do Direito? Dá. E não é porque a prova é fácil — é porque ela não te pede pra recitar a lei. |  |
| Tjteiros | 99 | 2 | vídeo | sem botão | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. |  |
| Brabo Concursos | 94 | 2 | vídeo | sem botão | O TJ-SP tem um novo concurso previsto para 2026, são mais de 3.300 cargos vagos de Escrevente Técnico Judiciário, temos contrato assinado com a banca organizadora e recentemente foram criados novas 720 vagas de Escrevent |  |
| Central de Concursos | 88 | 2 | vídeo | sem botão | O concurso do Tribunal de Justiça de São Paulo (TJ-SP) é uma das maiores oportunidades para quem tem apenas o ensino médio completo. Além de um excelente salário inicial, você conquista estabilidade financeira, benefício |  |
| Estratégia Concursos | 86 | 2 | vídeo | sem botão | 📢 O professor Herbert Almeida indica: vale a pena estudar para CGU e Tribunal de Contas da União! |  |
| Venâncio & Delgado - Advogados | 60 | 2 | vídeo | sem botão | ⚖️ A banca examinadora pode mudar de entendimento e te eliminar como PCD? Saiba o que o Superior Tribunal de Justiça (STJ) decidiu! |  |
| Lucas Viégas | 46 | 2 | vídeo | sem botão | Concurso TCE GO: Edital Publicado hoje! Provas em janeiro, como será a sua preparação até o dia da prova? |  |
| Serviço Social para Concursos | 31 | 2 | vídeo | sem botão | Quem quer uma vaga no sociojurídico sabe: não dá para estudar de qualquer jeito. |  |
| Tucuju Bizurado Concursos | 19 | 2 | carrossel | Saiba mais | Comente PC AMAPÁ e comece sua preparação agora!! | Checkout Tutory |
| Grupo Revisamed | 16 (baixo volume) | 2 | imagem | Saiba mais | Conheça seus pontos fortes e saiba onde precisa evoluir. |  |
| IDP - SP | 9 | 2 | imagem | Solicitar agora | Aprofunde sua pesquisa sobre Direito, Política e o funcionamento das instituições democráticas contemporâneas. |  |
| Isaque Concursos | 8 | 2 | vídeo | sem botão | ATENÇÃO! EDITAL PUBLICADO: TRT-8 (PA/AP) |  |
| Giovanna Carranza Desenvolvimento Profissional | 8 | 2 | imagem | sem botão | Concurso TRT8! |  |
| Sou Concurseiro | 8 | 2 | vídeo | sem botão | Acabou a faculdade ou vai se formar este ano? O concurso do TJ-AM pode ser o seu próximo passo. |  |
| Sou Concurseiro | 8 | 2 | vídeo | sem botão | Qualquer curso superior, salário acima de R$ 15 mil e jornada das 8h às 14h: esse é o concurso do TJ-AM. |  |
| Sou Concurseiro | 8 | 2 | vídeo | sem botão | Acha que já passou da idade para estudar? No TJ-AM tem gente de 30, 40 e 50 anos se preparando agora. |  |
| Sou Concurseiro | 8 | 2 | vídeo | sem botão | Mais de 30 ou 40 anos e ensino superior? Presta atenção no concurso do TJ-AM: 400 vagas e jornada das 8h às 14h. |  |
| Sou Concurseiro | 8 | 2 | vídeo | sem botão | Mais de 40 anos, ensino superior e vontade de mudar de carreira? Conheça o concurso do TJ-AM: 400 vagas. |  |
| Sou Concurseiro | 8 | 2 | vídeo | sem botão | Cada vez mais gente com 40, 50 anos está estudando para o TJ-AM: salário acima de R$ 15 mil e jornada das 8h às 14h. |  |
| Sou Concurseiro | 8 | 2 | vídeo | sem botão | Tem mais de 30, 40 ou 50 anos e já tem ensino superior? O Tribunal de Justiça do Amazonas pode ser a sua transição de carreira. |  |
| Caderno do Aprovado - Materiais para Concursos | 926 | 1 | imagem | sem botão | A matéria para concurso já é grande e os cursinhos ainda complicam mais: centenas de horas de videoaulas e milhares de páginas de PDFs. | Simbora Concursos |
| Simbora Concursos | 926 | 1 | carrossel | Visitar perfil do Instagram | Quando eu comecei a estudar para Tribunais, ficar "nas cabeças" era algo inimaginável... 1º lugar, então? Era coisa de maluco, extraterrestre, etc. |  |
| Caderno do Aprovado - Materiais para Concursos | 787 | 1 | carrossel | Visitar perfil do Instagram | Lançados em agosto de 2024 |  |
| Caderno do Aprovado - Materiais para Concursos | 729 | 1 | carrossel | Visitar perfil do Instagram | Lançados em outubro de 2024 |  |
| Caderno do Aprovado - Materiais para Concursos | 618 | 1 | vídeo | sem botão | Lançados em janeiro de 2025 |  |
| Caderno do Aprovado - Materiais para Concursos | 614 | 1 | carrossel | Visitar perfil do Instagram | Lançados em fevereiro de 2025 |  |
| Escola Flamengo - Unid Santos | 207 | 1 | imagem | Enviar mensagem pelo WhatsApp | Lançados em março de 2026 |  |
| Pódio Tribunais | 200 | 1 | vídeo | sem botão | Você estuda 4, 5 ou até 6 horas por dia e sente que não sai do lugar? |  |
| Concursos Ceisc | 193 | 1 | vídeo | Saiba mais | A sua preparação para o TJ-SP exige foco e direcionamento. |  |
| Concursos Ceisc | 193 | 1 | vídeo | Saiba mais | O edital do concurso do TJ-BA com o cargo de Analista Judiciário pode sair a qualquer momento, e o momento de estudar é agora. 🚀 |  |
| Gaby no Tribunal | 177 | 1 | carrossel | Visitar perfil do Instagram | Qual desses apps & sites você ainda não conhecia? Algum usa no seu dia a dia? Ah, se tiver uma outra indicação pode deixar nos comentários, amo descobrir novos kkkkk 💜 | Gaby Ungareli / TJSP (@gabynotribunal) • Instagram photos and videos |
| Felipe Sgarbossa Advocacia Criminal | 168 | 1 | vídeo | sem botão | 🗣️ Sustentação oral em Revisão Criminal envolvendo a correta delimitação das imputações e a aplicação do conceito de crime único no tráfico de drogas. |  |
| Estratégia Concursos | 156 | 1 | vídeo | Saiba mais | 🚀Pronto para o TJ SP? |  |
| Concursos Ceisc | 134 | 1 | vídeo | Ver detalhes | O Concurso para Escrevente Técnico Judiciário do Tribunal de Justiça de São Paulo deve ter seu edital publicado em 2026. | Aprove com Ceisc |

---

# Parte 1 — Ofertas de foco direto (29)

---
id_oferta: 001
anunciante: "Isaque Concursos"
url_destino: "https://projetotrt.com.br/imersao1v1/"
ad_library_url: "https://www.facebook.com/ads/library/?id=3249712645216747"
dias_ativo: 64
anuncios_coletados: 8
anuncios_ativos_estimados: 26
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "onprofit"
ticket_principal: "R$ 497,00"
fonte_ticket: "checkout"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (8)"
botoes: "sem botão (7), Saiba mais (1)"
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
anunciante: "Nova Concursos"
url_destino: "https://aprovacao.novaconcursos.com.br/curso-gratis-tj-sp-ads"
ad_library_url: "https://www.facebook.com/ads/library/?id=1058797666793436"
dias_ativo: 116
anuncios_coletados: 8
anuncios_ativos_estimados: 16
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Questões / simulados, Cronograma / plano de estudos, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (8)"
botoes: "Saiba mais (7), sem botão (1)"
precos_exibidos_na_lp: "R$ 297,00 | R$ 0,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 3
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
id_oferta: 003
anunciante: "Portal & OAB"
url_destino: "https://olympus.cursosdoportal.com.br/o-adm-trt-pa/?utm_source=%7B%7Bsite_source_name%7D%7D&utm_medium=%7B%7Badset.name%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D&utm_term=%7B%7Bplacement%7D%7D&utm_content=%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=2295062094681016"
dias_ativo: 12
anuncios_coletados: 13
anuncios_ativos_estimados: 13
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados, Cronograma / plano de estudos, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (5), imagem (8)"
botoes: "Ver detalhes (5), sem botão (8)"
precos_exibidos_na_lp: "R$ 9.776,71 | R$ 16.040,88"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
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
anunciante: "Ceisc Concursos"
url_destino: "https://lp.ceisc.com.br/projeto-nomeacao-tj-sp/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2095494471007965"
dias_ativo: 89
anuncios_coletados: 5
anuncios_ativos_estimados: 5
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "sympla"
ticket_principal: "R$ 6.345,94"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (5)"
botoes: "Ver detalhes (3), Solicitar agora (1), Inscreva-se (1)"
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
- Os cargos de Escrevente Técnico e Oficial de Justiça do Tribunal de Justiça de São Paulo exercem papéis essenciais para solucionar o alto volume de processos que tramitam na instituição.
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
id_oferta: 005
anunciante: "Thállius Moraes com Esquadrão de Elite"
url_destino: "https://lp.oesquadraodeelite.com.br/curso-intensivo-trt-8-reta-final"
ad_library_url: "https://www.facebook.com/ads/library/?id=1842940127056507"
dias_ativo: 8
anuncios_coletados: 2
anuncios_ativos_estimados: 5
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario, tjaa"
plataforma_checkout: "onprofit"
ticket_principal: "R$ 247,00"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Questões / simulados, Lei seca / legislação, Discursiva / redação, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (2)"
botoes: "sem botão (1), Ver detalhes (1)"
parcelas: "12x R$ 24,80"
precos_exibidos_na_lp: "R$ 13 | R$ 597,00 | R$ 247,00 | 12x de R$ 24,80"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 1
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
id_oferta: 006
anunciante: "MEQ Concursos"
url_destino: "https://www.facebook.com/61586241338760/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1684375369487437"
dias_ativo: 91
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
dias_distintos_coletado: 4
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
id_oferta: 007
anunciante: "Isaque Concursos"
url_destino: "https://projetotrt.com.br/vsl1v1/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1023281740551609"
dias_ativo: 64
anuncios_coletados: 4
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "onprofit"
ticket_principal: "R$ 497,00"
fonte_ticket: "checkout"
tipos_produto: "Mentoria / acompanhamento, Cronograma / plano de estudos"
formatos_dos_anuncios: "vídeo (4)"
botoes: "Saiba mais (4)"
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
- Tenha tudo que você precisa para estudar em alto nível para qualquer TRT do Brasil com o Projeto TRT🔥
- Tenha organização e direcionamento para

### Títulos do link nos anúncios
- Projeto TRT: Ecossistema Completo para TRTs
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
id_oferta: 008
anunciante: "Isaque Concursos"
url_destino: "https://projetotrt.com.br/trt8/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1562691092327193"
dias_ativo: 8
anuncios_coletados: 2
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "onprofit"
ticket_principal: "R$ 497,00"
fonte_ticket: "checkout"
tipos_produto: "Mentoria / acompanhamento, Cronograma / plano de estudos"
formatos_dos_anuncios: "vídeo (2)"
botoes: "sem botão (2)"
parcelas: "12x R$ 42,99"
precos_exibidos_na_lp: "R$ 9.776,71 | R$ 90,00 | R$ 11.928 | R$ 0 | R$ 997 | R$ 100 | R$ 497 | R$ 397"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 1
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
id_oferta: 009
anunciante: "Caderno Mapeado"
url_destino: "https://cadernomapeado.com.br/tce-ma-cmlm/?src=&utm_source=facebook-ads&utm_medium=%7B%7Badset.name%7D%7D&utm_content=%7B%7Bad.name%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D&utm_term=%7B%7Bplacement%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1718780919341886"
dias_ativo: 60
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
dias_distintos_coletado: 4
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
id_oferta: 010
anunciante: "Instituto INAPI"
url_destino: "https://cursos.inapionline.com.br/pre-trt-pi"
ad_library_url: "https://www.facebook.com/ads/library/?id=1054686240270707"
dias_ativo: 54
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
id_oferta: 011
anunciante: "Nova Concursos"
url_destino: "https://aprovacao.novaconcursos.com.br/curso-gratis-tj-sp-escrevente-ads-ca2"
ad_library_url: "https://www.facebook.com/ads/library/?id=2888791104852798"
dias_ativo: 50
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
id_oferta: 012
anunciante: "Hugo de Freitas"
url_destino: "https://www.facebook.com/hugoconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1567356078474323"
dias_ativo: 11
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "carrossel (3)"
botoes: "sem botão (2), Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
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
- SAIU O EDITAL DO TRT8!
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
anunciante: "Decorando a Lei Seca Cursos Para Concursos E OAB"
url_destino: "https://www.decorandoaleiseca.com.br/retafinal/analista-judiciario-area-judiciaria-trt-8-regiao"
ad_library_url: "https://www.facebook.com/ads/library/?id=1807015203847696"
dias_ativo: 8
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
dias_distintos_coletado: 1
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
id_oferta: 014
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2092-concurso-tj-sp-club-escrevente-tecnico-judiciario?utm_source=meta_ads&utm_medium=cpc&utm_campaign=vendas_tj_sp_escrevente"
ad_library_url: "https://www.facebook.com/ads/library/?id=864887869547603"
dias_ativo: 134
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
precos_exibidos_na_lp: "R$ 6 | R$ 6.345,94 | R$ 9.007,67 | R$ 1.797,00 | R$ 1.078,20 | 12x de R$ 89,85"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
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
id_oferta: 015
anunciante: "Concursosmeucurso"
url_destino: "https://meucurso.com.br/categorias/concursos-publicos-escrevente--tjsp"
ad_library_url: "https://www.facebook.com/ads/library/?id=941559835572125"
dias_ativo: 114
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
formatos_dos_anuncios: "carrossel (1), imagem (1)"
botoes: "Saiba mais (1), sem botão (1)"
precos_exibidos_na_lp: "R$ 1.899,00 | 12x de R$ 94,92 | R$ 1.139,00 | R$ 1.499,00 | 12x de R$ 58,67 | R$ 704,00 | R$ 999,50 | 12x de R$ 29,08"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 3
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
- Se você está esperando o edital ser publicado para começar a estudar, talvez esteja perdendo a melhor oportunidade de conquistar sua aprovação.
- Education

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
id_oferta: 016
anunciante: "Brabo Concursos"
url_destino: "https://www.facebook.com/braboconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=4583317258660193"
dias_ativo: 94
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
dias_distintos_coletado: 3
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
id_oferta: 017
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2138-concurso-trt-4-club-tecnico-judiciario-area-administrativa?utm_source=meta_ads&utm_medium=cpc&utm_campaign=vendas_trt_4_club_tec_judiciario&utm_term=advantage"
ad_library_url: "https://www.facebook.com/ads/library/?id=1020843757391368"
dias_ativo: 87
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
precos_exibidos_na_lp: "R$ 9 | R$ 9.776,71 | R$ 26.876,48 | R$ 9.007,67 | R$ 1.797,00 | R$ 1.168,05 | 12x de R$ 97,34"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 3
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
id_oferta: 018
anunciante: "Marcelomapas"
url_destino: "https://marcelomapas.com/tjsp/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1842212416642972"
dias_ativo: 9
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "kiwify"
ticket_principal: "R$ 97,00"
fonte_ticket: "checkout"
tipos_produto: "Material em PDF / apostila / caderno, Mapas mentais / esquemas, Lei seca / legislação"
formatos_dos_anuncios: "vídeo (2)"
botoes: "Saiba mais (2)"
parcelas: "12x de R$ 10,03"
precos_exibidos_na_lp: "R$ 133 | R$ 77 | R$ 56 | R$ 661 | R$ 47 | R$ 30 | R$ 871 | R$ 97"
primeira_coleta_propria: "2026-10-09"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Você estuda para o TJ-SP e sente que não sai do lugar? Talvez o problema seja o jeito que você está revisando! 📚⚖️
Com os Resumos Ilustrados para Escrevente Técnico Judiciário do TJ-SP, você revisa o conteúdo do último edital VUNESP de forma rápida, visual e estratégica — sem perder horas com PDFs enormes.
✅ 11 disciplinas: Português, Direito, Informática, RLM e mais
✅ Legislação Interna do TJSP (Regimento, NSCGJ, eproc)
✅ Resumos ilustrados e esquematizados
✅ Mapas mentais e quadros de revisão
✅ Foco no estilo de cobrança da VUNESP
📢 720 novos cargos criados + mais de 3.000 vagos: quem começa agora sai na frente!
👉 De R$871 por apenas R$97!
🚨 Promoção por tempo limitado. Garanta seu material enquanto a oferta estiver disponível!"

### Títulos do link nos anúncios
- 🔥 TJ-SP ESCREVENTE: DE R$871 POR APENAS R$97!

### Landing Page: Headline & Promessa Central
"Revise 5x mais rápido com os resumos ilustrados que te colocam na lista dos aprovados do concurso do TJSP. — O conteúdo cobrado na prova de Escrevente Técnico Judiciário do TJSP, organizado e simplificado em mapas mentais, esquemas e mnemônicos, em um único pacote."

### Seções da Landing Page (títulos, na ordem)
- Dentro do pacote, você vai receber…
- Facilidade
- Velocidade
- Estímulos
- O que mais vem junto com o material
- Liberado para impressão
- Atualizações gratuitas
- Em qualquer tela
- Arraste e veja: o mesmo artigo, dois formatos .
- Veja algumas das páginas que você vai receber
- O que cai na prova de Escrevente, bloco por bloco:
- O que dizem os alunos
- Receba também 2 bônus
- Macetes, Dicas e Mnemônicos
- Manual da Memorização
- Tudo isso, nessa oferta exclusiva
- Garanta seu acesso
- Receba no e-mail
- Abra e estude
- Mais de 6 anos ajudando milhares de estudantes a conquistar a aprovação
- Garantia incondicional de 7 dias
- Perguntas frequentes

### Seção "Para Quem NÃO É" (declarado na LP)
- Direito garantido pelo art. 49 do Código de Defesa do Consumidor. O pedido é feito direto pela Kiwify ou pelo nosso e-mail de suporte.

### Entregáveis / Formato (termos encontrados na LP)
- Mapas mentais
- PDF
- Resumos


========================================

---
id_oferta: 019
anunciante: "Site RP"
url_destino: "https://www.trt8.jus.br/noticias/2026/edital-para-concurso-publico-do-trt-8-e-publicado"
ad_library_url: "https://www.facebook.com/ads/library/?id=2510089052822709"
dias_ativo: 8
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
dias_distintos_coletado: 1
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
id_oferta: 020
anunciante: "cadernodoconcurseiro"
url_destino: "https://www.facebook.com/100064118526627/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1101272539160972"
dias_ativo: 8
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
dias_distintos_coletado: 1
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
id_oferta: 021
anunciante: "Simbora Concursos"
url_destino: "https://www.facebook.com/simboraconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=3157233831074462"
dias_ativo: 926
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
dias_distintos_coletado: 4
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
id_oferta: 022
anunciante: "Estratégia Concursos"
url_destino: "https://concursos.estrategia.com/concurso/tribunal-de-justica-do-estado-de-so-paulo/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1954755098733902"
dias_ativo: 156
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Assinatura / clube / vitalício, Material em PDF / apostila / caderno, Questões / simulados, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (1)"
botoes: "Saiba mais (1)"
precos_exibidos_na_lp: "12x de R$ 18,33 | 12x de R$ 12,83 | 12x de R$ 99,90 | 12x de R$ 20,17 | 12x de R$ 84,90 | 12x de R$ 74,90 | 12x de R$ 36,67 | 12x de R$ 30,00"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚀Pronto para o TJ SP?
🤔O maior Tribunal do país costuma surpreender com editais 'do nada'.
Não espere a concorrência sair na frente!
Com o 🦉Estratégia Concursos, você tem a preparação completa e antecipada que precisa: videoaulas, PDFs, questões e Trilha.
Aproveite as 💵condições especiais nos pacotes, garantia de 30 dias, acesso ilimitado até a prova e atualizações gratuitas!
Seus estudos estão seguros conosco.
Clique em SAIBA MAIS e comece agora com 30 dias de garantia! 🛡️
TJ SP: condições especiais nos pacotes completos por tempo limitado"

### Landing Page: Headline & Promessa Central
"Cursos para o Concurso TJ-SP: Escrevente Técnico Judiciário, Oficial de Justiça e Escrevente Técnico Judiciário (Capital e Interior) — Atualidades para TJ-SP (Escrevente Judiciário)"

### Seções da Landing Page (títulos, na ordem)
- Cursos para TJ-SP por cargo
- Pacote Completo para TJ-SP (Escrevente Técnico Judiciário) + Sistema de Questões
- Pacote Completo para TJ-SP (Escrevente Técnico Judiciário)
- Raciocínio Lógico e Matemática para TJ-SP (Escrevente Judiciário)
- Legislação Especial TJ-SP para TJ-SP (Escrevente Judiciário)
- Língua Portuguesa para TJ-SP (Escrevente Judiciário)
- Atualidades para TJ-SP (Escrevente Judiciário)
- Direito Processual Civil para TJ-SP (Escrevente Judiciário)
- Sobre o Concurso TJ-SP
- Disciplinas
- Como se preparar para o Concurso TJ-SP
- Compromisso de atualização pós-edital
- Estude com professores consagrados do mundo dos concursos
- Adriana Figueiredo
- Herbert Almeida
- Brunno Lima
- Adriane Fauth
- Policial Rodoviário federal: 952 aprovados nas 1.500 vagas (63%)
- 24 aprovados entre os 30 primeiros
- Agente, Escrivão e Papiloscopista: 977 aprovados dentro das 1.500 vagas.
- Os 1º, 2º e 3º colocados de Agente, Escrivão e Papiloscopista foram alunos do Estratégia.
- Agente: 497 alunos nas 898 vagas (55,34%)
- sendo 11 aprovados entre os 15 primeiros
- Papiloscopista: 51 aprovados nas 84 vagas (60,71%)
- sendo 3 aprovados entre os 3 primeiros.
- O que os aprovados andam dizendo por aí....
- Pacotes com conteúdo didático multimídia para acelerar a sua aprovação
- Livro Digital Interativo (LDI)
- Aulas em vídeo, PDF e Cast
- Questões e simulados

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Discursiva / redação
- Mapas mentais
- PDF
- Questões comentadas
- Resumos
- Simulados
- Videoaulas


========================================

---
id_oferta: 023
anunciante: "Junior Alcantara"
url_destino: "http://wa.me/5511934328043"
ad_library_url: "https://www.facebook.com/ads/library/?id=1425722342913421"
dias_ativo: 127
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
dias_distintos_coletado: 4
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
id_oferta: 024
anunciante: "Concursosmeucurso"
url_destino: "https://meucurso.com.br/cursos/concursos-publicos"
ad_library_url: "https://www.facebook.com/ads/library/?id=1542521100851019"
dias_ativo: 80
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tse, tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "carrossel (1)"
botoes: "Saiba mais (1)"
precos_exibidos_na_lp: "R$ 350 | R$ 699,00 | 12x de R$ 29,08 | R$ 349,00 | 12x de R$ 40,78 | R$ 489,30 | R$ 999,00 | 12x de R$ 66,58"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 3
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
- Procuradorias FCC | Resolução de Questões - online
- Procuradoria do Estado de São Paulo | Peças Práticas
- Regular Procuradorias Estaduais e Municipais
- Procuradorias Municipais e Estaduais | Peças Práticas
- Procuradorias | Assinatura
- Combo Escrevente TJ/SP + Analista MPSP
- Analista do MPSP | Pré-Edital Online
- OAB + Residência Jurídica TJ/SP
- Escrevente Técnico Judiciário TJ/SP | Regular Pré-Edital
- Escrevente Técnico Judiciário TJ/SP | Treino de Questões - Pré- Edital
- Escrevente Técnico Judiciário TJ/SP | Treino de Questões + Regular - Pré- Edital
- TSE/ TREs - Unificado | Assinatura
- TRF3 - Analista Judiciário - Área Judiciária | Pré-Edital - Online
- TRF3 - Técnico Judiciário - Área Administrativa | Pré - Edital - início 17/08
- Tribunais | Assinatura
- 6º ENAM 2026.2 - Online - início 08/09
- ENAM | Assinatura

### Entregáveis / Formato (termos encontrados na LP)
- PDF
- Simulados


========================================

---
id_oferta: 025
anunciante: "VLSA"
url_destino: "https://api.whatsapp.com/send"
ad_library_url: "https://www.facebook.com/ads/library/?id=1156163713628783"
dias_ativo: 56
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "justica eleitoral"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "imagem (1)"
botoes: "Saiba mais (1)"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Captura de Lead (WhatsApp / Grupo VIP)"
heuristica_nicho_estimado: "Carreiras Jurídicas / OAB"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Lançados em agosto de 2026
Categorias
Tamanho estimado do público:
1 mil a 5 mil
Valor gasto (BRL):
<R$100
100 a 999
Patrocinado • Pago por Canuto e Lucena Sociedade de Advogados
Cargo público, nova candidatura ou simples emissão de documento: você descobriu que está com pendência na Justiça Eleitoral por omissão da prestação de contas?
É muito comum que ex-candidatos só percebam esse problema anos depois da campanha, muitas vezes numa hora decisiva, como uma posse ou o início de uma nova disputa eleitoral.
Seja por falha do contador, do partido ou da equipe de campanha, a pendência acaba ficando no seu nome. Mas existe caminho para resolver isso através da Regularização da Prestação de Contas Eleitorais.
Com esse recurso, é possível avaliar o seu caso e buscar a regularização perante a Justiça Eleitoral.
Procure um advogado e conheça seus direitos.
Advogados Especialistas"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 026
anunciante: "Tribunal Regional Eleitoral de Santa Catarina"
url_destino: "https://linktr.ee/tribunalregionaleleitoraldesc?utm_source=linktree_profile_share&ltsid=493740a3-46c0-4ab3-b13d-7834ee719d97&utm_medium=social&utm_content=link_in_bio&fbclid=PAcGRvZgJleHRuA2FlbQIxMQBzcnRjBmFwcF9pZA85MzY2MTk3NDMzOTI0NTkAAae8-tmV39LZcelWqAv6pVt8Py2ghpelAMJXxevZCLdJZbbKTjJJBliiSX0AAw_aem_vgmFFLWuAa6EgoVKyI-qVQ"
ad_library_url: "https://www.facebook.com/ads/library/?id=1073809275368257"
dias_ativo: 22
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
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Categorias
Tamanho estimado do público:
50 mil a 100 mil
Valor gasto (BRL):
R$300 a R$399
500 mil a 600 mil
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
id_oferta: 027
anunciante: "Advocacia para Concursos - Mattozo & Ribeiro"
url_destino: "https://www.facebook.com/100089931653062/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1934024137978229"
dias_ativo: 15
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
dias_distintos_coletado: 4
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
id_oferta: 028
anunciante: "Escola Até a Aprovação Policiais"
url_destino: "https://www.facebook.com/eaapoliciais/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1837036453960474"
dias_ativo: 10
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
dias_distintos_coletado: 3
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

---
id_oferta: 029
anunciante: "oliberal.com"
url_destino: "https://www.facebook.com/oliberal/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1154864303742580"
dias_ativo: 8
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
dias_distintos_coletado: 1
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

# Parte 2 — Ofertas adjacentes (75)

Apareceram nas buscas, mas não citam os termos do foco. Servem para comparar formatos e preços de outros nichos de concurso; algumas não são de concurso.

---
id_oferta: 030
anunciante: "Sou Concurseiro"
url_destino: "https://www.facebook.com/souconcurseiroevoupassaroficial/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2192944634623317"
dias_ativo: 8
anuncios_coletados: 18
anuncios_ativos_estimados: 29
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "vídeo (18)"
botoes: "sem botão (18)"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 1
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
id_oferta: 031
anunciante: "Gustavo Dias"
url_destino: "https://lp.gdconcursos.com.br/mentoria-df"
ad_library_url: "https://www.facebook.com/ads/library/?id=1604173907842989"
dias_ativo: 8
anuncios_coletados: 2
anuncios_ativos_estimados: 20
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (2)"
botoes: "sem botão (2)"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 1
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
id_oferta: 032
anunciante: "Portal & OAB"
url_destino: "https://olympus.cursosdoportal.com.br/o-adm-tj-pb/?utm_source=%7B%7Bsite_source_name%7D%7D&utm_medium=%7B%7Badset.name%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D&utm_term=%7B%7Bplacement%7D%7D&utm_content=%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1046187021716727"
dias_ativo: 8
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
dias_distintos_coletado: 1
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
id_oferta: 033
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://www.facebook.com/simboraconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=436273172079349"
dias_ativo: 926
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
dias_distintos_coletado: 4
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
id_oferta: 034
anunciante: "Gustavo Nogueira - Aprovação Ágil"
url_destino: "https://pages.aprovacaoagil.com.br/vsl/tjsp/v01"
ad_library_url: "https://www.facebook.com/ads/library/?id=1701055018694486"
dias_ativo: 10
anuncios_coletados: 2
anuncios_ativos_estimados: 6
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (2)"
botoes: "sem botão (2)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 3
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Dá pra passar em escrevente sem ser do Direito? Dá. E não é porque a prova é fácil — é porque ela não te pede pra recitar a lei.
São 70 questões de múltipla escolha, com a resposta certa impressa entre as alternativas. Seu trabalho é reconhecer a certa, não escrever ela.
Cargo de nível médio, aceita qualquer formação, mais de R$9.000 iniciais.
Clica no botão e assiste a aula gratuita enquanto ela está no ar."

### Landing Page: Headline & Promessa Central
"Aprovação Ágil"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 035
anunciante: "Central de Concursos"
url_destino: "https://centraldeconcursos.com.br/concursos/concurso-tj-sp-escrevente"
ad_library_url: "https://www.facebook.com/ads/library/?id=4419979344943402"
dias_ativo: 88
anuncios_coletados: 2
anuncios_ativos_estimados: 5
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "vídeo (2)"
botoes: "sem botão (2)"
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
id_oferta: 036
anunciante: "Decorando a Lei Seca Cursos Para Concursos E OAB"
url_destino: "https://www.facebook.com/decorandoaleisecaconcursoseoab/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1351953739797164"
dias_ativo: 77
anuncios_coletados: 5
anuncios_ativos_estimados: 5
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Questões / simulados, Lei seca / legislação, Discursiva / redação"
formatos_dos_anuncios: "vídeo (1), carrossel (1), imagem (3)"
botoes: "sem botão (4), Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Carreiras Policiais"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O Código Penal usa a mesma técnica de redação em dois artigos diferentes, e as bancas cobram a diferença exatamente do mesmo jeito.
Conforme o art. 26, quem é inteiramente incapaz de entender o caráter ilícito do fato é inimputável: isento de pena. Quem não era inteiramente capaz é semi-imputável: responde pelo crime, com a pena reduzida de um a dois terços.
No art. 28, a lógica se repete na embriaguez proveniente de caso fortuito ou força maior. Completa e inteiramente incapaz, isenta. Sem a plena capacidade, reduz.
Repare no que a banca CEBRASPE fez: descreveu com precisão a hipótese do § 2º e concluiu pela isenção do § 1º. A FGV aplicou a mesma manobra no art. 26, neste ano.
E é aqui que está o detalhe que decide: a diferença entre isentar e reduzir não está na descrição do estado do agente, que é quase idêntica nos dois parágrafos. Está no advérbio. Memorizar o dispositivo até o fim, e não parar na parte que soa familiar, é o que separa o acerto do erro nesse tema.
Treine a lei seca artigo por artigo no Vade Mecum de Questões."

### Ganchos das variações (1ª linha de cada anúncio)
- EDITAL PUBLICADO: TRT-8ª REGIÃO (PA/AP)
- O art. 30 do Código Penal é daqueles dispositivos curtos, mas que a banca adora explorar em prova objetiva.
- ⚠️ Uma palavra pode mudar completamente o gabarito da questão.
- O Código Penal usa a mesma técnica de redação em dois artigos diferentes, e as bancas cobram a diferença exatamente do mesmo jeito.

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 037
anunciante: "Matheus Santos - Eu concursado"
url_destino: "https://seraprovado.com/mentoria-matheussantos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1059387566661056"
dias_ativo: 74
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
id_oferta: 038
anunciante: "Sou Concurseiro"
url_destino: "https://fabiomsam-cloud.github.io/sou-webinario-52b91323/?w=tjam"
ad_library_url: "https://www.facebook.com/ads/library/?id=2022633991782979"
dias_ativo: 8
anuncios_coletados: 5
anuncios_ativos_estimados: 5
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Lei seca / legislação"
formatos_dos_anuncios: "vídeo (5)"
botoes: "Saiba mais (5)"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 1
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

---
id_oferta: 039
anunciante: "Professor Fabiano Pereira"
url_destino: "https://aprovatte.com.br/mentoria-start90-2025/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1706536637805608"
dias_ativo: 19
anuncios_coletados: 4
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento"
formatos_dos_anuncios: "vídeo (4)"
botoes: "Saiba mais (4)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
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

### Títulos do link nos anúncios
- Tribunal de Justiça de GO

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
id_oferta: 040
anunciante: "Giovanna Carranza Desenvolvimento Profissional"
url_destino: "https://carranzacursos.com.br/trf8/?utm_source=mta-ads"
ad_library_url: "https://www.facebook.com/ads/library/?id=2312350235969478"
dias_ativo: 8
anuncios_coletados: 2
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (2)"
botoes: "sem botão (2)"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Concurso TRT8!
Participe do Grupo de Estudos VIP e recebe uma série de aulas e materiais totalmente gratuito, com o passo a passo para sua aprovação!"

### Landing Page: Headline & Promessa Central
"Concurso TRT 8 (AP/PA): descubra como ser aprovado mesmo começando do zero — A banca do concurso do TRT 8, Tribunal Regional do Trabalho da 8ª Região (AP/PA) , já foi definida. Entre para o grupo de estudos no WhatsApp, saia na frente e receba conteúdos exclusivos e muito mais. Totalmente online e gratuito."

### Seções da Landing Page (títulos, na ordem)
- Entre na sua conta
- Aprovados

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 041
anunciante: "Editora Solução"
url_destino: "https://aprovacao.editorasolucao.com.br/cupons-de-desconto"
ad_library_url: "https://www.facebook.com/ads/library/?id=2044043522985885"
dias_ativo: 134
anuncios_coletados: 1
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "imagem (1)"
botoes: "sem botão (1)"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🎉 Desconto Exclusivo para Você! 🎉
Aproveite 5% OFF em todo o site da Editora Solução! 😍
📚 Primeira compra? Já começa com aquele descontinho especial!
🔗 Use o cupom e garanta seu sucesso nos estudos com o material ideal. Não perca essa oportunidade! 🚀
Já pegou seu Cupom?
See Details"

### Landing Page: Headline & Promessa Central
"Cupom EXCLUSIVO de 5% OFF em todo Site — DESCONTOS ESPECIAIS!"

### Seções da Landing Page (títulos, na ordem)
- DESCONTOS ESPECIAIS!
- Cupons de desconto, liberados especialmente para VOCÊ!
- COPIE O CUPOM:
- 5% de Desconto em sua primeira compra na Editora Solução!
- Melhor Custo Benefício!
- Materiais Atualizados
- Qualidade Garantida!
- ALGUMA DÚVIDA?
- Entre em contato com a nossa equipe, estaremos prontos para te ajudar.
- Editora Solução 2025 ©. Todos os direitos reservados

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 042
anunciante: "Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24"
url_destino: "https://ataticadaaprovacao.com.br/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1685357465868904"
dias_ativo: 85
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
dias_distintos_coletado: 4
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
id_oferta: 043
anunciante: "Revolução Concursos"
url_destino: "https://www.facebook.com/61576683587518/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1423969583205016"
dias_ativo: 47
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
dias_distintos_coletado: 2
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
id_oferta: 044
anunciante: "Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24"
url_destino: "https://ataticadaaprovacao.com.br/combao/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1088210254181707"
dias_ativo: 31
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
dias_distintos_coletado: 4
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

## Demais adjacentes (resumo)

| id | Anunciante | Dias | Anúncios | Tração | Ticket (checkout) | Destino |
|---|---|---|---|---|---|---|
| 045 | Memoriza-aí Concursos | 8 | 3 | médio | Não confirmado | https://memorizaai.com.br/trt-8/?src=&utm_source=facebook-ads&utm_medium=%7B%7Ba |
| 046 | Concursos Ceisc | 193 | 2 | médio | Não confirmado | https://ceisc.com.br/cursos/2067-concurso-tj-sp-club-oficial-de-justica?utm_sour |
| 047 | Pódio Tribunais | 173 | 2 | médio | Não confirmado | https://api.whatsapp.com/send |
| 048 | Felipe Sgarbossa Advocacia Criminal | 168 | 2 | médio | Não confirmado | https://www.facebook.com/felipesgarbossa/ |
| 049 | Prof.carlosgoncalves | 123 | 2 | médio | Não confirmado | https://typebot.co/plataformaanalistadetribunais |
| 050 | IPOG Salvador | 114 | 2 | médio | Não confirmado | https://ipog.edu.br/cursos/pos-graduacao/psicologia-juridica-com-enfase-em-peric |
| 051 | Tjteiros | 99 | 2 | médio | Não confirmado | https://www.facebook.com/61582438800580/ |
| 052 | Estratégia Concursos | 86 | 2 | médio | Não confirmado | https://www.facebook.com/EstrategiaConcursos/ |
| 053 | Gazeta dos Concursos | 78 | 2 | médio | Não confirmado | https://lp.aprovacaoagil.com.br/vsl-white-trt-noticia |
| 054 | Venâncio & Delgado - Advogados | 60 | 2 | médio | Não confirmado | https://api.whatsapp.com/send |
| 055 | Venâncio & Delgado - Advogados | 60 | 2 | médio | Não confirmado | https://www.facebook.com/venancioedelgadoadvogados/ |
| 056 | Concursos Ceisc | 53 | 2 | médio | Não confirmado | https://ceisc.com.br/cursos/2089-concurso-trt-4-club-analista-judiciario-area-ju |
| 057 | Alan Matos | 53 | 2 | médio | Não confirmado | https://concursotcdf.editorainovedigital.com/ |
| 058 | Lucas Viégas | 46 | 2 | médio | Não confirmado | https://foconocontrole.com.br/ |
| 059 | Serviço Social para Concursos | 31 | 2 | médio | R$ 837,00 | https://ssparaconcursos.com.br/clube-assistente-social-sociojuridico/?utm_source |
| 060 | Tucuju Bizurado Concursos | 19 | 2 | médio | Não confirmado | https://pay.plataformatutory.com.br/checkout/e5143ac2-626f-4616-9ab0-f146202578c |
| 061 | Grupo Revisamed | 16 | 2 | fraco | Não confirmado | https://mediccurso.com.br/medprovas-lp/?utm_medium=%7B%7Badset.name%7D%7D_-_%7B% |
| 062 | IDP - SP | 9 | 2 | médio | Não confirmado | https://pos.idp.edu.br/pages/lp-mestrado-profissional-em-direito-justica-e-desen |
| 063 | Escola Flamengo - Unid Santos | 207 | 1 | médio | Não confirmado | https://www.facebook.com/61573410848498/ |
| 064 | Pódio Tribunais | 200 | 1 | médio | Não confirmado | https://cronosconcursos.com.br/tribunais/?utm_source=meta&utm_medium=ig-ads&utm_ |
| 065 | Concursos Ceisc | 193 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2070-concurso-tj-ba-analista-judiciario-area-judicia |
| 066 | Gaby no Tribunal | 177 | 1 | médio | Não confirmado | https://www.facebook.com/100090566482087/ |
| 067 | Discursiva na Prática | 128 | 1 | médio | R$ 1.489,00 | https://discursivanapratica.com.br/assinaturacontrole/?utm_source=facebook&utm_m |
| 068 | Douglas Prado - Servidor 30k | 105 | 1 | médio | Não confirmado | https://odouglasprado.com.br/plano-servidor-30k/ |
| 069 | Fauth e Freitas Sociedade de Advogados com Adriane Fauth | 94 | 1 | médio | Não confirmado | https://www.facebook.com/61573224123970/ |
| 070 | Brabo Editora | 85 | 1 | médio | R$ 397,00 | https://braboeditora.com.br/mestre-em-questoes-tjsp-v8/ |
| 071 | Ludy Sena | 85 | 1 | médio | Não confirmado | https://www.facebook.com/ludysena.perita/ |
| 072 | Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24 | 80 | 1 | médio | Não confirmado | https://metastatus.com/ads-transparency |
| 073 | LH no pódio | 79 | 1 | médio | Não confirmado | https://typebot.co/mentoria-zeroaopodio |
| 074 | Trteiros | 74 | 1 | médio | Não confirmado | https://www.facebook.com/61560675890210/ |
| 075 | Mege | 68 | 1 | médio | Não confirmado | https://concurcity.mege.com.br/explorar |
| 076 | Caderno do Aprovado - Materiais para Concursos | 67 | 1 | médio | R$ 497,00 | https://cadernodoaprovado.com/trf-tj-mp/ |
| 077 | Themas Cartórios | 66 | 1 | médio | Não confirmado | http://www.themas.com.br/ |
| 078 | Concurseiro Fora da Caixa | 59 | 1 | médio | Não confirmado | https://concurseiroforadacaixa.com.br/collections/todos-os-materiais |
| 079 | Bruna Vieira | 58 | 1 | médio | Não confirmado | https://5k.taciotj.online/ |
| 080 | Professora Amanda Aires | 56 | 1 | médio | Não confirmado | https://www.amandaaires.com.br/curso/%5B2026%5D-economia-para-o-tcu/345 |
| 081 | Rô Santtana - OAB | 53 | 1 | médio | Não confirmado | https://rosanttana.com.br/captacao/lp-discursiva-oab.html |
| 082 | Concursos Ceisc | 52 | 1 | médio | Não confirmado | https://www.sympla.com.br/produtor/ceisc |
| 083 | Advogado de concurso | 47 | 1 | médio | Não confirmado | https://olivaesouza.com.br/tjsc-objetiva-nivel-superior-conhecimentos-gerais/ |
| 084 | Jus Expert | 47 | 1 | médio | R$ 997,00 | https://pages.jusexpert.com/vsl-grafotecnica-principal |
| 085 | Progresso Concursos | 39 | 1 | médio | Não confirmado | https://progressoconcursos.com.br/produto/resumo-bizurado-do-que-mais-cai-em-pro |
| 086 | Concursos Ceisc | 29 | 1 | médio | Não confirmado | https://lp.ceisc.com.br/material-concurso-trt-4-projeto-nomeacao/ |
| 087 | Treinar na Oficina | 29 | 1 | médio | Não confirmado | https://www.facebook.com/61575606707746/ |
| 088 | Treinar na Oficina | 29 | 1 | médio | Não confirmado | https://www.ev8auto.com.br/osciloscopio-e-multimetro |
| 089 | Elevato Brasil Cursos e Treinamentos | 29 | 1 | médio | Não confirmado | https://www.facebook.com/brunovanuciseg/ |
| 090 | _rrautomoveis_ | 26 | 1 | médio | Não confirmado | https://rrautomoveis1.com.br/ |
| 091 | Local Imóveis Alto de Pinheiros | 19 | 1 | médio | Não confirmado | http://fb.me/ |
| 092 | Fas Lex Treinamentos E Licitações Ltda | 15 | 1 | médio | Não confirmado | https://escalla.pro/ |
| 093 | Portal & OAB | 10 | 1 | médio | Não confirmado | https://olympus.cursosdoportal.com.br/o-mil-smtt-aracaju/?utm_source=%7B%7Bsite_ |
| 094 | Professor Raphael Reis | 10 | 1 | médio | Não confirmado | https://www.facebook.com/profraphaelreis/ |
| 095 | Unipds | 10 | 1 | médio | Não confirmado | https://unipds.com.br/unipds-ia-funil/#hero |
| 096 | Migalhas | 10 | 1 | médio | Não confirmado | https://eventos.migalhas.com.br/evento/738/namoro-qualificado-e-uniao-estavel-ca |
| 097 | Êutika Assessoria Empresarial | 9 | 1 | médio | Não confirmado | https://www.facebook.com/61556190747058/ |
| 098 | 123passei | 8 | 1 | médio | Não confirmado | https://www.facebook.com/123PasseiOficial/ |
| 099 | Malditafcc | 8 | 1 | médio | Não confirmado | https://www.facebook.com/malditafcc/ |
| 100 | Carreiras Educação com Professor Jobson Castelo Branco | 8 | 1 | médio | Não confirmado | https://www.facebook.com/61572024614383/ |
| 101 | HB CAR | 8 | 1 | médio | Não confirmado | https://www.facebook.com/hbcaroficial/ |
| 102 | Aprovando Concurseiro | 8 | 1 | médio | R$ 57,99 | https://pay.hotmart.com/S107640643D?checkoutMode=10 |
| 103 | Aprovando Concurseiro | 8 | 1 | médio | R$ 57,99 | https://pay.hotmart.com/M107002055F?checkoutMode=10 |
| 104 | Marcelomapas | 8 | 1 | fraco | Não confirmado | https://resumosmapasdireito.com/cgi-sys/suspendedpage.cgi |

# Apêndice — Descartadas por não citarem concurso (74)

Vieram nas buscas (ex.: escritórios que citam o TRF como tribunal), mas o texto não tem nenhum termo de concurso. Confira se algo relevante caiu aqui por engano.

| Anunciante | Dias | Destino |
|---|---|---|
| mauroautomoveisrj | 226 | https://www.facebook.com/mauroautomoveisrj/ |
| Scientific Research & Co - Pelve | 32 | https://scientificresearch.com.br/incontinencia-urinaria/ |
| DARKNESS NATION | 18 | https://www.darkness.com.br/melhor-pre-treino-evora-xt/p?sabor=Orange%20Storm&ta |
| Pablo | 43 | https://pablochaer.com.br/treinamento/?utm_source=%7B%7Bplacement%7D%7D&utm_medi |
| Elton Fernandes - Advocacia Especializada em Saúde | 119 | https://foierromedico.com.br/ |
| Rita Bervig | 180 | https://www.facebook.com/100091834883862/ |
| CONPEJ | 121 | https://www.facebook.com/conpejnacional/ |
| Aquática American Park | 112 | https://sobre.aquaticaamericanpark.com.br/eventos |
| Emais | 18 | https://emais.com/terrenos/eplenum-reserve?utm_source=meta-ads&utm_medium=cpc&ut |
| Previdas Saúde | 12 | https://provamedica3.previdas.com.br/?src=&utm_source=meta&utm_medium=%7B%7Badse |
| Comunidade Milhorin | 8 | https://www.facebook.com/milhorincalculos/ |
| Heraclio Cunha | 53 | https://peritoem7dias.com.br/ |
| FlipWash | 26 | https://www.facebook.com/flipwash/ |
| Vitafor Nutrientes com Vitafor Science | 17 | https://www.facebook.com/vitafor/ |
| DARKNESS NATION | 17 | https://www.darkness.com.br/pre-treino |
| Farmácias Nissei | 10 | https://www.farmaciasnissei.com.br/lam-quinzena-outubro-cabelos |
| Good Shape Rj | 10 | https://www.facebook.com/goodshaperj25/ |
| LuFi Life Comércio De Cosméticos e Suplementação | 8 | https://lufilife.com/ |
| Tribunal Regional Eleitoral de Mato Grosso | 414 | https://www.facebook.com/tremtoficial/ |
| Loja do Mecânico | 185 | https://www.facebook.com/lojadomecanico/ |
| Danielle Bartoly | 172 | https://www.facebook.com/61577922862090/ |
| Editora Mizuno | 143 | https://www.editoramizuno.com.br/ |
| Douglas Prado - Servidor 30k com Servidores High Level | 126 | https://www.facebook.com/professorlucrativo/ |
| REDI Acoustics | 115 | https://app.rediacoustics.com/ |
| 42pericias | 104 | https://www.42pericias.com.br/ |
| Duarte Advogados Associados | 103 | https://www.facebook.com/61555624388490/ |
| JQM Advocacia Especializada | 102 | https://www.facebook.com/61561436444397/ |
| Cetrus - Educação Médica | 101 | http://fb.me/ |
| Fibra Pará | 96 | https://www.facebook.com/fibrapara/ |
| Farmácias Farmassim | 92 | https://www.facebook.com/farmassim/ |
| Carreira de Perito | 90 | https://carreiradeperito.com.br/ |
| IBCCRIM | 85 | https://jcc.ibccrim.org.br/ |
| Instituto Doutrina Policial 2 | 73 | http://fb.me/ |
| Scientific Research & Co - Pelve | 68 | https://scientificresearch.com.br/curso-avancado-de-hiperplasia-prostatica-benig |
| Sky Automóveis | 67 | https://www.facebook.com/61590275407719/ |
| Gel Mudanças e Transportes | 67 | https://www.facebook.com/61577458875831/ |
| Aquática American Park | 66 | https://www.facebook.com/aquaticaamericanpark/ |
| Academia Pinheiros | 62 | https://academiapinheiros.site/academia-pinheiros/ |
| Marcelo Mansano de Moraes | 61 | http://fb.me/ |
| RAIR Silva | 59 | https://www.facebook.com/jornalistarairsilva/ |
| Viégas Filho | 59 | https://www.facebook.com/100094050184913/ |
| thainara.assistentesocial | 57 | https://www.instagram.com/_u/thainara.assistentesocial |
| Gabriela Franco | 54 | https://www.facebook.com/61575028750782/ |
| Closet da BK | 53 | https://www.facebook.com/61556917691160/ |
| Go Kursos | 52 | https://www.gokursos.com/go-oab---direito-penal---2%C2%AA-fase-30553/p |
| Drogamil Carangola | 45 | https://api.whatsapp.com/send |
| Strong Car Services | 38 | https://www.facebook.com/strongcarservices/ |
| Expressa Veículos | 31 | https://www.facebook.com/expressaveiculos/ |
| Alibaba.com | 31 | https://www.alibaba.com/product-detail/haoge_11000005907027.html?src=cpm_fb&sub_ |
| Cetrus Grupo | 24 | http://fb.me/ |
| drayasminferreirazevedo | 24 | https://api.whatsapp.com/send |
| Dr Daniel Kruschewsky | 20 | https://www.facebook.com/drdanielkruschewsky/ |
| Cross Life Veloso - Osasco | 16 | https://www.facebook.com/61559104595340/ |
| Tre Amici Pizza | 15 | https://app.cardapioweb.com/tre_amici_pizzaria_e_restaurante?s=pub |
| Simone Freitas Imóveis | 15 | https://www.facebook.com/simonefreitasimoveisvr/ |
| Cleidimar Sousa | 14 | https://aceleradordenomeacao.com.br/mentoria-em-grupo |
| Halohealth | 14 | https://www.halodevice.com.br/products/halo-band |
| Elite Barber Shop | 11 | https://www.facebook.com/61574507885102/ |
| Sungrow | 10 | https://www.facebook.com/CleanPowerForAll/ |
| Beatriz Queiroz Semijóias | 10 | https://www.facebook.com/61579067742432/ |
| Gracielle Lima Assessoria e Consultoria Jurídica | 9 | https://www.facebook.com/61585454075287/ |
| Tapai Advogados | 9 | https://www.facebook.com/TapaiAdvogados/ |
| Giselle Tapai | 9 | https://www.facebook.com/61588752251791/ |
| Monica Freitas MTE | 9 | https://www.facebook.com/61583807948841/ |
| brenomarxoficial | 9 | https://www.facebook.com/100081178312118/ |
| SpeakApp | 9 | https://apps.apple.com/us/app/speakapp-ai-voice-notes/id6468764490 |
| Pharmafit Nutracêutica e Fitoterapia | 9 | https://www.facebook.com/feliphycustodiofito/ |
| Him+ Skin | 9 | https://himpluskin.com/pages/advertorial-lp |
| Daniella Costa Agro | 8 | https://www.facebook.com/61594331413710/ |
| samwelholandaadv | 8 | https://www.instagram.com/_u/samwelholandaadv |
| BSSP Centro Educacional | 8 | https://bsspce.com.br/pos-graduacao-e-mba/mba-pericia-contabil-economica-e-finan |
| Dr. Elpídio Donizetti | 8 | https://elpidiodonizetti.com.br/ |
| Top Life Purificadores | 8 | https://www.toplifefiltros.com.br/blog/onde-comprar-purificador-top-life |
| Mentoria Premium | 8 | https://www.facebook.com/61565632567995/ |
