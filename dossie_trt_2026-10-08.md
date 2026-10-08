# Dossiê ConcursoRadar — Técnico Judiciário — TRT (08/10/2026)

## Métricas da Rodada
- **Buscas na Meta Ad Library:** `concurso TRT`, `tribunal regional do trabalho`, `justiça do trabalho concurso`, `técnico judiciário`, `TRT técnico judiciário`, `TRT2`, `TRT15`, `TRT1`, `TRT4`, `TRT3`, `concurso tribunal`
- **Filtro:** anúncios ativos no Brasil, no ar há 7+ dias (coleta ampla para achar padrões; a longevidade é analisada nas tabelas)
- **Ofertas do nicho:** 130 (de 342 anúncios; agrupadas por anunciante + página de destino)
- **Descartadas por não citarem concurso:** 128 (listadas no fim para auditoria)
- **Ofertas de foco direto:** 64 | adjacentes: 66
- **Sinal de tração:** 9 forte, 1 fraco, 120 médio
- **Landing pages lidas:** 88 de 130
- **Ticket confirmado no checkout:** 13 de 15 ofertas com checkout detectado (87%)
- **Tempo de processamento:** 819 segundos

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

Base: **342 anúncios de 98 anunciantes**; 144 estão no ar há 45+ dias (veteranos); mediana de 17 dias.

Como ler: **Anunciantes** = quantos produtores distintos usam (popularidade). **Veteranos** = quantos desses anúncios estão no ar há 45+ dias, e **% dos veteranos** = a fatia da categoria entre todos os veteranos. Se a fatia entre veteranos é maior que a fatia geral (% anúncios), a categoria aparece mais entre os que duram. Categoria com 1 ou 2 anunciantes é só um caso isolado.

A coleta junta duas amostras por busca (anúncios com 7+ dias e anúncios com 45+ dias), então a proporção de veteranos no total não é uma taxa de sobrevivência.

## Formato do criativo

Vídeo, imagem única ou carrossel.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| vídeo | 57 | 58% | 126 | 37% | 57 | 77 | 53% |
| imagem | 37 | 38% | 162 | 47% | 11 | 41 | 28% |
| carrossel | 26 | 27% | 54 | 16% | 36 | 26 | 18% |

## Proporção do criativo

Vertical (4:5 ou 9:16), quadrada (1:1) ou horizontal.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| vídeo vertical | 54 | 55% | 121 | 35% | 58 | 75 | 52% |
| imagem vertical | 30 | 31% | 146 | 43% | 11 | 30 | 21% |
| carrossel vertical | 18 | 18% | 32 | 9% | 71 | 21 | 15% |
| carrossel quadrada | 9 | 9% | 12 | 4% | 25 | 5 | 3% |
| imagem quadrada | 8 | 8% | 14 | 4% | 57 | 11 | 8% |
| vídeo quadrada | 3 | 3% | 4 | 1% | 40 | 2 | 1% |
| carrossel horizontal | 2 | 2% | 10 | 3% | 8 | 0 | 0% |
| imagem horizontal | 2 | 2% | 2 | 1% | 23 | 0 | 0% |
| vídeo horizontal | 1 | 1% | 1 | 0% | 23 | 0 | 0% |

## Duração dos vídeos

Só anúncios em vídeo.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| 31s a 1min | 31 | 54% | 60 | 48% | 58 | 40 | 52% |
| 1 a 2min | 23 | 40% | 39 | 31% | 57 | 22 | 29% |
| Mais de 2min | 11 | 19% | 14 | 11% | 62 | 9 | 12% |
| Até 30s | 8 | 14% | 13 | 10% | 15 | 6 | 8% |

## Botão (CTA)

Rótulo do botão exibido no anúncio.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Saiba mais | 41 | 42% | 128 | 37% | 11 | 53 | 37% |
| sem botão | 40 | 41% | 109 | 32% | 17 | 44 | 31% |
| Ver detalhes | 18 | 18% | 43 | 13% | 49 | 25 | 17% |
| Visitar perfil do Instagram | 14 | 14% | 24 | 7% | 74 | 13 | 9% |
| Enviar mensagem pelo WhatsApp | 9 | 9% | 21 | 6% | 8 | 0 | 0% |
| Comprar agora | 6 | 6% | 13 | 4% | 13 | 6 | 4% |
| Cadastre-se | 2 | 2% | 2 | 1% | 39 | 1 | 1% |
| Solicitar agora | 1 | 1% | 1 | 0% | 87 | 1 | 1% |
| Inscreva-se | 1 | 1% | 1 | 0% | 87 | 1 | 1% |

## Destino do clique

Para onde o anúncio leva.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Página própria (LP / site) | 65 | 66% | 259 | 76% | 13 | 97 | 67% |
| Página / formulário no Facebook | 36 | 37% | 74 | 22% | 58 | 41 | 28% |
| WhatsApp | 4 | 4% | 7 | 2% | 58 | 4 | 3% |
| Perfil do Instagram | 1 | 1% | 1 | 0% | 49 | 1 | 1% |
| Checkout direto | 1 | 1% | 1 | 0% | 50 | 1 | 1% |

## Tamanho da copy

Texto principal do anúncio.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Longa (mais de 600) | 50 | 51% | 136 | 40% | 23 | 58 | 40% |
| Média (200 a 600) | 48 | 49% | 152 | 44% | 48 | 78 | 54% |
| Curta (até 200 caracteres) | 12 | 12% | 53 | 15% | 11 | 8 | 6% |
| Sem texto | 1 | 1% | 1 | 0% | 13 | 0 | 0% |

## Tipo de gancho (1ª linha da copy)

Classificação por palavras-chave; um gancho pode cair em mais de um tipo.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos | Exemplo |
|---|---|---|---|---|---|---|---|---|
| Outro | 54 | 55% | 105 | 31% | 30 | 51 | 35% | 🚨 PROCURA-SE FISIOTERAPEUTAS🚨 — Clube do Perito |
| Notícia de concurso / edital | 26 | 27% | 83 | 24% | 9 | 25 | 17% | Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova? — MEQ Concursos |
| Pergunta | 18 | 18% | 55 | 16% | 58 | 30 | 21% | Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova? — MEQ Concursos |
| Dor / erro do candidato | 14 | 14% | 40 | 12% | 9 | 10 | 7% | Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova? — MEQ Concursos |
| Número / lista | 14 | 14% | 40 | 12% | 11 | 8 | 6% | A Ana Flávia chegou até mim faltando apenas 15 dias para o concurso do Tribunal de Justiça do Rio de Janeiro. — Prof. Ronaldo Santos |
| Oferta / desconto / urgência | 12 | 12% | 28 | 8% | 45 | 14 | 10% | "📚🆓 Curso Grátis TJ-SP 2026 - Escrevente Técnico Judiciário! 🆓📚 — Nova Concursos |
| Salário / estabilidade | 11 | 11% | 38 | 11% | 11 | 10 | 7% | O TJ-SP Escrevente é uma grande oportunidade para quem busca estabilidade e carreira pública com nível médio. — Central de Concursos |
| Prova social / autoridade | 11 | 11% | 26 | 8% | 58 | 18 | 12% | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? — Isaque Concursos |
| Chamada direta ao público | 11 | 11% | 20 | 6% | 85 | 16 | 11% | O TJ-SP Escrevente é uma grande oportunidade para quem busca estabilidade e carreira pública com nível médio. — Central de Concursos |
| Promessa de método | 8 | 8% | 20 | 6% | 58 | 19 | 13% | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? — Isaque Concursos |
| Contraintuitivo / inimigo comum | 4 | 4% | 6 | 2% | 11 | 2 | 1% | Três anos no cursinho jurídico. Sete apostilões de Direito. E fiquei em cadastro de reserva no primeiro TRT que eu prestei. — Gustavo Nogueira - Aprovação Ágil |

## Elementos da copy

Recursos presentes no texto; não são excludentes.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Usa emojis | 59 | 60% | 189 | 55% | 23 | 86 | 60% |
| Hashtags | 26 | 27% | 45 | 13% | 58 | 27 | 19% |
| Cita valor em R$ | 25 | 26% | 81 | 24% | 9 | 13 | 9% |
| Lista com marcadores (✔, ✅, •) | 23 | 23% | 58 | 17% | 58 | 34 | 24% |
| Link ou 'link na bio' no texto | 14 | 14% | 29 | 8% | 17 | 14 | 10% |
| Gancho em CAIXA ALTA | 9 | 9% | 18 | 5% | 8 | 3 | 2% |
| Cita bônus | 4 | 4% | 8 | 2% | 58 | 7 | 5% |
| Cita garantia | 4 | 4% | 5 | 1% | 85 | 3 | 2% |

## Sinais de público (ICP) citados na copy

Quem o anúncio diz atender, por palavras-chave. Indica a quem o mercado fala, não quem compra.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos | Exemplo |
|---|---|---|---|---|---|---|---|---|
| Motivado por salário / estabilidade | 29 | 30% | 98 | 29% | 11 | 28 | 19% | Se você quer chegar competitivo para ser aprovado e nomeado nas próximas provas de TRTs, a Imersão Aprova TRT pode ser um divisor de águas para conquistar a tão — Isaque Concursos |
| Esquece o que estuda / revisão | 20 | 20% | 49 | 14% | 29 | 21 | 15% | 📚 Quem quer disputar uma vaga de verdade precisa construir base, revisar com método, acompanhar o próprio desempenho e estudar com direção. — Concurseiro aos 40 |
| Trabalha / tem pouco tempo | 15 | 15% | 82 | 24% | 11 | 29 | 20% | Durante essa jornada de estudos, eu estudava de 2h a 3h por dia, já que estudava e trabalhava como CLT. — Isaque Concursos |
| Pré-edital / sair na frente | 14 | 14% | 34 | 10% | 10 | 12 | 8% | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. — Tjteiros |
| Dificuldade em discursiva / redação | 10 | 10% | 38 | 11% | 9 | 8 | 6% | Não para estudar mais um pouco. Para sentar, encarar 60 questões seguidas, matérias misturadas, discursiva e o relógio correndo. — MEQ Concursos |
| Nível médio | 10 | 10% | 29 | 8% | 56 | 15 | 10% | Para você ter uma ideia, eu só me formei no ensino médio por meio do ENCCEJA, já que tinha repetido em todas as matérias. — Isaque Concursos |
| Começando do zero | 8 | 8% | 35 | 10% | 23 | 15 | 10% | • Esteja começando os estudos agora; — Isaque Concursos |
| Estuda há tempo e não passa | 8 | 8% | 16 | 5% | 57 | 11 | 8% | Você estuda, se prepara, domina o conteúdo… mas ainda trava na hora da redação? 📝 — Professor Hansk |
| Reta final / pós-edital | 8 | 8% | 14 | 4% | 30 | 6 | 4% | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. — Tjteiros |
| Mãe / família | 5 | 5% | 13 | 4% | 58 | 12 | 8% | Se isso não fosse o bastante, eu tive uma infância/adolescência bem difícil. Sou filho de ex -empregada doméstica e, por isso, não tínhamos condições financeira — Isaque Concursos |
| Perdido no excesso de conteúdo | 4 | 4% | 11 | 3% | 14 | 4 | 3% | O que trava a maioria é achar que pra passar tem que saber a matéria inteira. Você abre o edital gigante, tenta decorar tudo e chega no dia da prova travado, po — Gustavo Nogueira - Aprovação Ágil |
| Erra questões / pegadinhas da banca | 4 | 4% | 7 | 2% | 38 | 3 | 2% | O que trava a maioria é achar que pra passar tem que saber a matéria inteira. Você abre o edital gigante, tenta decorar tudo e chega no dia da prova travado, po — Gustavo Nogueira - Aprovação Ágil |
| Nível superior / Direito | 3 | 3% | 3 | 1% | 87 | 2 | 1% | Trata-se de uma oportunidade de nível superior com MUITAS vagas, e uma remuneração inicial muito atrativa. — Concursos Ceisc |

## Tipo de produto × ticket

Tipo identificado por palavras-chave na copy, no título do link e na headline (uma oferta pode ter vários). Ticket só entra quando foi lido no checkout.

| Tipo de produto | Anunciantes | Ofertas | Veteranas | Com ticket lido | Mínimo | Mediana | Máximo | Tickets lidos |
|---|---|---|---|---|---|---|---|---|
| Material em PDF / apostila / caderno | 48 | 54 | 31 | 4 | R$ 397 | R$ 497 | R$ 1.489 | Brabo Editora R$ 397; Academia do Perito R$ 497; Caderno do Aprovado - Materiais para Concursos R$ 497; Discursiva na Prática R$ 1.489 |
| Curso em videoaulas | 28 | 39 | 25 | 5 | R$ 397 | R$ 827 | R$ 6.346 | Brabo Editora R$ 397; Professor Raphael Reis R$ 450; Instituto INAPI R$ 827; Discursiva na Prática R$ 1.489; Ceisc Concursos R$ 6.346 |
| Questões / simulados | 24 | 33 | 13 | 2 | R$ 397 | R$ 612 | R$ 827 | Brabo Editora R$ 397; Instituto INAPI R$ 827 |
| Isca gratuita / grupo VIP | 19 | 25 | 11 | 3 | R$ 497 | R$ 827 | R$ 6.346 | Isaque Concursos R$ 497; Instituto INAPI R$ 827; Ceisc Concursos R$ 6.346 |
| Não identificado | 18 | 19 | 10 | 3 | R$ 1.725 | R$ 2.747 | R$ 2.747 | Escola Trabalhista R$ 1.725; Escola Trabalhista R$ 2.747; prof.camilasabongi com Escola Trabalhista R$ 2.747 |
| Mentoria / acompanhamento | 17 | 21 | 12 | 1 | R$ 497 | R$ 497 | R$ 497 | Isaque Concursos R$ 497 |
| Cronograma / plano de estudos | 13 | 18 | 9 | 1 | R$ 497 | R$ 497 | R$ 497 | Isaque Concursos R$ 497 |
| Discursiva / redação | 11 | 14 | 6 | 2 | R$ 450 | R$ 970 | R$ 1.489 | Professor Raphael Reis R$ 450; Discursiva na Prática R$ 1.489 |
| Lei seca / legislação | 9 | 11 | 6 | 1 | R$ 497 | R$ 497 | R$ 497 | Caderno do Aprovado - Materiais para Concursos R$ 497 |
| Assinatura / clube / vitalício | 4 | 4 | 1 | 2 | R$ 598 | R$ 1.043 | R$ 1.489 | Mapas da Lulu Concurseira com Laura Amorim R$ 598; Discursiva na Prática R$ 1.489 |
| Mapas mentais / esquemas | 3 | 3 | 1 | 2 | R$ 497 | R$ 547 | R$ 598 | Caderno do Aprovado - Materiais para Concursos R$ 497; Mapas da Lulu Concurseira com Laura Amorim R$ 598 |
| Flashcards | 1 | 1 | 1 | 0 | — | — | — |  |

## Expressões repetidas entre anunciantes

Sequências de 2 ou 3 palavras (sem acento) usadas na copy por 3 ou mais anunciantes distintos.

`clique em saiba` (17), `tecnico judiciario` (14), `garanta sua vaga` (11), `tj sp` (8), `nivel medio` (8), `edital sair` (8), `analista judiciario` (8), `agora mesmo` (8), `quem quer` (7), `pre edital` (7), `concurso do trt` (7), `tribunal de contas` (6), `sair para comecar` (6), `remuneracao inicial` (6), `link da bio` (6), `escrevente tecnico judiciario` (6), `concursos publicos` (6), `ultimo concurso` (5), `tribunal regional` (5), `tribunal de justica` (5), `toque em saiba` (5), `regional do trabalho` (5), `realmente cai` (5), `quem estuda` (5), `publicacao do edital` (5), `pos edital` (5), `pode sair` (5), `novo concurso` (5), `ensino medio` (5), `concurso publico` (5)

## Arquivo de ganchos (anúncios mais replicados e mais antigos)

| Anunciante | Dias | Cópias | Formato | Botão | Gancho (1ª linha) | Título do link |
|---|---|---|---|---|---|---|
| MEQ Concursos | 9 | 13 | imagem | sem botão | Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova? |  |
| Isaque Concursos | 58 | 4 | vídeo | sem botão | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? |  |
| Clube do Perito | 15 | 4 | imagem | sem botão | 🚨 PROCURA-SE FISIOTERAPEUTAS🚨 |  |
| Central de Concursos | 86 | 3 | vídeo | sem botão | O TJ-SP Escrevente é uma grande oportunidade para quem busca estabilidade e carreira pública com nível médio. |  |
| Nova Concursos | 48 | 3 | imagem | sem botão | "📚🆓 Curso Grátis TJ-SP 2026 - Escrevente Técnico Judiciário! 🆓📚 |  |
| Concurseiro aos 40 | 23 | 3 | imagem | sem botão | ⚖️ Os próximos concursos de TRTs podem abrir excelentes oportunidades em diferentes regiões do país, com remunerações iniciais que podem chegar a cerca de R$ 16 mil. |  |
| Gazeta dos Concursos | 14 | 3 | vídeo | sem botão | Atravessei a faculdade de Direito decorando manual, virando noites, com a sensação de que estudar é sofrer. Quando comecei a pensar em TRT, achei que ia ser mais do mesmo. |  |
| Metodo.Gafanhoto | 9 | 3 | vídeo | sem botão | INDICAÇÃO CONCURSO PARA MULHERES QUE NÃO TEM BASE NOS ESTUDOS |  |
| Professor Hansk | 9 (baixo volume) | 3 | vídeo | sem botão | Você estuda, se prepara, domina o conteúdo… mas ainda trava na hora da redação? 📝 |  |
| Gustavo Nogueira - Aprovação Ágil | 8 | 3 | vídeo | sem botão | Três anos no cursinho jurídico. Sete apostilões de Direito. E fiquei em cadastro de reserva no primeiro TRT que eu prestei. |  |
| Meirelles Quintella Escritório de Advocacia | 8 | 3 | vídeo | sem botão | Alguns profissionais da área da saúde atuam em hospitais públicos sem ter ingressado por concurso. |  |
| Gustavo Nogueira - Aprovação Ágil | 8 | 3 | vídeo | sem botão | Dá pra passar em escrevente sem ser do Direito? Dá. E não é porque a prova é fácil — é porque ela não te pede pra recitar a lei. |  |
| Trteiros | 121 | 2 | vídeo | sem botão | 🚨Informações sobre o TRT/MG |  |
| Trteiros | 121 | 2 | vídeo | sem botão | 🚨Informações sobre o TRT/BA |  |
| Tjteiros | 97 | 2 | vídeo | sem botão | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. |  |
| Brabo Concursos | 92 | 2 | vídeo | sem botão | O TJ-SP tem um novo concurso previsto para 2026, são mais de 3.300 cargos vagos de Escrevente Técnico Judiciário, temos contrato assinado com a banca organizadora e recentemente foram criados novas 720 vagas de Escrevent |  |
| Central de Concursos | 86 | 2 | vídeo | sem botão | O concurso do Tribunal de Justiça de São Paulo (TJ-SP) é uma das maiores oportunidades para quem tem apenas o ensino médio completo. Além de um excelente salário inicial, você conquista estabilidade financeira, benefício |  |
| Estratégia Concursos | 84 | 2 | vídeo | sem botão | 📢 O professor Herbert Almeida indica: vale a pena estudar para CGU e Tribunal de Contas da União! |  |
| Venâncio & Delgado - Advogados | 58 | 2 | vídeo | sem botão | ⚖️ A banca examinadora pode mudar de entendimento e te eliminar como PCD? Saiba o que o Superior Tribunal de Justiça (STJ) decidiu! |  |
| Milena Correia Advocacia | 23 | 2 | vídeo | sem botão | Irregularidades em concursos públicos podem arruinar seus sonhos! |  |
| Concurseiro aos 40 | 17 | 2 | imagem | sem botão | 🔥 Começar depois dos 40 não significa estar atrasado. |  |
| Gustavo Nogueira - Aprovação Ágil | 14 | 2 | vídeo | sem botão | Funciona — e melhor: não é sorte, é conta. |  |
| Concurseiro aos 40 | 11 (baixo volume) | 2 | imagem | sem botão | 🔥 O TRT-MG já começou a se movimentar para um novo concurso em 2027. |  |
| Monica Freitas MTE | 8 | 2 | imagem | sem botão | ⚖️ O próximo concurso do TRT do Rio Grande do Sul já está em preparação, e esperar o edital sair para começar pode custar um tempo precioso. |  |
| Prof. Ronaldo Santos | 8 | 2 | imagem | sem botão | A Ana Flávia chegou até mim faltando apenas 15 dias para o concurso do Tribunal de Justiça do Rio de Janeiro. |  |
| Caderno do Aprovado - Materiais para Concursos | 924 | 1 | imagem | sem botão | A matéria para concurso já é grande e os cursinhos ainda complicam mais: centenas de horas de videoaulas e milhares de páginas de PDFs. | Simbora Concursos |
| Simbora Concursos | 924 | 1 | carrossel | Visitar perfil do Instagram | Quando eu comecei a estudar para Tribunais, ficar "nas cabeças" era algo inimaginável... 1º lugar, então? Era coisa de maluco, extraterrestre, etc. |  |
| Caderno do Aprovado - Materiais para Concursos | 834 | 1 | carrossel | Visitar perfil do Instagram | Lançados em junho de 2024 |  |
| Caderno do Aprovado - Materiais para Concursos | 785 | 1 | carrossel | Visitar perfil do Instagram | Lançados em agosto de 2024 |  |
| Caderno do Aprovado - Materiais para Concursos | 727 | 1 | carrossel | Visitar perfil do Instagram | CARAAAACA... Quando eu comecei a estudar para Tribunais, eu via esse “TOP 100” como algo inatingível!!! Top 30, Top 20, Top 10 então... Extraterrestres! |  |
| Caderno do Aprovado - Materiais para Concursos | 710 | 1 | carrossel | Visitar perfil do Instagram | Lançados em outubro de 2024 |  |
| Caderno do Aprovado - Materiais para Concursos | 616 | 1 | vídeo | sem botão | 3 cenários de APROVAÇÃO ✅️ |  |
| Caderno do Aprovado - Materiais para Concursos | 616 | 1 | vídeo | sem botão | O caderno de Português do 1º lugar no TRT-PI, com toda a teoria organizada de forma objetiva + questões comentadas das 3 principais bancas de concurso (FCC, FGV e Cespe/Cebraspe). |  |
| Caderno do Aprovado - Materiais para Concursos | 612 | 1 | carrossel | Visitar perfil do Instagram | O tão esperado Caderno do Aprovado da disciplina de Administração Financeira e Orçamentária - AFO (ou Orçamento Público), cada vez mais cobrada em concursos de Tribunais. |  |
| Caderno do Aprovado - Materiais para Concursos | 471 | 1 | imagem | sem botão | Lançados em junho de 2025 |  |
| Projeto Caveira | 325 | 1 | imagem | sem botão | Lançados em novembro de 2025 |  |
| Pódio Tribunais | 198 | 1 | vídeo | sem botão | Você estuda 4, 5 ou até 6 horas por dia e sente que não sai do lugar? |  |
| Concursos Ceisc | 191 | 1 | vídeo | Saiba mais | A sua preparação para o TJ-SP exige foco e direcionamento. |  |
| Concursos Ceisc | 191 | 1 | vídeo | Saiba mais | O edital do concurso do TJ-BA com o cargo de Analista Judiciário pode sair a qualquer momento, e o momento de estudar é agora. 🚀 |  |
| Decorando a Lei Seca Cursos Para Concursos E OAB | 186 | 1 | carrossel | Visitar perfil do Instagram | O art. 319 do Código Penal caiu no concurso para Promotor do MP-GO! |  |

---

# Parte 1 — Ofertas de foco direto (64)

---
id_oferta: 001
anunciante: "MEQ Concursos"
url_destino: "https://meqconcursos.com.br/concurso-simulado-meq-2-analista-trt-v2-l/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1437481675010897"
dias_ativo: 9
anuncios_coletados: 20
anuncios_ativos_estimados: 103
anuncios_com_baixo_volume_de_impressoes: 3
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados, Discursiva / redação, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (5), imagem (15)"
botoes: "sem botão (17), Ver detalhes (2), Saiba mais (1)"
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
termos_foco_encontrados: "trt, tecnico judiciario"
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
anunciante: "Concurseiro aos 40"
url_destino: "https://form.respondi.app/CN2Wk6Lk"
ad_library_url: "https://www.facebook.com/ads/library/?id=2615824408860801"
dias_ativo: 23
anuncios_coletados: 11
anuncios_ativos_estimados: 28
anuncios_com_baixo_volume_de_impressoes: 2
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, justica do trabalho"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "imagem (11)"
botoes: "sem botão (11)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"⚖️ Os próximos concursos de TRTs podem abrir excelentes oportunidades em diferentes regiões do país, com remunerações iniciais que podem chegar a cerca de R$ 16 mil.
📍 Estados como MT, PA, RS e PR já estão no radar de quem busca uma carreira mais estável, valorizada e com alta remuneração na Justiça do Trabalho.
⏰ Mas esperar o edital sair para começar pode significar perder um tempo precioso de preparação.
📚 Quem quer disputar uma vaga de verdade precisa construir base, revisar com método, acompanhar o próprio desempenho e estudar com direção.
🏆 Foi assim que eu consegui ser aprovado em 3 TRTs, mesmo começando depois dos 40.
🎯 Se você quer se preparar de forma estratégica para os próximos concursos de TRTs e buscar uma carreira com remuneração inicial de até R$ 16.000, clique no link e fale comigo"

### Ganchos das variações (1ª linha de cada anúncio)
- ⚖️ Os próximos concursos de TRTs podem abrir excelentes oportunidades em diferentes regiões do país, com remunerações iniciais que podem chegar a cerca de R$ 16 mil.
- 🔥 O TRT-MG já começou a se movimentar para um novo concurso em 2027.
- 🔥 Começar depois dos 40 não significa estar atrasado.

### Landing Page: Headline & Promessa Central
"Inicie o passo mais importante rumo à sua aprovação no Concurso do TRT"

### Entregáveis / Formato (termos encontrados na LP)
- Mentoria


========================================

---
id_oferta: 004
anunciante: "Leandro Reinhardt l Estudos & Concursos"
url_destino: "https://leandroreinhardt.com.br/trt-desafio-nucleo-duro-tjaa/?utm_source=meta-ads&utm_medium=%7B%7Badset.name%7D%7D%7C%7B%7Badset.id%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D%7C%7B%7Bcampaign.id%7D%7D&utm_content=%7B%7Bad.name%7D%7D%7C%7B%7Bad.id%7D%7D&utm_term=%7B%7Bplacement%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1667286944925819"
dias_ativo: 11
anuncios_coletados: 21
anuncios_ativos_estimados: 21
anuncios_com_baixo_volume_de_impressoes: 1
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tjaa"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados"
formatos_dos_anuncios: "imagem (21)"
botoes: "Saiba mais (21)"
precos_exibidos_na_lp: "R$ 297 | R$ 97 | 12x de R$ 9,70"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"<100
33 tópicos, 71% das questões específicas
70 dias, 1 hora por dia, dentro do que a FCC cobra de verdade."

### Ganchos das variações (1ª linha de cada anúncio)
- R$ 12.200 de remuneração inicial
- 33 tópicos, 71% das questões específicas
- 1 hora por dia, depois do trabalho
- Você não precisa do edital inteiro
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
id_oferta: 005
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://www.facebook.com/simboraconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=436273172079349"
dias_ativo: 924
anuncios_coletados: 15
anuncios_ativos_estimados: 15
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trt, tst"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Discursiva / redação"
formatos_dos_anuncios: "carrossel (11), imagem (2), vídeo (2)"
botoes: "Visitar perfil do Instagram (9), sem botão (6)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Lançados em junho de 2025
O MATERIAL QUE FALTAVA PARA SUA NOTA MÁXIMA NA REDAÇÃO!
🤯 Se você se sente assim...
❌ Travou na hora de começar a #redação;
❌ Fica inseguro(a) para desenvolver argumentos fortes;
❌ Não sabe como estruturar um texto que impressione a banca;
❌ Percebe que escreve bem, mas não sai da nota mediana;
❌ Tem pavor de fugir do tema ou perder pontos por detalhes...
💡 Esse material não é só uma apostila. É um guia definitivo, completo, direto e prático para você dominar qualquer tema e garantir sua nota máxima!
🔥 MÉTODO REDAÇÃO IMBATÍVEL
✔️ Como interpretar qualquer tema corretamente;
✔️ Como construir uma tese irrefutável e alinhada;
✔️ Como planejar argumentos fortes, pertinentes e sofisticados;
✔️ Modelos prontos e adaptáveis de introdução, desenvolvimento e conclusão.
✔️ Passo a passo claro e direto para montar textos no nível dos aprovados.
🏛️ BANCO DE REPERTÓRIO DE ALTO NÍVEL
✔️ 50 citações coringas, prontas, explicadas e aplicáveis;
✔️ 25 resumos de livros, filmes e obras essenciais, todos com contexto e modelo de uso na redação;
✔️ Repertórios exclusivos de autores brasileiros como Milton Santos, Darcy Ribeiro, Caio Prado Jr., Jorge Caldeira, Eduardo Giannetti, e muito mais.
✍️ MICROESTRUTURA TEXTUAL — O SEGREDO DOS TEXTOS NOTA MÁXIMA
✔️ Como iniciar períodos de forma variada e elegante;
✔️ Como evitar cacofonias, pleonasmos e repetições que derrubam sua nota;
✔️ Técnicas para construir períodos compostos claros, sofisticados e com fluidez;
✔️ Checklist prático para garantir clareza, coesão, objetividade e linguagem formal.
🔗 GUIA COMPLETO DE CONECTIVOS — SUA REDAÇÃO 100% COESA E SOFISTICADA
✔️ Expressões inteligentes para iniciar, desenvolver, transitar entre argumentos e concluir com impacto.
✔️ Acabe de vez com textos repetitivos, rasos e sem progressão textual.
✔️ Seu texto se torna fluido, maduro e com padrão profissional.
✔️ Mais de 150 conectivos e operadores argumentativos organizados por função.
🏆 PROPOSTAS INÉDITAS E COMPLETAS
✔️ Temas atuais, exigentes e no nível das principais bancas;
✔️ Cada proposta contém:
Contextualização perfeita;
Citações prontas;
Argumentos planejados;
Modelo de redação completa no padrão nota máxima."

### Ganchos das variações (1ª linha de cada anúncio)
- Comente MPPE e receba também! 🎁
- Não sei se a ficha já caiu por aí, mas vocês serão servidores públicos do Poder Judiciário cearense. 😮🙏👏
- Lançados em junho de 2024
- CARAAAACA... Quando eu comecei a estudar para Tribunais, eu via esse “TOP 100” como algo inatingível!!! Top 30, Top 20, Top 10 então... Extraterrestres!
- O tão esperado Caderno do Aprovado da disciplina de Administração Financeira e Orçamentária - AFO (ou Orçamento Público), cada vez mais cobrada em concursos de Tribunais.
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
id_oferta: 006
anunciante: "Leandro Reinhardt l Estudos & Concursos"
url_destino: "https://leandroreinhardt.com.br/trt-desafio-nucleo-duro/?utm_source=meta-ads&utm_medium=%7B%7Badset.name%7D%7D%7C%7B%7Badset.id%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D%7C%7B%7Bcampaign.id%7D%7D&utm_content=%7B%7Bad.name%7D%7D%7C%7B%7Bad.id%7D%7D&utm_term=%7B%7Bplacement%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1383702350413675"
dias_ativo: 11
anuncios_coletados: 14
anuncios_ativos_estimados: 14
anuncios_com_baixo_volume_de_impressoes: 4
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados"
formatos_dos_anuncios: "imagem (14)"
botoes: "Saiba mais (14)"
precos_exibidos_na_lp: "R$ 297 | R$ 97 | 12x de R$ 9,70"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"<100
29 tópicos concentram 72% das específicas
70 dias, 1 hora por dia, com o Mapa de Engenharia Reversa da FCC."

### Ganchos das variações (1ª linha de cada anúncio)
- Domine o núcleo duro dos TRTs em 70 dias
- Não falta tempo. Falta direção.
- 29 tópicos concentram 72% das específicas
- <100
- De R$ 297 por R$ 97, menos de R$ 1,40 por dia

### Landing Page: Headline & Promessa Central
"72% das questões específicas estão em 29 tópicos . E é isso o que vai decidir sua aprovação. — Mapeamos as questões do Núcleo Duro que a FCC cobrou nos TRTs dos últimos 5 anos. Em 70 dias, você se desafia a dominar esses tópicos."

### Seções da Landing Page (títulos, na ordem)
- Você já sabe estudar. O problema é que nunca teve o mapa certo.
- O Núcleo Duro te mostra o que a banca cobra de verdade, e onde vale a pena se aprofundar.
- 2.819 questões analisadas
- 29 tópicos favoritos da FCC
- Padrões que se repetem
- Profundidade na medida certa
- Disciplinas do Núcleo Duro
- O que não está no Desafio
- Os dados que provam o que você vai estudar.
- Processo Civil
- Direito Constitucional
- Direito do Trabalho
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

### Seção "Para Quem NÃO É" (declarado na LP)
- ×acredita que passar em TRT é só assistir videoaulas do cursinho×quer mais um material para colecionar sem executar×não está disposto à rotina diária de 70 dias

### Entregáveis / Formato (termos encontrados na LP)
- Mentoria
- Simulados
- Videoaulas


========================================

---
id_oferta: 007
anunciante: "Portal & OAB"
url_destino: "https://olympus.cursosdoportal.com.br/o-adm-trt-pa/?utm_source=%7B%7Bsite_source_name%7D%7D&utm_medium=%7B%7Badset.name%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D&utm_term=%7B%7Bplacement%7D%7D&utm_content=%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1074976398625545"
dias_ativo: 10
anuncios_coletados: 11
anuncios_ativos_estimados: 11
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tribunal regional do trabalho, trt 8, tecnico judiciario"
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
id_oferta: 008
anunciante: "Portal Concursos"
url_destino: "https://oportalconcursos.com.br/h-adm-trt-mt/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1436015981795868"
dias_ativo: 8
anuncios_coletados: 11
anuncios_ativos_estimados: 11
anuncios_com_baixo_volume_de_impressoes: 2
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tribunal regional do trabalho, tecnico judiciario"
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
id_oferta: 009
anunciante: "Vinco Leilões"
url_destino: "https://www.vincoleiloes.com.br/lote.php?idLote=7315"
ad_library_url: "https://www.facebook.com/ads/library/?id=1749137523049974"
dias_ativo: 8
anuncios_coletados: 9
anuncios_ativos_estimados: 9
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt2"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "carrossel (8), imagem (1)"
botoes: "Enviar mensagem pelo WhatsApp (9)"
precos_exibidos_na_lp: "R$ 3.500.000,00 | R$ 1.750.000,00 | R$ 87.500,00"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🏢 Sala comercial em Tamboré/Barueri em leilão judicial
Oportunidade no 709º Leilão Judicial Unificado do TRT2.
Escritório localizado no Edifício Office Tamboré, integrante do Condomínio Shopping Center Tamboré.
📍 Tamboré – Barueri/SP
🏢 10º andar
📐 42,12 m² de área privativa
💰 Avaliação: R$ 530.000
🔨 Lance mínimo: R$ 265.000
Busca um imóvel comercial na região de Tamboré?
📲 Fale com a equipe da Vinco pelo WhatsApp para receber mais informações e entender como participar do leilão.
🌐 Você também pode acessar o site da Vinco para consultar a descrição completa do lote, edital e condições do leilão: https://www.vincoleiloes.com.br/lote.php?idLote=7399
WHATSAPP
Sala comercial em Tamboré | Lance a partir de R$ 265 mil
42,12 m² privativos no Office Tamboré. Consulte as condições do leilão."

### Ganchos das variações (1ª linha de cada anúncio)
- 🏙️ Apartamento de 254,96 m² no Jardim Paulista com lance mínimo de R$ 1,75 milhão
- 🏢 Imóvel comercial em Itaquaquecetuba com lance mínimo de R$ 1,26 milhão
- 🌳 Grande área em Santana de Parnaíba com lance mínimo de R$ 10 milhões
- 🏭 Galpão comercial em Campinas com lance mínimo de R$ 1,32 milhão
- 🏡 Casa no Jardim Morumbi com lance mínimo 60% abaixo do valor de avaliação
- 🏢 Apartamento em Alphaville com lance mínimo de R$ 475 mil

### Títulos do link nos anúncios
- Apto no Jardim Paulista | Lance mínimo R$ 1,75 mi
- Imóvel em Itaquaquecetuba | Lance mínimo R$ 1,26 mi
- Área de 480 mil m² em Santana de Parnaíba | R$ 10 mi
- Galpão em Campinas | Lance mínimo R$ 1,32 mi
- Casa no Morumbi | Lance mínimo R$ 2,136 milhões
- Apartamento em Alphaville | Lance a partir de R$ 475 mil

### Landing Page: Headline & Promessa Central
"708º LEILÃO JUDICIAL UNIFICADO DO TRT2 - GRANDE LEILÃO DE IMÓVEIS , VEÍCULOS E DIVERSOS (CÓDIGO 447) — Vinco® 2026 - Todos os direitos reservados."

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 010
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
id_oferta: 011
anunciante: "Trteiros"
url_destino: "https://www.facebook.com/61560675890210/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1931729394374222"
dias_ativo: 167
anuncios_coletados: 5
anuncios_ativos_estimados: 7
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Curso em videoaulas, Material em PDF / apostila / caderno"
formatos_dos_anuncios: "imagem (2), vídeo (3)"
botoes: "sem botão (5)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"TRT RS e o TRT PA-AP estão realizando a contratação da banca FCC para gerenciar o novo concurso de servidores.
Previsão de publicação de edital iminente para o TRT RS e o PA-AP 🥳
.
O objetivo dos TRTeiros é dominar as classificações nas cabeças.
.
Os materiais + mentoria dos TRTeiros ajudarão você a encurtar o caminho até a aprovação 📚📚
Venha estudar com o curso que mais cresceu na última onda de TRT no ano de 2025 e que sabe como te preparar para a aprovação entre os primeiros classificados nos concursos de TRT no ano de 2026🥇🥇🥇
.
O curso TRTeiros é uma grande comunidade 🧡📚🚀"

### Ganchos das variações (1ª linha de cada anúncio)
- TRT RS e o TRT PA-AP estão realizando a contratação da banca FCC para gerenciar o novo concurso de servidores.
- 🚨Informações sobre o TRT/MG
- 🚨Informações sobre o TRT/BA
- Transparência da UE
- A metodologia do curso TRTeiros é o que está faltando na sua aprovação 🧡📚🚀

### Títulos do link nos anúncios
- instagram.com

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 012
anunciante: "Gazeta dos Concursos"
url_destino: "https://lp.aprovacaoagil.com.br/vsl-white-trt-rs"
ad_library_url: "https://www.facebook.com/ads/library/?id=2330834957742562"
dias_ativo: 14
anuncios_coletados: 2
anuncios_ativos_estimados: 6
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tst"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados, Lei seca / legislação, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (2)"
botoes: "sem botão (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Atravessei a faculdade de Direito decorando manual, virando noites, com a sensação de que estudar é sofrer. Quando comecei a pensar em TRT, achei que ia ser mais do mesmo.
Não é. A prova do TRT não premia quem sofreu mais nem quem leu mais — premia quem acerta mais questão no mesmo tempo. O erro número um de quem vem do Direito é ler a teoria inteira antes de encarar uma primeira questão. É a ordem que mais cansa e que menos rende.
Inverte: começa pela questão comentada, usa o gabarito pra enxergar o que a prova cobra, e só depois vai na lei seca. Concentra fogo, por exemplo, nos 3 temas que respondem por 73% das questões de Direito do Trabalho.
O raciocínio jurídico que a faculdade te deu joga a favor na ordem certa. Técnico entra em R$ 11.500, e a base serve pros 24 TRTs e pro TST.
Clica no botão e assiste a aula gratuita enquanto ela está no ar."

### Landing Page: Headline & Promessa Central
"Título"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 013
anunciante: "Monica Freitas MTE"
url_destino: "https://form.respondi.app/yLeg4HU6"
ad_library_url: "https://www.facebook.com/ads/library/?id=4497844090493414"
dias_ativo: 8
anuncios_coletados: 4
anuncios_ativos_estimados: 6
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Questões / simulados, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (4)"
botoes: "sem botão (2), Saiba mais (2)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"⚖️ O próximo concurso do TRT do Rio Grande do Sul já está em preparação, e esperar o edital sair para começar pode custar um tempo precioso.
Quem quer chegar competitivo precisa aproveitar o pré-edital para construir base, organizar as disciplinas e criar constância nos estudos.
Na Mentoria MTE, eu te ajudo a organizar essa preparação de acordo com a sua realidade.
✅ Planejamento personalizado
✅ Direcionamento dos estudos
✅ Metas adaptadas à sua rotina
✅ Acompanhamento da evolução
✅ Estratégia de revisões e questões
✅ Método MTE: Mente, Técnica e Execução
Você não precisa estudar no improviso e muito menos esperar o edital para descobrir por onde começar.
👉 Clique em Saiba Mais e conheça a minha mentoria."

### Landing Page: Headline & Promessa Central
"Mentoria MTE | Formulário de Aplicação"

### Entregáveis / Formato (termos encontrados na LP)
- Mentoria


========================================

---
id_oferta: 014
anunciante: "MEQ Concursos"
url_destino: "https://www.facebook.com/61586241338760/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1652434139167708"
dias_ativo: 141
anuncios_coletados: 5
anuncios_ativos_estimados: 5
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trt, trt4, trt 4, tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (1), carrossel (1), vídeo (3)"
botoes: "sem botão (4), Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
- Alguns TRTs estão entrando em uma fase decisiva. 👀
- Tem tribunal com banca em definição, grupo de trabalho formado, concurso prorrogado e validade chegando ao fim. Não é promessa de edital imediato, mas é cenário para acompanhar de perto.
- Vale a reflexão: nas próximas provas de TRT, talvez a pergunta não seja “como eu faço para passar?”, mas “como eu estudo para ser nomeado?”. Parece detalhe, mas essa mudança de cabeça pode separar quem fica no quase de q
- “TRT não vale a pena…”

### Títulos do link nos anúncios
- www.instagram.com

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 015
anunciante: "Gazeta dos Concursos"
url_destino: "https://lp.aprovacaoagil.com.br/vsl-white-trt-noticia"
ad_library_url: "https://www.facebook.com/ads/library/?id=2150289195888138"
dias_ativo: 76
anuncios_coletados: 5
anuncios_ativos_estimados: 5
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tst"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno, Lei seca / legislação"
formatos_dos_anuncios: "vídeo (5)"
botoes: "Saiba mais (5)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
- A maior leva de TRTs da última década está entrando na fila. 14 provas até o final de 2027 — uma atrás da outra.
- Qual concurso te bota mais rápido em R$11.500 iniciais com qualquer graduação — inclusive tecnólogo?
- "Trabalho 8 horas e ainda tenho família. Sobram 2 horas por dia pra estudar. TRT com 2 horas dá?"
- "Quero muito passar num TRT, começo por onde?"

### Títulos do link nos anúncios
- Melhor tribunal pra começar hoje
- A enxurrada de TRTs começou
- O caminho mais rápido pra R$11.500
- TRT dá com 2 horas por dia?
- Quero passar num TRT — por onde?

### Landing Page: Headline & Promessa Central
"Título"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 016
anunciante: "Isaque Concursos"
url_destino: "https://projetotrt.com.br/vsl1v1/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1023281740551609"
dias_ativo: 62
anuncios_coletados: 5
anuncios_ativos_estimados: 5
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tecnico judiciario"
plataforma_checkout: "onprofit"
ticket_principal: "R$ 497,00"
fonte_ticket: "checkout"
tipos_produto: "Mentoria / acompanhamento, Cronograma / plano de estudos"
formatos_dos_anuncios: "vídeo (5)"
botoes: "Saiba mais (5)"
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
id_oferta: 017
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
id_oferta: 018
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2089-concurso-trt-4-club-analista-judiciario-area-judiciaria"
ad_library_url: "https://www.facebook.com/ads/library/?id=2796129990724803"
dias_ativo: 166
anuncios_coletados: 4
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trt, trt 4"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Curso em videoaulas, Material em PDF / apostila / caderno, Questões / simulados, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (4)"
botoes: "Saiba mais (3), Ver detalhes (1)"
precos_exibidos_na_lp: "R$ 16 | R$ 16.041,21 | R$ 10 | R$ 2.137,00 | R$ 1.389,05 | 12x de R$ 115,75"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Uma nova remuneração que pode transformar sua vida!
E para chegar lá, você precisa da preparação que o o Club Ceisc tem, confira:
✅ Garantia de atualização do curso na fase pós-edital
✅ Professores especialistas em concursos de Tribunais
✅ Simulados com gabarito comentado
✅ Mentorias ao vivo
✅ Aulas de resolução de questões
✅ Cronogramas de estudos
✅ Banco de questões e planner interativo
✅ Cadernos de lei
Comece agora a sua preparação para o cargo de Analista do Judiciário.
Garanta sua Vaga
Ceisc Concursos"

### Ganchos das variações (1ª linha de cada anúncio)
- A sua oportunidade de atuar no estado do Rio Grande do Sul, pelo Tribunal Regional do Trabalho, está chegando!
- O TRT-4 pode estar prestes a anunciar um novo concurso!
- Se preparar para tribunais exige método.
- Uma nova remuneração que pode transformar sua vida!

### Títulos do link nos anúncios
- Garanta sua Vaga

### Landing Page: Headline & Promessa Central
"TRT-4 Club | Analista Judiciário - Área Judiciária — Sobre o curso"

### Seções da Landing Page (títulos, na ordem)
- Sobre o curso
- Nesse curso você terá
- Conheça os professores
- Sobre a prova
- Conteúdo Programático
- Perguntas frequentes
- Confira as últimas notícias do nosso blog

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Mentoria
- Planner
- Simulados
- Videoaulas


========================================

---
id_oferta: 019
anunciante: "Meirelles Quintella Escritório de Advocacia"
url_destino: "https://www.facebook.com/100090050235471/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2118332055398747"
dias_ativo: 155
anuncios_coletados: 2
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "justica do trabalho"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "vídeo (2)"
botoes: "sem botão (1), Saiba mais (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Área da Saúde"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Alguns profissionais da área da saúde atuam em hospitais públicos sem ter ingressado por concurso.
Em determinadas situações, a Justiça do Trabalho pode reconhecer direitos como FGTS, adicional de insalubridade e diferenças salariais.
Quer entender melhor como isso funciona? Clique em “Saiba mais”."

### Títulos do link nos anúncios
- Meirelles e Quintella

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 020
anunciante: "Nova Concursos"
url_destino: "https://aprovacao.novaconcursos.com.br/curso-gratis-tj-sp-ads"
ad_library_url: "https://www.facebook.com/ads/library/?id=1742296783853552"
dias_ativo: 114
anuncios_coletados: 2
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Questões / simulados, Cronograma / plano de estudos, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (2)"
botoes: "Saiba mais (2)"
precos_exibidos_na_lp: "R$ 297,00 | R$ 0,00"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
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
id_oferta: 021
anunciante: "Ceisc Concursos"
url_destino: "https://lp.ceisc.com.br/projeto-nomeacao-tj-sp/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2095494471007965"
dias_ativo: 87
anuncios_coletados: 4
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "sympla"
ticket_principal: "R$ 6.345,94"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (4)"
botoes: "Ver detalhes (2), Solicitar agora (1), Inscreva-se (1)"
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
id_oferta: 022
anunciante: "Gustavo Nogueira - Aprovação Ágil"
url_destino: "https://lp.aprovacaoagil.com.br/vsl-white-trt-pa-ap"
ad_library_url: "https://www.facebook.com/ads/library/?id=1051146427756845"
dias_ativo: 14
anuncios_coletados: 2
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tst"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (2)"
botoes: "sem botão (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Funciona — e melhor: não é sorte, é conta.
O que trava a maioria é achar que pra passar tem que saber a matéria inteira. Você abre o edital gigante, tenta decorar tudo e chega no dia da prova travado, porque nunca treinou como a banca cobra.
O truque do gabarito faz o contrário. Você pega a questão já comentada, abre o gabarito e faz a engenharia reversa da cabeça de quem elaborou: que pegadinha ele armou, que palavra muda tudo. A lei você lê depois, já entendendo pra que serve cada artigo.
E funciona pro TRT-8 pelo mesmo motivo que funciona nos outros tribunais: em Direito do Trabalho, 3 temas respondem por 73% das questões. Em vez de espalhar energia, você concentra fogo onde a prova cai. E a mesma preparação serve pros 24 TRTs e o TST — técnico entra em R$ 11.500.
Clica no botão e assiste a aula gratuita enquanto ela está no ar."

### Landing Page: Headline & Promessa Central
"Título"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 023
anunciante: "Prime Curso"
url_destino: "https://sala.concurseiroprime.com.br/buscar?query=trt"
ad_library_url: "https://www.facebook.com/ads/library/?id=1129411490041604"
dias_ativo: 13
anuncios_coletados: 4
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tribunal regional do trabalho, trt8, trt22, tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "imagem (4)"
botoes: "Comprar agora (4)"
precos_exibidos_na_lp: "R$ 42,00 | 10x de R$ 42,00 | R$ 1200 | R$ 378,00 | R$ 49,00 | 10x de R$ 49,00 | R$ 1400 | R$ 441,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
id_oferta: 024
anunciante: "Escola Trabalhista"
url_destino: "https://escolatrabalhista.com.br/preparacao-acesso-total-trt-tst/"
ad_library_url: "https://www.facebook.com/ads/library/?id=838276629301718"
dias_ativo: 185
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trt, tst, tecnico judiciario"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 2.746,65"
fonte_ticket: "checkout"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "vídeo (2), imagem (1)"
botoes: "Comprar agora (2), Saiba mais (1)"
parcelas: "12x de R$ 284,07"
precos_exibidos_na_lp: "R$ 1,00 | R$ 2.746,65 | 12x de R$ 284,07"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O Acesso Total TRT/TST é uma formação completa pensada exatamente para quem vai disputar vagas de técnico judiciário e analista judiciário. Conteúdo organizado por trilhas, materiais atualizados e foco absoluto na jurisprudência e no estilo de prova dos Tribunais do Trabalho.
Estude com método profissional e chegue competitivo para o próximo edital."

### Ganchos das variações (1ª linha de cada anúncio)
- O Acesso Total TRT/TST é uma formação completa pensada exatamente para quem vai disputar vagas de técnico judiciário e analista judiciário. Conteúdo organizado por trilhas, materiais atualizados e foco absoluto na jurisp
- O Acesso Total TRT/TST foi criado para quem se prepara de forma estratégica para as provas da área trabalhista, especialmente para os cargos de analista judiciário e técnico judiciário.

### Títulos do link nos anúncios
- ACESSO TOTAL TRT/TST – Escola Trabalhista

### Landing Page: Headline & Promessa Central
"PREPARAÇÃO ACESSO TOTAL TRT/TST — Junte-se a mais de 12.000 alunos"

### Seções da Landing Page (títulos, na ordem)
- Você não precisa escolher um único concurso para focar.
- Esteja pronto e multiplique suas chances de aprovação!
- Um único investimento e acesso a todos os cursos de Técnico e Analista da Escola Trabalhista por 2 anos, que é o tempo médio de aprovação.
- Como funciona o Acesso Total?
- Veja tudo que você terá acesso:
- ✅ Com o Acesso Total, você não vai precisar gastar mais R$ 1,00 com outros cursos durante dois anos.
- O que dizem os alunos
- Mais depoimentos
- Um plano comprovadamente eficiente
- Vamos te colocar dentro dos 5% dos candidatos que realmente concorrem às vagas
- Três são os elementos
- que irão te deixar à frente dos concorrentes, potencializando sua chances de aprovação
- Metodologia Exclusiva
- Atualização Constante
- O que você vai receber
- Metas diárias e cronograma de estudos
- Questões objetivas comentadas
- Central de dúvidas exclusiva
- Ciclos de revisão
- Legislação Destacada
- Resumos dos principais pontos do edital
- Módulos de videoaulas
- Bônus: Temas Fundamentais: Discriminação e Assédio para concursos Trabalhistas
- E-books de Informativos do TST
- E-books de súmulas e OJs do TST
- Acesso a todos os cursos Pré-edital
- Acesso a todos os cursos Reta Final
- Acesso a todos os cursos de Preparação Discursiva
- Acesso a todos os outros cursos para Técnico e Analista disponíveis na plataforma
- Atualização Constante do material

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Discursiva / redação
- PDF
- Resumos
- Simulados
- Videoaulas


========================================

---
id_oferta: 025
anunciante: "prof.camilasabongi com Escola Trabalhista"
url_destino: "https://escolatrabalhista.com.br/preparacao-acesso-total-trt-tst/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1278772247787449"
dias_ativo: 181
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trt, tst, tecnico judiciario"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 2.746,65"
fonte_ticket: "checkout"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "vídeo (3)"
botoes: "Saiba mais (2), Comprar agora (1)"
parcelas: "12x de R$ 284,07"
precos_exibidos_na_lp: "R$ 1,00 | R$ 2.746,65 | 12x de R$ 284,07"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O Acesso Total TRT/TST é uma formação completa pensada exatamente para quem vai disputar vagas de técnico judiciário e analista judiciário. Conteúdo organizado por trilhas, materiais atualizados e foco absoluto na jurisprudência e no estilo de prova dos Tribunais do Trabalho.
Estude com método profissional e chegue competitivo para o próximo edital."

### Ganchos das variações (1ª linha de cada anúncio)
- O Acesso Total TRT/TST foi criado para quem se prepara de forma estratégica para as provas da área trabalhista, especialmente para os cargos de analista judiciário e técnico judiciário.
- O Acesso Total TRT/TST é uma formação completa pensada exatamente para quem vai disputar vagas de técnico judiciário e analista judiciário. Conteúdo organizado por trilhas, materiais atualizados e foco absoluto na jurisp

### Títulos do link nos anúncios
- prof.camilasabongi

### Landing Page: Headline & Promessa Central
"PREPARAÇÃO ACESSO TOTAL TRT/TST — Junte-se a mais de 12.000 alunos"

### Seções da Landing Page (títulos, na ordem)
- Você não precisa escolher um único concurso para focar.
- Esteja pronto e multiplique suas chances de aprovação!
- Um único investimento e acesso a todos os cursos de Técnico e Analista da Escola Trabalhista por 2 anos, que é o tempo médio de aprovação.
- Como funciona o Acesso Total?
- Veja tudo que você terá acesso:
- ✅ Com o Acesso Total, você não vai precisar gastar mais R$ 1,00 com outros cursos durante dois anos.
- O que dizem os alunos
- Mais depoimentos
- Um plano comprovadamente eficiente
- Vamos te colocar dentro dos 5% dos candidatos que realmente concorrem às vagas
- Três são os elementos
- que irão te deixar à frente dos concorrentes, potencializando sua chances de aprovação
- Metodologia Exclusiva
- Atualização Constante
- O que você vai receber
- Metas diárias e cronograma de estudos
- Questões objetivas comentadas
- Central de dúvidas exclusiva
- Ciclos de revisão
- Legislação Destacada
- Resumos dos principais pontos do edital
- Módulos de videoaulas
- Bônus: Temas Fundamentais: Discriminação e Assédio para concursos Trabalhistas
- E-books de Informativos do TST
- E-books de súmulas e OJs do TST
- Acesso a todos os cursos Pré-edital
- Acesso a todos os cursos Reta Final
- Acesso a todos os cursos de Preparação Discursiva
- Acesso a todos os outros cursos para Técnico e Analista disponíveis na plataforma
- Atualização Constante do material

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Discursiva / redação
- PDF
- Resumos
- Simulados
- Videoaulas


========================================

---
id_oferta: 026
anunciante: "Professor Fabiano Pereira"
url_destino: "https://www.facebook.com/professorfp/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1622749052884640"
dias_ativo: 17
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Material em PDF / apostila / caderno, Questões / simulados"
formatos_dos_anuncios: "vídeo (2), carrossel (1)"
botoes: "sem botão (2), Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Tem um detalhe do TRT do Rio Grande do Sul que diz mais do que qualquer previsão de edital.
Em julho de 2026 o tribunal contratou o Banco do Brasil para processar as taxas de inscrição do próximo concurso. A estimativa contratada foi de 50 mil pagamentos. No concurso anterior foram 35.894 inscritos. Ou seja, o próprio tribunal está se preparando para quase 40% a mais de gente na disputa.
E olha o tamanho da ironia: o concurso já foi autorizado, a comissão já está formada, a operadora da taxa já foi contratada, mas a banca ainda não foi divulgada oficialmente e não existe data para o edital (apesar de a expectativa ser para as próximas semanas).
É exatamente aí que mora a sua chance. Enquanto a data não vem, você tem tempo tranquilo para aprender de verdade. Quando o edital sair, esse tempo acaba para todo mundo ao mesmo tempo.
O plano certo é chegar no dia da publicação com o conteúdo já estudado. A partir dali o seu dia deixa de ser aprender matéria nova e passa a ser revisar e resolver o máximo de questões possível.
Se você quer disputar o TRT RS com um caminho pronto e acompanhamento de perto, digite EU QUERO aqui nos comentários que eu te explico como funciona a minha MENTORIA."

### Ganchos das variações (1ª linha de cada anúncio)
- Estudar sozinho não significa estudar sem direção.
- Tem um detalhe do TRT do Rio Grande do Sul que diz mais do que qualquer previsão de edital.
- Já tentou o TRT-RS 3 vezes e não passou? Será que ainda vale a pena tentar de novo?

### Títulos do link nos anúncios
- Fabiano Pereira | Concursos de Tribunais (@fabianopereiraprof) • Instagram photos and videos

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 027
anunciante: "Verbo Carreiras Jurídicas"
url_destino: "https://www.facebook.com/verbocarreirasjuridicas/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1110449348094847"
dias_ativo: 15
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 1
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Material em PDF / apostila / caderno, Lei seca / legislação, Discursiva / redação"
formatos_dos_anuncios: "vídeo (3)"
botoes: "Enviar mensagem pelo WhatsApp (3)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Língua Portuguesa e Redação com quem entende de aprovação para o concurso do TRT-4
São 50 encontros, mentorias com especialistas e Vade Mecum incluso na modalidade presencial e muito mais!
Para passar, tem que ser Verbo!"

### Ganchos das variações (1ª linha de cada anúncio)
- Língua Portuguesa e Redação com quem entende de aprovação para o concurso do TRT-4
- <100

### Títulos do link nos anúncios
- Por menos de R$5,00 ao dia você aprende Língua Portuguesa para o concurso do TRT-4!
- Se prepare com quem entende de APROVAÇÃO!

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 028
anunciante: "Professor Raphael Reis"
url_destino: "https://www.facebook.com/profraphaelreis/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1494830749215441"
dias_ativo: 8
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Questões / simulados, Discursiva / redação"
formatos_dos_anuncios: "imagem (2), carrossel (1)"
botoes: "sem botão (2), Visitar perfil do Instagram (1)"
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

### Ganchos das variações (1ª linha de cada anúncio)
- 🔴No universo dos concursos públicos, muitos candidatos concentram sua energia quase exclusivamente nas questões objetivas. De fato, elas são essenciais: funcionam como filtro inicial, abrindo a porta para as etapas segui
- Historicamente, desde 2018, os melhores resultados são dos meus alunos 🧙‍♂️
- Concorda com a classificação do Prof. Rapha? rsrs

### Títulos do link nos anúncios
- instagram.com

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 029
anunciante: "Gustavo Nogueira - Aprovação Ágil"
url_destino: "https://pages.aprovacaoagil.com.br/vsl/trt/v01"
ad_library_url: "https://www.facebook.com/ads/library/?id=1762089464999221"
dias_ativo: 8
anuncios_coletados: 1
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
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
id_oferta: 030
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
id_oferta: 031
anunciante: "Concursosmeucurso"
url_destino: "https://meucurso.com.br/categorias/concursos-publicos-escrevente--tjsp"
ad_library_url: "https://www.facebook.com/ads/library/?id=941559835572125"
dias_ativo: 112
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
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
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
id_oferta: 032
anunciante: "Brabo Concursos"
url_destino: "https://www.facebook.com/braboconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=4583317258660193"
dias_ativo: 92
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
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
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
id_oferta: 033
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2138-concurso-trt-4-club-tecnico-judiciario-area-administrativa?utm_source=meta_ads&utm_medium=cpc&utm_campaign=vendas_trt_4_club_tec_judiciario&utm_term=advantage"
ad_library_url: "https://www.facebook.com/ads/library/?id=1020843757391368"
dias_ativo: 85
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt 4, tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Curso em videoaulas, Questões / simulados, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (2)"
botoes: "Saiba mais (2)"
precos_exibidos_na_lp: "R$ 9 | R$ 9.776,71 | R$ 10 | R$ 1.797,00 | R$ 1.168,05 | 12x de R$ 97,34"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
id_oferta: 034
anunciante: "Prof. Bruno Klippel"
url_destino: "http://www.brunoklippel.com.br/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1660718711665340"
dias_ativo: 77
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "carrossel (2)"
botoes: "Comprar agora (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Quer ser aprovado em um concurso de TRT?
Conheça os meus e-books desenvolvidos para ajudar você a estudar com mais organização, compreender os principais temas de Direito do Trabalho e Processo do Trabalho e revisar de forma estratégica.
São materiais objetivos, didáticos e direcionados para quem deseja melhorar o desempenho nas provas dos Tribunais Regionais do Trabalho.
Escolha o material ideal para a sua preparação e dê mais um passo em direção à aprovação.
Acesse: [www.brunoklippel.com.br](http://www.brunoklippel.com.br)"

### Títulos do link nos anúncios
- Prof. Bruno Klippel - Você no mundo trabalhista

### Landing Page: Headline & Promessa Central
[não capturada — status da LP: fetch_failed]

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 035
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://cadernodoaprovado.com/trf-tj-mp/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1533733075435407"
dias_ativo: 65
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 497,00"
fonte_ticket: "checkout"
tipos_produto: "Material em PDF / apostila / caderno, Mapas mentais / esquemas, Lei seca / legislação"
formatos_dos_anuncios: "imagem (1), carrossel (1)"
botoes: "Ver detalhes (1), sem botão (1)"
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
id_oferta: 036
anunciante: "Instituto INAPI"
url_destino: "https://cursos.inapionline.com.br/pre-trt-pi"
ad_library_url: "https://www.facebook.com/ads/library/?id=1364004345923443"
dias_ativo: 52
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tecnico judiciario"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 827,00"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Questões / simulados, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (1), imagem (1)"
botoes: "Saiba mais (1), Ver detalhes (1)"
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
id_oferta: 037
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://cadernodoaprovado.com/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1808412633912288"
dias_ativo: 30
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno, Questões / simulados, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (2)"
botoes: "Ver detalhes (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Estude com o 1º lugar no TRT-22 🏆
São mais de 10.000 concurseiros estudando com o Caderno do Aprovado 📚
✅ Materiais de estudos para Tribunais:
• Meus cadernos de todas as disciplinas
• Cronograma flexível
• Metas de estudos
• Planilha de controle
• Links para videoaulas
• Links para questões
• Revisões programadas
• Estratégia de reta final
✅ Meu direcionamento em TODAS as matérias
✅ SUPORTE no Whatsapp
✅ ATUALIZAÇÕES no pós-edital
Clique em SAIBA MAIS e prepare-se em alto nível para os próximos concursos!"

### Títulos do link nos anúncios
- Caderno do Aprovado – Materiais de estudos para concursos públicos

### Landing Page: Headline & Promessa Central
"Caderno do Aprovado – Materiais de estudos para concursos públicos — Prepare-se em alto nível estudando com o 1º lugar ."

### Seções da Landing Page (títulos, na ordem)
- Prepare-se em alto nível estudando com o 1º lugar .
- 1º lugar
- O Caderno do Aprovado resolve isso organizando tudo em um só lugar.
- Tudo pronto para estudar, revisar e avançar.
- A diferença está em quem faz e em como é feito.
- Conheça por dentro.
- Você estuda para qual concurso?
- Oi, eu sou o Beto.
- O material de estudos dos primeiros colocados!
- Estudar sozinho x Estudar com o Caderno do Aprovado
- Sem riscos, com garantia de 7 dias para ter certeza.
- Dúvidas frequentes e suas respostas.
- Outras dúvidas?
- Por aqui, tudo pronto. Agora é contigo.

### Entregáveis / Formato (termos encontrados na LP)
- Caderno de erros
- Cronograma
- PDF
- Resumos
- Videoaulas


========================================

---
id_oferta: 038
anunciante: "Weverton Reis"
url_destino: "https://www.facebook.com/100070415432523/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1069790249007641"
dias_ativo: 14
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "imagem (1), vídeo (1)"
botoes: "Enviar mensagem pelo WhatsApp (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🏙️ Apartamento de 103 m² no Setor Bueno, com 3 suítes plenas, andar alto e excelente custo-benefício para a região.
📍 Matiz Bueno | Próximo ao TRT | Setor Bueno
▪️ 103 m² privativos
▪️ 3 suítes plenas
▪️ Varanda gourmet ampla com churrasqueira a gás
▪️ Apartamento nascente
▪️ Andar alto
▪️ 2 vagas paralelas
▪️ Lazer completo
▪️ Possibilidade de venda mobiliado
💰 R$ 930.000
✨ Uma planta que aproveita muito bem os espaços, com ambientes amplos para viver e receber com conforto.
📲 Entre em contato e agende sua visita.
WHATSAPP
Custo-benefício no Bueno"

### Títulos do link nos anúncios
- Custo-benefício no Bueno

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 039
anunciante: "GG Concursos"
url_destino: "https://ggconcursos.com.br/cursos/trt4/?cupom=GG-30"
ad_library_url: "https://www.facebook.com/ads/library/?id=2193032804613934"
dias_ativo: 13
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tribunal regional do trabalho, trt4"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "imagem (2)"
botoes: "Comprar agora (2)"
precos_exibidos_na_lp: "R$ 9.000,00 | R$ 890,00 | R$ 483,00 | 12x de R$ 40 | R$ 690,00 | R$ 413,00 | 12x de R$ 34 | R$ 16.000,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Prepare-se para o concurso do Tribunal Regional do Trabalho (TRT4) com o GG. Clique e comece hoje mesmo!"

### Títulos do link nos anúncios
- Curso TRT4 30% OFF

### Landing Page: Headline & Promessa Central
"GG Concursos - Disruptivos e humanos! Assim somos GG!"

### Seções da Landing Page (títulos, na ordem)
- Benefícios do GG
- Professores
- Exclusivos
- o que nossos alunos dizem

### Entregáveis / Formato (termos encontrados na LP)
- Simulados
- Videoaulas


========================================

---
id_oferta: 040
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
id_oferta: 041
anunciante: "Simbora Concursos"
url_destino: "https://www.facebook.com/simboraconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=3157233831074462"
dias_ativo: 924
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt6, trt7, trt11, trt20, trt24"
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
id_oferta: 042
anunciante: "Escola Trabalhista"
url_destino: "https://escolatrabalhista.com.br/preparacao-extensiva-analista-judiciario-do-trt-area-judiciaria/"
ad_library_url: "https://www.facebook.com/ads/library/?id=971307882122417"
dias_ativo: 185
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 1.725,00"
fonte_ticket: "checkout"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "vídeo (1)"
botoes: "Saiba mais (1)"
precos_exibidos_na_lp: "R$ 2.397,00 | R$ 1.725,00 | R$ 178,40"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps:
  - nome: "CURSO COMPLETO DE DIREITO DO TRABALHO 2026 -"
    valor: "R$ 367,00"
  - nome: "CLUBE DE QUESTÕES 2.0 - 12 MESES DE"
    valor: "R$ 897,00"
---
### Copy do Anúncio (Gancho de Entrada)
"Conheça o método da Escola Trabalhista que vai te dar condições REAIS de ser aprovado como Analista Judiciário do TRT em 24 semanas de estudos, com qualidade e direcionamento! 🔥 Garanta sua vaga na Preparação Extensiva Analista TRT!"

### Landing Page: Headline & Promessa Central
"PREPARAÇÃO EXTENSIVA ANALISTA JUDICIÁRIO DO TRT - ÁREA JUDICIÁRIA — Junte-se a mais de 12.000 alunos"

### Seções da Landing Page (títulos, na ordem)
- Qualquer pessoa pode ser aprovada
- A Escola Trabalhista te oferece tudo isso
- O que dizem os alunos
- Mais depoimentos da nossa metodologia
- Um plano comprovadamente eficiente
- Vamos te colocar dentro dos 5% dos candidatos que realmente concorrem às vagas
- Três são os elementos
- que irão te deixar à frente dos concorrentes, potencializando sua chances de aprovação
- Metodologia Exclusiva
- Atualização Constante
- O que você vai receber
- Metas diárias e cronograma de estudos
- Quatro simulados completos
- Questões objetivas comentadas
- Central de dúvidas exclusiva
- E-books aprofundados
- Ciclos de revisão
- ⁠Caderno de jurisprudência
- Acesso garantido
- Caderno de jurisprudência destacada
- Mapas mentais, supercards e tabelas incorporadas ao material didático
- Dicas rápidas de Direito do Trabalho em vídeoaulas
- Atualização Constante do Material
- Mini módulo de discursiva
- Mini módulo de redação
- Professores dos módulos de videoaulas
- Já são centenas de aprovados
- Quais disciplinas você irá dominar
- Faça sua matrícula
- PREPARAÇÃO EXTENSIVA ANALISTA JUDICIÁRIO DO TRT – ÁREA JUDICIÁRIA

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Discursiva / redação
- Mapas mentais
- PDF
- Simulados
- Videoaulas


========================================

---
id_oferta: 043
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2292-concurso-trt-nacional-club-analista-judiciario-area-judiciaria"
ad_library_url: "https://www.facebook.com/ads/library/?id=1568529141941465"
dias_ativo: 162
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Curso em videoaulas, Material em PDF / apostila / caderno, Questões / simulados"
formatos_dos_anuncios: "imagem (1)"
botoes: "Saiba mais (1)"
precos_exibidos_na_lp: "R$ 16 | R$ 10 | R$ 3.710,00 | R$ 2.411,50 | 12x de R$ 200,96"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Lançados em abril de 2026
O ano de 2026 está muito promissor nas oportunidades de concursos para Tribunais de Justiça.
E você pode se preparar para todos os certames com o curso TRT Nacional Club.
Estude com mentorias ao vivo, simulados, aulas de revisão, caderno de metas e muito mais! 🚀
Dê o próximo passo rumo a uma melhor qualidade de vida pessoal e profissional.
Matricule-se agora no TRT Nacional Club! 👇
Equipe de Especialistas
Ceisc"

### Landing Page: Headline & Promessa Central
"TRT Nacional Club | Analista Judiciário - Área Judiciária — TRT-8 EDITAL PUBLICADO"

### Seções da Landing Page (títulos, na ordem)
- TRT-8 EDITAL PUBLICADO
- Sobre o curso
- Nesse curso você terá
- Conheça os professores
- Assista ao panorama de concursos de TRTs
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
id_oferta: 044
anunciante: "Concurseiro aos 40"
url_destino: "https://www.facebook.com/61564214427286/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1330662368927610"
dias_ativo: 160
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
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
"Lançados em maio de 2026
🛑 Você ainda tá esperando o edital sair pra começar?
Esses TRTs seguem com validade ativa — Mas quem só começar depois… já vai chegar atrasado. ⏳
O pré-edital é o momento mais estratégico da preparação.
É agora que se constrói o resultado que aparece lá na frente.
📚💡
👉 Quer se organizar com eficiência pra aproveitar essas oportunidades?
Comenta TRT aqui ⬇️ que eu vou te ajudar com um direcionamento personalizado.
#concursos #concursospublicos #concurseiro #estudaqueavidamuda #provas #trt"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 045
anunciante: "Pódio Procuradorias"
url_destino: "https://cronosconcursos.com.br/livro-fichamento/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1023341813683635"
dias_ativo: 127
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "vídeo (1)"
botoes: "Ver detalhes (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Lançados em junho de 2026
⚖️Fichar é pensar o Direito com estratégia
📍No Direito Material e Processual do Trabalho, o fichamento não é apenas um resumo, é uma forma inteligente de compreender, conectar e aplicar os institutos jurídicos no dia a dia, seja na prática profissional ou na preparação para provas.
📖 “O estudo sistematizado transforma a leitura em compreensão e a compreensão em aplicação segura do Direito.”
🎯 Quem organiza o estudo, ganha clareza.
⚖️ Quem ganha clareza, atua com mais segurança jurídica.
✍️ Autores:
Hector Cavalcanti Chamberlain — Procurador do Estado de Alagoas. Mestre em Processo Civil pela UFES.
Ana Karenina Cavalcanti Chamberlain — Oficial de Justiça do TRT da 2ª Região. Especialista em Direito Material e Processual do Trabalho.
👉 Clique em "Saiba mais" e garanta seu exemplar"

### Landing Page: Headline & Promessa Central
"Fichamento de Direito Material e Processual do Trabalho — O guia definitivo para concurseiros: organização completa da legislação trabalhista, súmulas e jurisprudência selecionada: tudo em um único recurso."

### Seções da Landing Page (títulos, na ordem)
- Fichamento de Direito Material e Processual do Trabalho
- Seu guia completo para dominar o Direito do Trabalho
- Legislação Organizada
- Jurisprudência Selecionada
- Tudo em Um Lugar
- Por que escolher este livro?
- Escrito por Professores da Cronos
- Hector Cavalcanti Chamberlain
- Ana Karenina Cavalcanti Chamberlain
- O que dizem os concurseiros
- Conteúdo Completo do Livro
- Direito Material do Trabalho
- Direito Processual do Trabalho
- Dúvidas sobre o livro ?
- Ainda tem dúvidas?
- Garanta seu exemplar agora

### Seção "Para Quem É" (declarado na LP)
- •Princípios e fontes do direito do trabalho
- •Relação de trabalho e relação de emprego
- •Contrato individual de trabalho
- •Alteração, suspensão e interrupção do contrato
- •Rescisão do contrato de trabalho
- •Jornada de trabalho e períodos de descanso

### Entregáveis / Formato (termos encontrados na LP)
- Mentoria
- Resumos


========================================

---
id_oferta: 046
anunciante: "nomaderachel com Focus Concursos Públicos"
url_destino: "https://focusconcursos.com.br/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1937040066929154"
dias_ativo: 83
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt 8"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "vídeo (1)"
botoes: "Ver detalhes (1)"
precos_exibidos_na_lp: "R$ 1.773,33 | 12x de R$ 39,90 | R$ 478,80 | R$ 2.217,78 | 12x de R$ 42,90 | R$ 514,80 | R$ 3.995,56 | 12x de R$ 89,90"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"@focusconcursos #cupomnomaderachel #nomaderachel #alegria #feliz #concursospúblicos"

### Títulos do link nos anúncios
- nomaderachel

### Landing Page: Headline & Promessa Central
"Procurando um curso específico? — Veja o que estão falando sobre nós"

### Seções da Landing Page (títulos, na ordem)
- Assinatura Focus Acesso de 1 ano
- Assinatura Focus Acesso de 2 anos
- Assinatura Focus Acesso Vitalício
- Depoimento de nossos alunos
- Últimas notícias
- Concursos Maranhão: FCC é confirmada e governo anuncia mais de 3.500 vagas
- TRT 8: edital é publicado com salários de até R$ 16 mil
- Concurso PC PE: edital oferece 1.315 vagas; salários chegam a R$ 13,5 mil
- Concurso de Aparecida de Goiânia oferece 2.956 vagas na área da educação
- Concursos PM e Bombeiros PE: editais somam 1.890 vagas
- Concurso ALEPA: editais abrem 135 vagas para níveis médio e superior
- Edital da UFBA abre 139 vagas com salários que chegam a R$ 5,2 mil
- Concurso SEDF 2026: banca entra em definição para 10.604 vagas
- Concurso Prefeitura de Curitiba: três editais trazem mais de 340 vagas
- Concurso GCM São Gonçalo: 101 vagas e até R$ 4,5 mil de salário
- Concurso TCE GO: inscrições começam em outubro; salário de R$ 11,8 mil
- Concurso DPE SP: abertura do certame segue em análise

### Entregáveis / Formato (termos encontrados na LP)
- Discursiva / redação


========================================

---
id_oferta: 047
anunciante: "Concursosmeucurso"
url_destino: "https://meucurso.com.br/cursos/concursos-publicos"
ad_library_url: "https://www.facebook.com/ads/library/?id=1542521100851019"
dias_ativo: 78
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "carrossel (1)"
botoes: "Saiba mais (1)"
precos_exibidos_na_lp: "R$ 350 | R$ 1.899,00 | 12x de R$ 94,92 | R$ 1.139,00 | R$ 899,00 | 12x de R$ 33,25 | R$ 399,00 | R$ 799,00"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
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
- Procuradorias FCC | Resolução de Questões - online
- Procuradoria do Estado de São Paulo | Peças Práticas
- Regular Procuradorias Estaduais e Municipais
- Procuradorias Municipais e Estaduais | Peças Práticas
- Procuradorias | Assinatura
- 6º ENAM 2026.2 - Online - início 08/09
- ENAM | Assinatura

### Entregáveis / Formato (termos encontrados na LP)
- PDF
- Simulados


========================================

---
id_oferta: 048
anunciante: "BZP Bancários"
url_destino: "http://fb.me/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2249586425882185"
dias_ativo: 51
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tst"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "imagem (1)"
botoes: "Saiba mais (1)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Passar no PSI e mudar de cidade é uma das coisas mais comuns na carreira de um bancário. E uma das menos discutidas.
Você se inscreveu. Foi aprovado. Recebeu uma ajuda para a mudança, arrumou a vida em outro estado e seguiu.
E é aí que a maioria encerra o assunto.
Mas ajuda de custo de mudança e adicional de transferência são coisas juridicamente diferentes. Já houve caso em que a Caixa tentou abater um auxílio pago na mudança do valor do adicional e o Tribunal não admitiu, entre outros motivos porque não ficou demonstrado que as duas verbas têm a mesma natureza e a mesma finalidade.
Uma é despesa. A outra está no artigo 469 da CLT, tem natureza salarial e repercute em outras verbas do contrato.
Esse tema vem sendo analisado em decisões recentes de diferentes regiões do país, inclusive em segunda instância - todas sujeitas a recurso.
Três pontos que costumam surpreender quem nunca olhou para isso:
A inscrição no processo seletivo interno não descaracteriza, por si só, o interesse da empresa em movimentar o empregado.
Exercer cargo comissionado não afasta o direito. O TST já firmou esse entendimento.
E a prova de que a transferência foi definitiva cabe à empresa, que detém os registros - não ao trabalhador.
O que define tudo isso não é o nome dado ao ato de remoção. É o que aconteceu na prática: quanto tempo você ficou, se houve mudança de cidade, se você voltou depois.
Se você mudou de cidade a trabalho e depois retornou, vale a análise. Seu histórico funcional conta essa história melhor do que a memória.
Cada caso é analisado individualmente.
#bancarios #empregadocaixa #adicionaldetransferencia #direitodotrabalho #bzpbancarios"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 049
anunciante: "Nomade Rachel com Focus Concursos Públicos"
url_destino: "https://focusconcursos.com.br:443/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1071730625255558"
dias_ativo: 48
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt 8"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "vídeo (1)"
botoes: "Saiba mais (1)"
precos_exibidos_na_lp: "R$ 1.773,33 | 12x de R$ 39,90 | R$ 478,80 | R$ 2.217,78 | 12x de R$ 42,90 | R$ 514,80 | R$ 3.995,56 | 12x de R$ 89,90"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"www.focusconcursos.com.br @focusconcursos cupom:nomaderachel descontos, bora estudar, passar no concurso, trabalhar, aposentar bem e curtir a melhor fase da vida: A aposentadoria♥️#nomaderachel #focusconcursos #concursopúblico ##cursopreparatorioparaconcursos"

### Títulos do link nos anúncios
- Nomade Rachel

### Landing Page: Headline & Promessa Central
"Procurando um curso específico? — Veja o que estão falando sobre nós"

### Seções da Landing Page (títulos, na ordem)
- Assinatura Focus Acesso de 1 ano
- Assinatura Focus Acesso de 2 anos
- Assinatura Focus Acesso Vitalício
- Depoimento de nossos alunos
- Últimas notícias
- Concursos Maranhão: FCC é confirmada e governo anuncia mais de 3.500 vagas
- TRT 8: edital é publicado com salários de até R$ 16 mil
- Concurso PC PE: edital oferece 1.315 vagas; salários chegam a R$ 13,5 mil
- Concurso de Aparecida de Goiânia oferece 2.956 vagas na área da educação
- Concursos PM e Bombeiros PE: editais somam 1.890 vagas
- Concurso ALEPA: editais abrem 135 vagas para níveis médio e superior
- Edital da UFBA abre 139 vagas com salários que chegam a R$ 5,2 mil
- Concurso SEDF 2026: banca entra em definição para 10.604 vagas
- Concurso Prefeitura de Curitiba: três editais trazem mais de 340 vagas
- Concurso GCM São Gonçalo: 101 vagas e até R$ 4,5 mil de salário
- Concurso TCE GO: inscrições começam em outubro; salário de R$ 11,8 mil
- Concurso DPE SP: abertura do certame segue em análise

### Entregáveis / Formato (termos encontrados na LP)
- Discursiva / redação


========================================

---
id_oferta: 050
anunciante: "MEQ Concursos"
url_destino: "https://meqconcursos.com.br/amostra-pre-edital/"
ad_library_url: "https://www.facebook.com/ads/library/?id=938466562639552"
dias_ativo: 43
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Cronograma / plano de estudos, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "carrossel (1)"
botoes: "Saiba mais (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Testar a Amostra do Pré-Edital TRT's não é só "dar uma olhada".
Você entra e recebe 7 dias de acesso às duas primeiras semanas do cronograma oficial, com PDMEQ, VadeMEQ e MEQ Cards, a mesma estrutura de quem já é aluno matriculado.
Cronograma pronto, material organizado, e você sentindo na prática se o método funciona pra você antes de decidir qualquer coisa.
Testa grátis por 7 dias, sem custo e sem compromisso.
Toque em saiba mais e confira!"

### Landing Page: Headline & Promessa Central
"Comece a estudar de graça com o pré‑edital TRTs 2026 — Preencha seus dados e destrave 7 dias de acesso gratuito ao curso, sem precisar cadastrar cartão de crédito."

### Seções da Landing Page (títulos, na ordem)
- Por 7 dias, você terá acesso a conteúdos específicos para TRTs , através de:
- MEQCards
- Cronogramas
- Link de questões
- Quem estuda com o MEQ, percebe a diferença

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma


========================================

---
id_oferta: 051
anunciante: "Gustavo Nogueira - Aprovação Ágil"
url_destino: "https://lp.aprovacaoagil.com.br/vsl-white-trt-noticia"
ad_library_url: "https://www.facebook.com/ads/library/?id=1058146883624666"
dias_ativo: 43
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tst"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno, Lei seca / legislação"
formatos_dos_anuncios: "vídeo (1)"
botoes: "Saiba mais (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Qual o melhor concurso de tribunal pra você começar hoje?
TRT. Técnico entra em R$11.500 iniciais, jornada de 35 horas por semana, teletrabalho na maioria dos tribunais. Contando os 24 TRTs mais o TST, são 25 chances na mesma matéria.
Só que essa fila não se atravessa com 500 horas de videoaula e apostilão de 15 mil páginas. A prova é objetiva — o jogo é acertar a questão.
A ordem que resolve: questão comentada, gabarito destrinchado, lei seca e súmula do TST.
Clica no botão que eu te mostro como acertar mais questão em menos tempo, de graça."

### Títulos do link nos anúncios
- Melhor tribunal pra começar hoje

### Landing Page: Headline & Promessa Central
"Título"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 052
anunciante: "Editora Instituto CDT"
url_destino: "https://editora.institutocdt.com.br/produto/libido-masculina-da-fisiologia-a-prescricao"
ad_library_url: "https://www.facebook.com/ads/library/?id=1345385987351355"
dias_ativo: 38
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (1)"
botoes: "Ver detalhes (1)"
precos_exibidos_na_lp: "R$ 409,00 | R$ 257,67"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Todo médico que atende homens adultos conhece as armadilhas do consultório: pedir só testosterona total e perder o diagnóstico, confundir libido com ereção, não reconhecer a síndrome MOSH no paciente obeso, subestimar o efeito de ISRS, betabloqueadores, opioides e espironolactona sobre o desejo sexual, ou ficar sem rumo diante do usuário de anabolizantes em "blast and cruise". Some-se a isso a insegurança com fitoterápicos, a dose errada de anastrozol que provoca hipoestrogenismo iatrogênico e o monitoramento frouxo da TRT — e o resultado é o paciente migrando para coaches de academia e protocolos de internet.
"Libido masculina — da fisiologia à prescrição" foi escrito para resolver essas dores. Em 14 capítulos divididos em cinco partes — Fundamentos, Etiologia, Tratamento Não Hormonal, Tratamento Hormonal e Populações Especiais — o livro entrega fluxogramas diagnósticos, painéis laboratoriais mínimos, fórmulas fitoterápicas combinadas com doses fechadas, protocolos detalhados de TRT (cipionato, Durateston, Nebido, gel e pellets) com cronograma de monitoramento, e protocolos completos de terapia pós-ciclo com clomifeno e hCG. Cada capítulo traz casos clínicos, regras de ouro, pegadinhas e alertas que transformam conhecimento em decisão imediata.
Destinado a médicos, é a referência prática para quem entendeu que a queixa sexual masculina não é detalhe — é frequentemente o primeiro sinal de doenças metabólicas, psiquiátricas e cardiovasculares que merecem método. Da fisiologia à prescrição. Da queixa à conduta."

### Títulos do link nos anúncios
- Libido masculina: da fisiologia à prescrição 👉

### Landing Page: Headline & Promessa Central
"Libido masculina: da fisiologia à prescrição — Todo médico que atende homens adultos conhece as armadilhas do consultório: pedir só testosterona total e perder o diagnóstico, confundir libido com ereção…"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 053
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://lp.cadernodoaprovado.com/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1607407254411907"
dias_ativo: 30
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno, Questões / simulados, Discursiva / redação, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (1)"
botoes: "Ver detalhes (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Estude com com o 1º lugar no TRT-22 🏆
São mais de 10.000 concurseiros estudando com o Caderno do Aprovado 📚
✅ Materiais de estudos para TRT:
• Meus cadernos das principais matérias
• Cronograma flexível
• Metas de estudos
• Planilha de controle
• Links para videoaulas
• Links para questões
• Revisões programadas
• Atualizações pós-edital
• Manual de redação
• Estratégia de reta final
• Jurisprudência organizada
✅ Meu direcionamento em TODAS as matérias
✅ Diversos BÔNUS
✅ SUPORTE no Whatsapp
✅ ATUALIZAÇÕES no pós-edital
Clique em SAIBA MAIS e prepare-se em alto nível para os próximos concursos!
clique em SAIBA MAIS e comece agora mesmo! ✅️"

### Títulos do link nos anúncios
- Caderno Do aprovado

### Landing Page: Headline & Promessa Central
"Caderno Do aprovado"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 054
anunciante: "Pratique Concursos"
url_destino: "https://ti.pratiqueconcursos.com.br/fcti/main.html"
ad_library_url: "https://www.facebook.com/ads/library/?id=2307143873373354"
dias_ativo: 28
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tribunal regional do trabalho"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Mapas mentais / esquemas, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "carrossel (1)"
botoes: "Saiba mais (1)"
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

### Títulos do link nos anúncios
- Super Resumos para Concurso TRT

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
id_oferta: 055
anunciante: "Nação Jurídica com GGS Advogados Associados"
url_destino: "https://guimasilvadvogados.com.br/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1295807189831029"
dias_ativo: 17
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, justica do trabalho"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "imagem (1)"
botoes: "Enviar mensagem pelo WhatsApp (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Trabalhar no setor administrativo de um hospital não coloca ninguém a salvo dos riscos biológicos. E a Justiça do Trabalho acaba de reconhecer isso.
Em atuação conduzida pelos advogados Dr. Paulo Vinicius Guimarães e Dr. Marcos Raimundo da Silva, do escritório Guimarães e Silva (@guima_e_silva - https://guimasilvadvogados.com.br/), a Justiça do Trabalho de Ribeirão Preto (TRT da 15ª Região) condenou um hospital a pagar adicional de insalubridade de 20% a uma trabalhadora administrativa. A perícia confirmou que o direito depende da exposição ao ambiente de risco, independentemente do cargo.
⚖️ O que o hospital foi condenado a pagar:
✅ Adicional de insalubridade de 20% por todo o contrato
✅ Reflexos em férias + 1/3, 13º salários, aviso prévio indenizado e FGTS + multa de 40%
✅ R$ 4.000,00 de honorários periciais
✅ Indenização de 20% equivalente aos honorários advocatícios, valor que vai integralmente para a trabalhadora
✅ Honorários sucumbenciais de 15% aos advogados da parte
O direito nasce do ambiente e da exposição ao risco, não do cargo na carteira. Quem atua na recepção, faturamento, arquivo ou portaria de unidades de saúde sem a proteção adequada pode estar perdendo 20% do salário todos os meses, sendo essencial contar com análise técnica especializada.
#DireitoDoTrabalho #Insalubridade #DireitosTrabalhistas #Hospital #JustiçaDoTrabalho AgentesBiológicos Advocacia
WHATSAPP
api.whatsapp.com"

### Landing Page: Headline & Promessa Central
"Defesa firme dos seus direitos — com a experiência de quem já atuou em mais de 25 mil processos . — Mais de 8 anos defendendo pessoas e empresas com seriedade, técnica e proximidade. Atuação sólida em Direito Bancário, Previdenciário, Trabalhista, Cível e de Família."

### Seções da Landing Page (títulos, na ordem)
- Áreas de atuação
- Bancário & Consumidor
- Previdenciário
- Trabalhista
- Consultoria Jurídica
- De Franca para todo o interior paulista
- Decisões recentes
- Revisão de empréstimo consignado CLT
- Proteção do mínimo existencial de aposentado
- Nulidade de cláusula de compartilhamento de dados
- Adicionais por tempo de serviço a servidor
- Ao seu lado, do primeiro atendimento à decisão final.
- Sócios, Parceiros & Equipe
- Marcos Raimundo da Silva
- Paulo Vinicius Guimarães
- João Marcelo de Avelar Neto
- Darielis Magalhães Cordeiro
- Jéssica Paula Barbosa Silva
- Vamos conversar sobre o seu caso

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 056
anunciante: "Verbo Carreiras Jurídicas"
url_destino: "https://api.whatsapp.com/send"
ad_library_url: "https://www.facebook.com/ads/library/?id=1098210225904481"
dias_ativo: 15
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Curso em videoaulas, Lei seca / legislação"
formatos_dos_anuncios: "vídeo (1)"
botoes: "Ver detalhes (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Captura de Lead (WhatsApp / Grupo VIP)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Conheça o curso que vai te aprovar no TRT-4 por menos de 5,00 ao dia!
São 50 encontros, mentorias com especialistas e Vade Mecum incluso na modalidade presencial e muito mais!
Para passar, tem que ser Verbo!"

### Títulos do link nos anúncios
- Curso preparatório para o concurso do TRT-4 por menos de R$5,00 ao dia!

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 057
anunciante: "Markup Inc."
url_destino: "http://fb.me/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1327471585972272"
dias_ativo: 14
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "imagem (1)"
botoes: "Cadastre-se (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"um novo padrão de alto padrão para os negócios na Praia da Avenida, Maceió.
Salas comerciais flexíveis de 41m² a 111m², em um empreendimento beira-mar exclusivo, com vista mar em 80% das unidades e esquadrias do piso ao teto.
✅ Boulevard comercial com vista mar
✅ Rooftop exclusivo com restaurante panorâmico e heliponto
✅ Auditório/Espaço Multiuso com vista panorâmica
✅ Espaço Zen para o seu bem-estar
✅ Arquitetura com fachada verde e design contemporâneo
✅ 2 a 4 vagas de garagem
✅ 9 andares | 270 unidades
✅ Obra a preço de custo
✅ A 8 min da Ponta Verde e 10 min da Barra Nova
Localização estratégica, próxima ao novo centro administrativo, hospitais, TRT, Fórum e cartórios.
Desenvolvido pela Markup Incorporações.
📲 Quer saber mais? Fale com a nossa equipe e garanta sua sala no endereço mais sofisticado de Maceió!
Clique e receba mais informações"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 058
anunciante: "Malditafcc"
url_destino: "https://www.facebook.com/malditafcc/"
ad_library_url: "https://www.facebook.com/ads/library/?id=4717861935137850"
dias_ativo: 9
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt3, trt4, trt8, trt18"
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
"Os TRTs estão se mexendo e tem muita gente que só vai perceber quando o edital sair.
Arrasta pro lado que eu te conto o que aconteceu essa semana em quatro tribunais diferentes.
E fica o recado: quem começa agora chega no edital com vantagem. Não é sobre estudar mais, é sobre estudar o que realmente cai.
💬 Comenta TRT que eu te mando o link do Protocolo no direct.
📌 Salva pra não perder e manda pra quem também sonha com tribunal.
#concursotrt #trt #trtrs #trt4 #trt8 #trtmg #trt3 #trtgo #trt18 #concursopublico #concursos #concurseiro #concurseira #tecnicojudiciario #analistajudiciario #tribunais #concursostribunais #fcc #estudarparaconcurso #vidadeconcurseiro #aprovacao #servidorpublico #ploa2027"

### Títulos do link nos anúncios
- Mateus Alves (@malditafcc) • Instagram photos and videos

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 059
anunciante: "Escola Até a Aprovação Policiais"
url_destino: "https://www.facebook.com/eaapoliciais/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1837036453960474"
dias_ativo: 8
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
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

---
id_oferta: 060
anunciante: "Vinco Leilões"
url_destino: "https://www.facebook.com/61575191932532/"
ad_library_url: "https://www.facebook.com/ads/library/?id=4069762199991599"
dias_ativo: 8
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt2"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "carrossel (1)"
botoes: "Enviar mensagem pelo WhatsApp (1)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🎣 Pesqueiro em São Roque com lance mínimo de R$ 6,6 milhões
Uma oportunidade no 708º Leilão Judicial Unificado do TRT2, em São João Novo, São Roque/SP.
O imóvel abriga atualmente um pesqueiro para atividades recreativas e conta com uma ampla estrutura:
🌳 Área de aproximadamente 12,42 alqueires paulistas
🏗️ 1.896,93 m² de área construída em benfeitorias
🎣 Lago e quiosques com churrasqueiras
🏊 Piscina
🎉 Salões de festas
🏡 Chalé e casa de administração
⚽ Campo de futebol e playground
🍽️ Espaço para restaurante/lanchonete
💰 Avaliação: R$ 13.200.000
🔨 Lance mínimo: R$ 6.600.000
➡️ Lance mínimo correspondente a 50% do valor de avaliação.
📲 Fale com a equipe da Vinco pelo WhatsApp para saber mais e consulte no site a descrição completa, o edital e as condições da arrematação."

### Títulos do link nos anúncios
- Pesqueiro em São Roque | Lance mínimo R$ 6,6 mi

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 061
anunciante: "Benito Soluções Judiciais"
url_destino: "https://www.facebook.com/benitosolucoesjudiciais/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1639791717871051"
dias_ativo: 8
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "imagem (1)"
botoes: "Enviar mensagem pelo WhatsApp (1)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚛 VENDA JUDICIAL – SEMIRREBOQUES SR/RANDON SR CA
⚪ Lote composto por: 2 semirreboques SR/Randon SR CA, 24 pneus e 1 estepe.
💰 Lance inicial: R$ 93.000,00
📌 Com possibilidade de parcelamento!
📌 Aceita venda separada dos veículos!
Descrição: Lote composto por dois semirreboques SR/Randon SR CA, acompanhados de 24 pneus e 1 estepe, disponibilizados em venda judicial. Os bens podem ser adquiridos em conjunto ou separadamente, proporcionando maior flexibilidade ao comprador. Trata-se de uma excelente oportunidade para aquisição de equipamentos robustos, reconhecidos pela resistência, durabilidade e excelente custo-benefício, com possibilidade de compra abaixo do valor de mercado.
Destaques do equipamento:
Venda em lote ou separadamente
Conjunto composto por 2 semirreboques, 24 pneus e 1 estepe
Modelo reconhecido pela resistência estrutural
Excelente opção para ampliar ou renovar a frota
Indicado para transporte rodoviário de cargas diversas
Baixo custo de manutenção e ampla disponibilidade de peças
📌 Ótima oportunidade para transportadoras, frotistas e motoristas autônomos que desejam investir com segurança e economia.
📞 Mais informações e acesso ao edital completo:
WhatsApp: (19) 99919-2010
👨‍💼 Corretor Judicial habilitado junto ao TRT-15 – CRECI/SP nº 78.903-F"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 062
anunciante: "vamos.falardireito"
url_destino: "http://preceder.com.br/inscreva/"
ad_library_url: "https://www.facebook.com/ads/library/?id=871645662605057"
dias_ativo: 8
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt15"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados"
formatos_dos_anuncios: "carrossel (1)"
botoes: "Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Carreiras Jurídicas / OAB"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Saúde e segurança no trabalho: dos riscos psicossociais à higiene ocupacional.
O Comitê Regional do Trabalho Seguro do TRT da 15ª Região reúne a Magistratura do Trabalho, o Ministério Público do Trabalho, a Advocacia, a Toledo Prudente e a Unoeste. Serão dois painéis e uma conferência de encerramento sobre a identificação dos riscos no ambiente laboral, a responsabilidade e a reparação dos danos e as questões atuais das normas de higiene ocupacional.
🗓 27 de outubro de 2026, terça-feira, das 13h às 18h
📍 OAB de Presidente Prudente
📝 Inscrições: preceder.com.br/inscreva
🎓 Com certificado
🤝 Leve 1 kg de alimento (doação voluntária)
Arraste para o lado e veja a programação completa.
#TrabalhoSeguro #TRT15 #SaúdeESegurançaNoTrabalho #RiscosPsicossociais #PresidentePrudente"

### Landing Page: Headline & Promessa Central
"Faça sua inscrição — Preencha os dados para fazer sua inscrição."

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 063
anunciante: "Professor Raphael Reis"
url_destino: "https://www.professorraphaelreis.com.br/curso/curso-de-redacao-trt-8-tecnico/"
ad_library_url: "https://www.facebook.com/ads/library/?id=4394209337506519"
dias_ativo: 8
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt 8"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 450,00"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Discursiva / redação"
formatos_dos_anuncios: "carrossel (1)"
botoes: "sem botão (1)"
precos_exibidos_na_lp: "12x de R$ 49,32 | R$ 450,00"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps:
  - nome: "Agente de I.A: Bruxinho da Redação Tenha o"
    valor: "R$ 21,90"
  - nome: "Mapas Mentais para usar na Redação Revise com"
    valor: "R$ 61,00"
---
### Copy do Anúncio (Gancho de Entrada)
"Aprenda com quem é referência nacional em redação para concursos e transforme a discursiva em um dos seus maiores diferenciais."

### Títulos do link nos anúncios
- Redação TRT-8

### Landing Page: Headline & Promessa Central
"Curso de Redação TRT-8 — O que dizem nossos alunos"

### Seções da Landing Page (títulos, na ordem)
- 12x de R$49,32
- +20 MÓDULOS DE CONTEÚDO
- 4 CORREÇÕES PERSONALIZADAS
- ACESSO ATÉ O DIA DA PROVA
- O que dizem nossos alunos
- Assista à aula de apresentação do curso
- Carga horária
- Acesso por celular
- Garantia
- Baixe os PDFs
- Assista outra vez
- Suporte por whatsapp
- Tudo isso por apenas
- 12x R$49,32 Ou R$450,00 à vista

### Entregáveis / Formato (termos encontrados na LP)
- Discursiva / redação
- PDF
- Videoaulas


========================================

---
id_oferta: 064
anunciante: "Professor Raphael Reis"
url_destino: "https://www.professorraphaelreis.com.br/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1264220292516021"
dias_ativo: 8
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt8"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Discursiva / redação"
formatos_dos_anuncios: "vídeo (1)"
botoes: "sem botão (1)"
precos_exibidos_na_lp: "R$ 450,00 | R$ 390,00"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"A nossa aluna @eduardarsena deu show no TJCE: tirou 10 na redação de técnico e 9.35 na redação de analista!
Maria Eduarda, parabéns pelos resultados e pela aprovação 👏🧙‍♂️
Rumo à posse 🚀
www.magodaredacao.com.br
#tjce #concursotjce #concursospúblicos #aprovação #magodaredação"

### Landing Page: Headline & Promessa Central
"Home - Mago da Redação — Cursos em destaque"

### Seções da Landing Page (títulos, na ordem)
- Cursos em destaque
- Curso de Redação TRT-4
- Curso de Redação TRT-8
- Estudo de Caso TRT8 (AJAJ e AJOJ)
- Cursos de Redação
- Mentorias e Correções
- e-Books Premium
- E ainda tem muito material gratuito!
- Newsletter
- Exclusivos
- Sobre o Professor Raphael Reis
- Assista os últimos vídeos do Youtube:
- Depoimentos
- Últimas do blog
- A Revolução dos Bichos, de George Orwell
- Tudo sobre a redação e o estudo de caso do TRT-8
- Curso de Redação PC-PE (banca Cebraspe) passo a passo

### Entregáveis / Formato (termos encontrados na LP)
- Discursiva / redação
- Mentoria


========================================

# Parte 2 — Ofertas adjacentes (66)

Apareceram nas buscas, mas não citam os termos do foco. Servem para comparar formatos e preços de outros nichos de concurso; algumas não são de concurso.

---
id_oferta: 065
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
id_oferta: 066
anunciante: "Central de Concursos"
url_destino: "https://centraldeconcursos.com.br/concursos/concurso-tj-sp-escrevente"
ad_library_url: "https://www.facebook.com/ads/library/?id=4419979344943402"
dias_ativo: 86
anuncios_coletados: 3
anuncios_ativos_estimados: 8
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "vídeo (3)"
botoes: "sem botão (3)"
precos_exibidos_na_lp: "R$ 8.872,54"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
id_oferta: 067
anunciante: "Decorando a Lei Seca Cursos Para Concursos E OAB"
url_destino: "https://www.facebook.com/decorandoaleisecaconcursoseoab/"
ad_library_url: "https://www.facebook.com/ads/library/?id=792696320220760"
dias_ativo: 186
anuncios_coletados: 6
anuncios_ativos_estimados: 6
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Questões / simulados, Lei seca / legislação, Discursiva / redação"
formatos_dos_anuncios: "carrossel (3), imagem (3)"
botoes: "Visitar perfil do Instagram (3), sem botão (3)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
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
- O art. 30 do Código Penal é daqueles dispositivos curtos, mas que a banca adora explorar em prova objetiva.
- ⚠️ Uma palavra pode mudar completamente o gabarito da questão.
- O Código Penal usa a mesma técnica de redação em dois artigos diferentes, e as bancas cobram a diferença exatamente do mesmo jeito.
- O art. 6º da Lei 14.133/2021 é, hoje, um dos dispositivos mais cobrados em concursos públicos. Só em provas da FGV e do CEBRASPE, já apareceu mais de 40 vezes.
- O art. 319 do Código Penal caiu no concurso para Promotor do MP-GO!

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 068
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
id_oferta: 069
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
id_oferta: 070
anunciante: "Clube do Perito"
url_destino: "https://lp.vagasjustica.com.br/wpj/diario/fisioterapeuta/c?utm_source=meta_%7B%7Bsite_source_name%7D%7D&utm_medium=cpc_%7B%7Bplacement%7D%7D&utm_campaign=%7B%7Bcampaign.id%7D%7D_%7B%7Bcampaign.name%7D%7D&utm_content=%7B%7Badset.id%7D%7D_%7B%7Badset.name%7D%7D&utm_term=%7B%7Bad.id%7D%7D_%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1404455104491303"
dias_ativo: 15
anuncios_coletados: 1
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (1)"
botoes: "sem botão (1)"
precos_exibidos_na_lp: "R$ 6.350,10"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 PROCURA-SE FISIOTERAPEUTAS🚨
👉 Se você deseja trabalhar para a Justiça sem prestar concurso público, ter renda extra de casa e atuar com laudos dentro da sua área de formação,
essa é a sua grande oportunidade!
✅ Participe do AULÃO ON-LINE e GRATUITO, HOJE, às 20h, e descubra como ingressar nessa área e conquistar sua independência profissional.
Clique em "SAIBA MAIS" e garanta sua vaga!"

### Landing Page: Headline & Promessa Central
"VAGA PARA FISIOTERAPEUTA : ATUE COMO PERITO TEMPORÁRIO SEM PRESTAR CONCURSO E RECEBA UMA RENDA EXTRA MÉDIA DE R$6.350,10 A CADA 30 DIAS. — Reunião AO VIVO, GRATUITA E ON-LINE"

### Seções da Landing Page (títulos, na ordem)
- Informe seu nome e telefone para concluir a inscrição

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 071
anunciante: "Eccos Cursos"
url_destino: "https://eccosedu.com/laser-transdermico/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2426372244512830"
dias_ativo: 76
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "imagem (1), carrossel (2)"
botoes: "Saiba mais (3)"
precos_exibidos_na_lp: "R$ 9.900,00 | R$ 22.852,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Área da Saúde"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"A escleroterapia facial tem risco documentado de migração intracraniana e, na prática, um risco ainda maior: embolia arterial, numa região com incontáveis artérias pequenas.
O Laser Nd:YAG 1064nm tem risco zero de migração e de embolia. Por quê? Ação local. Nada é injetado, nada pode migrar.
Não é comparação teórica. É o que a anatomia facial impõe a qualquer cirurgião que opera nessa região sem critério de seleção claro.
O sistema valvular da face existe, mas não protege contra a migração do agente esclerosante para o sistema intracraniano.
Em veia periorbital, o volume recomendado não passa de 0,2ml por injeção. E mesmo dentro desse limite, o maior risco não é o volume: é acertar uma artéria no meio do caminho.
Foi assim que um caso documentado de espuma de polidocanol em veia supratroclear terminou em perda total de visão, por injeção arterial inadvertida.
O Curso de LASER Transdérmico da ECCOS foi desenvolvido para o cirurgião vascular que quer dominar a ferramenta mais segura disponível para tratar lesões vasculares faciais, com parametrização precisa, protocolo anatômico e prática supervisionada.
Vagas limitadas. Módulo presencial em São Paulo.
Garanta sua vaga no curso mais completo de LASER Transdérmico do Brasil e transforme sua prática clínica.
HTTPS://ECCOSEDU.COM/LASER-TRANSDERMICO/
Veja Detalhes"

### Ganchos das variações (1ª linha de cada anúncio)
- A escleroterapia facial tem risco documentado de migração intracraniana e, na prática, um risco ainda maior: embolia arterial, numa região com incontáveis artérias pequenas.
- Comprimento de onda correto. Duração de pulso dentro do TRT. Fluência calibrada para o alvo.
- Vasos abaixo do calibre 30G: o laser não é uma alternativa à escleroterapia. É a indicação correta.

### Landing Page: Headline & Promessa Central
"OUTROS CURSOS DISPONÍVEIS — Amplie sua formação com outros cursos da ECCOS Edu. Oferecemos outros cursos especializados para complementar sua formação."

### Seções da Landing Page (títulos, na ordem)
- Hands-on Laser Transdérmico
- Amplie seus horizontes no tratamento de vasos
- Próxima turma presencial dias 5 a 6 de março 2027 Prime Care - Rua Traipú, 509 - Perdizes, São Paulo
- Seja um Médico de Excelência
- Se você deseja ser reconhecido no mercado pelos tratamentos tecnológicos de ponta, você precisa:
- Dominar as técnicas avançadas:
- Aprenda as bases teóricas de interação luz-tecido e ajuste os parâmetros do laser para diferentes lesões vasculares.
- Expandir seu horizonte de tratamentos:
- Integre novas técnicas em sua prática clínica e ofereça tratamentos mais eficazes e inovadores.
- Aumentar a satisfação dos pacientes:
- Melhore os resultados dos tratamentos e ofereça uma experiência superior aos seus pacientes.
- Agregar valor aos seus procedimentos:
- Diferencie-se da concorrência com técnicas avançadas, aumentando a fidelização dos pacientes e o faturamento da sua clínica.
- Para quem é destinado
- Cirurgiões vasculares
- Especialistas em tratamentos de varizes dos membros inferiores
- Médicos que desejam se atualizar e dominar técnicas avançadas de laser
- Programação
- O curso é cuidadosamente estruturado para fornecer a você todo o conhecimento necessário:
- Bases teóricas do laser
- Como adequar parâmetros ao aparelho disponível
- Como escolher as lesões vasculares para tratamento com laser
- O uso do laser justifica-se como técnica e resultado? Ou somente como ferramenta de marketing?
- Como prever o resultado do tratamento vascular com laser transdérmico.
- Atingindo o limite da técnica.
- Complicações do laser transdérmico 1064nm Nd para tratamento de vasos
- Complicações das terapias a laser e LIP
- Controle de dor durante os procedimentos cutâneos
- Uso do Laser Transdérmico
- Qual técnica e quando associar ao tratamento de vasos com laser?

### Entregáveis / Formato (termos encontrados na LP)
- Mentoria


========================================

---
id_oferta: 072
anunciante: "Caderno Mapeado"
url_destino: "https://cadernomapeado.com.br/tce-ma-cmlm/?src=&utm_source=facebook-ads&utm_medium=%7B%7Badset.name%7D%7D&utm_content=%7B%7Bad.name%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D&utm_term=%7B%7Bplacement%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=4297463713898141"
dias_ativo: 58
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
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
id_oferta: 073
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
id_oferta: 074
anunciante: "Milena Correia Advocacia"
url_destino: "https://api.whatsapp.com/send"
ad_library_url: "https://www.facebook.com/ads/library/?id=1625294329172426"
dias_ativo: 23
anuncios_coletados: 2
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "vídeo (2)"
botoes: "Saiba mais (1), sem botão (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Captura de Lead (WhatsApp / Grupo VIP)"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Irregularidades em concursos públicos podem arruinar seus sonhos!
Você sabia que muitos candidatos são prejudicados por erros em concursos públicos?
Editais mal feitos, decisões injustas e bancas que ferem a igualdade entre candidatos podem destruir anos de esforço.
Eu sou Milena Correia, advogada especializada, e já ajudei várias pessoas a reverterem essas situações e garantirem seus direitos.
📲 Clique em Saiba Mais e veja como posso te ajudar!"

### Títulos do link nos anúncios
- Clique em "SAIBA MAIS"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 075
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
id_oferta: 076
anunciante: "Gustavo Nogueira - Aprovação Ágil"
url_destino: "https://pages.aprovacaoagil.com.br/vsl/tjsp/v01"
ad_library_url: "https://www.facebook.com/ads/library/?id=1577788783367784"
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
tipos_produto: "Questões / simulados, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (1)"
botoes: "sem botão (1)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 1
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
id_oferta: 077
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2067-concurso-tj-sp-club-oficial-de-justica?utm_source=meta_ads&utm_medium=cpc&utm_campaign=vendas_tj_sp_oficial_de_justica"
ad_library_url: "https://www.facebook.com/ads/library/?id=2800223780310745"
dias_ativo: 191
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (1), vídeo (1)"
botoes: "Saiba mais (2)"
precos_exibidos_na_lp: "R$ 9 | R$ 7.312,44 | R$ 10 | R$ 1.799,00 | 12x de R$ 149,92 | R$ 1.619,10 | R$ 4.390,00 | 12x de R$ 365,83"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"A sua preparação para o TJ-SP exige foco e direcionamento.
Por isso, preparamos um material exclusivo para você focado em Língua Portuguesa: Interpretação de Texto no TJ-SP: O Estilo da Banca Vunesp.
Produzido por especialistas e 100% gratuito, o e-book traz o perfil da prova e conteúdos direcionados para ajudar você a avançar rumo à nomeação como Oficial de Justiça.
👉 Inscreva-se e baixe agora mesmo!
Material Exclusivo
Aprove com Ceisc"

### Ganchos das variações (1ª linha de cada anúncio)
- Mais um concurso para Oficial de Justiça do TJ-SP deve chegar em breve!
- A sua preparação para o TJ-SP exige foco e direcionamento.

### Landing Page: Headline & Promessa Central
"TJ-SP Club | Oficial de Justiça — Sobre o curso"

### Seções da Landing Page (títulos, na ordem)
- Sobre o curso
- Nesse curso você terá
- Conheça os professores
- Sobre a prova
- Conteúdo Programático
- Perguntas frequentes
- Confira as últimas notícias do nosso blog

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Mentoria
- Planner
- Simulados
- Videoaulas


========================================

---
id_oferta: 078
anunciante: "Pódio Tribunais"
url_destino: "https://api.whatsapp.com/send"
ad_library_url: "https://www.facebook.com/ads/library/?id=966341029113449"
dias_ativo: 171
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Cronograma / plano de estudos"
formatos_dos_anuncios: "vídeo (2)"
botoes: "Saiba mais (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Captura de Lead (WhatsApp / Grupo VIP)"
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
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 079
anunciante: "Felipe Sgarbossa Advocacia Criminal"
url_destino: "https://www.facebook.com/felipesgarbossa/"
ad_library_url: "https://www.facebook.com/ads/library/?id=881739941593479"
dias_ativo: 166
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "vídeo (2)"
botoes: "Saiba mais (1), sem botão (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Carreiras Policiais"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🗣️ Sustentação oral em Revisão Criminal envolvendo a correta delimitação das imputações e a aplicação do conceito de crime único no tráfico de drogas.
A condenação havia sido estruturada em concurso material entre dois fatos de tráfico, resultando em pena de 15 anos, 07 meses e 15 dias de reclusão.
♟️A partir da leitura técnica dos autos, a defesa demonstrou um ponto central: as condutas imputadas não eram autônomas.
As apreensões ocorreram no mesmo dia, como desdobramento de uma única operação policial, envolvendo os mesmos agentes e os mesmos verbos nucleares do tipo (“guardar” e “ter em depósito”), inseridas em um mesmo contexto fático-probatório.
✔️Ausente a pluralidade de ações, não há espaço para o concurso material.
✔️ O correto enquadramento jurídico impõe o reconhecimento de crime único, com a unificação das condutas.
⚖️ O Tribunal acolheu a tese defensiva e fixou diretriz relevante: Múltiplas apreensões, quando decorrentes de uma mesma investigação e inseridas em unidade de contexto, não autorizam a fragmentação da imputação penal.
O resultado foi uma redução da pena para 09 anos, 04 meses e 15 dias de reclusão, com extensão dos efeitos ao corréu.
📌 A Sustentação Oral foi determinante para a consolidação dessa compreensão perante o colegiado, especialmente por se tratar de Revisão Criminal, onde os requisitos para análise do pedido são específicos e limitados às hipóteses do art. 621 do Código de Processo Penal.
.
.
.
#AdvocaciaCriminal #RevisãoCriminal #SustentaçãoOral #AtuaçãoemTribunais #TribunaisSuperiores"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

## Demais adjacentes (resumo)

| id | Anunciante | Dias | Anúncios | Tração | Ticket (checkout) | Destino |
|---|---|---|---|---|---|---|
| 080 | Prof.carlosgoncalves | 121 | 2 | médio | Não confirmado | https://typebot.co/plataformaanalistadetribunais |
| 081 | IPOG Salvador | 112 | 2 | médio | Não confirmado | https://ipog.edu.br/cursos/pos-graduacao/psicologia-juridica-com-enfase-em-peric |
| 082 | Tjteiros | 97 | 2 | médio | Não confirmado | https://www.facebook.com/61582438800580/ |
| 083 | Estratégia Concursos | 84 | 2 | médio | Não confirmado | https://www.facebook.com/EstrategiaConcursos/ |
| 084 | Ludy Sena | 83 | 2 | médio | Não confirmado | https://www.facebook.com/ludysena.perita/ |
| 085 | LH no pódio | 77 | 2 | médio | Não confirmado | https://typebot.co/mentoria-zeroaopodio |
| 086 | Venâncio & Delgado - Advogados | 58 | 2 | médio | Não confirmado | https://api.whatsapp.com/send |
| 087 | Venâncio & Delgado - Advogados | 58 | 2 | médio | Não confirmado | https://www.facebook.com/venancioedelgadoadvogados/ |
| 088 | Academia do Perito | 22 | 2 | médio | R$ 497,00 | https://lp.academiadoperito.com/peju-dor?utm_source=facebook&utm_medium=paid&utm |
| 089 | Estudo e Memorização | 17 | 2 | médio | Não confirmado | https://estudomemorizacao.com.br/pv-video-v2/ |
| 090 | Mapas da Lulu Concurseira com Laura Amorim | 10 | 2 | médio | R$ 597,90 | https://paginas.mapasdalulu.com.br/lp-pacote/ |
| 091 | Prof. Ronaldo Santos | 8 | 2 | médio | Não confirmado | https://rslinguaportuguesa.com/aplicacao-fgv/?utm_source=facebook&utm_medium=cpc |
| 092 | Projeto Caveira | 325 | 1 | médio | Não confirmado | https://www.facebook.com/projetocaveiraprf/ |
| 093 | Pódio Tribunais | 198 | 1 | médio | Não confirmado | https://cronosconcursos.com.br/tribunais/?utm_source=meta&utm_medium=ig-ads&utm_ |
| 094 | Concursos Ceisc | 191 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2070-concurso-tj-ba-analista-judiciario-area-judicia |
| 095 | Ceisc Concursos | 178 | 1 | médio | Não confirmado | https://lp.ceisc.com.br/evento-concursos-nivel-medio/ |
| 096 | Gaby no Tribunal | 175 | 1 | médio | Não confirmado | https://www.facebook.com/100090566482087/ |
| 097 | Discursiva na Prática | 126 | 1 | médio | R$ 1.489,00 | https://discursivanapratica.com.br/assinaturacontrole/?utm_source=facebook&utm_m |
| 098 | Douglas Prado - Servidor 30k | 103 | 1 | médio | Não confirmado | https://odouglasprado.com.br/plano-servidor-30k/ |
| 099 | Rafael Amaral Adv | 94 | 1 | médio | Não confirmado | https://www.facebook.com/cleytonrafaelamaral/ |
| 100 | Fauth e Freitas Sociedade de Advogados com Adriane Fauth | 92 | 1 | médio | Não confirmado | https://www.facebook.com/61573224123970/ |
| 101 | mamae_concurseira6 com Decorando a Lei Seca Cursos Para Concursos E OAB | 85 | 1 | médio | Não confirmado | https://www.decorandoaleiseca.com.br/ |
| 102 | Atleta dos Concursos | 83 | 1 | médio | Não confirmado | https://atletadosconcursos.com.br/kit-aprovacao-enam/?sck=facebook%7Cads%7Cconve |
| 103 | Brabo Editora | 83 | 1 | médio | R$ 397,00 | https://braboeditora.com.br/mestre-em-questoes-tjsp-v8/ |
| 104 | Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24 | 78 | 1 | médio | Não confirmado | https://ataticadaaprovacao.com.br/ |
| 105 | Mege | 66 | 1 | médio | Não confirmado | https://concurcity.mege.com.br/explorar |
| 106 | NEAF Concursos Públicos com tjserei | 64 | 1 | médio | Não confirmado | https://www.neafconcursos.com.br/produtos/escrevente-tjsp-2026-demonstrativo-tes |
| 107 | Themas Cartórios | 64 | 1 | médio | Não confirmado | http://www.themas.com.br/ |
| 108 | cristinedentista | 59 | 1 | médio | Não confirmado | https://www.facebook.com/cristinedentista/ |
| 109 | Concurseiro Fora da Caixa | 57 | 1 | médio | Não confirmado | https://concurseiroforadacaixa.com.br/collections/todos-os-materiais |
| 110 | Professora Amanda Aires | 54 | 1 | médio | Não confirmado | https://www.amandaaires.com.br/curso/%5B2026%5D-economia-para-o-tcu/345 |
| 111 | Rô Santtana - OAB | 51 | 1 | médio | Não confirmado | https://rosanttana.com.br/captacao/lp-discursiva-oab.html |
| 112 | Rhema Lab com Rodrigo Noronha | 50 | 1 | médio | Não confirmado | https://rhemalab.com.br/ |
| 113 | Concursos Ceisc | 50 | 1 | médio | Não confirmado | https://www.sympla.com.br/produtor/ceisc |
| 114 | emanuellasouza.adv | 49 | 1 | médio | Não confirmado | https://www.instagram.com/_u/emanuellasouza.adv |
| 115 | Prof. Herbert Almeida | 23 | 1 | médio | Não confirmado | https://herbertalmeida.com.br/mentoria-cgu/ |
| 116 | Memorização Bruno Campos Concursos | 21 | 1 | médio | Não confirmado | https://www.facebook.com/100088833677510/ |
| 117 | Clube do Perito | 14 | 1 | médio | Não confirmado | https://lp.vagasjustica.com.br/wpj/diario/psicologo/c?utm_source=meta_%7B%7Bsite |
| 118 | Aprovação Perfeita | 14 | 1 | médio | Não confirmado | https://aprovacaoperfeita.com.br/oferta-GOLD-VSL/ |
| 119 | Marco Cursos Preparatórios | 13 | 1 | médio | Não confirmado | https://www.facebook.com/marcocursos/ |
| 120 | danielvieira_2 | 13 | 1 | médio | Não confirmado | https://hotmart.com/pt-br/marketplace/produtos/hagsxd-o-jogo-da-aprovacao-z99mi/ |
| 121 | Pedro Auar Advocacia | 9 | 1 | médio | Não confirmado | https://www.facebook.com/pedroauar/ |
| 122 | Paulo Afonso Advocacia | 9 | 1 | fraco | Não confirmado | https://www.facebook.com/61582851535500/ |
| 123 | Gtcar | 9 | 1 | médio | Não confirmado | https://www.facebook.com/61556284626069/ |
| 124 | Professora Fernanda Barboza | 8 | 1 | médio | Não confirmado | https://hml.fernandabarboza.com.br/2026/09/16/dt-black-friday-antecipada-vsl/ |
| 125 | GG Concursos | 8 | 1 | médio | Não confirmado | https://ggconcursos.com.br/cursos/gg-play/gg-play-vitalicio-360 |
| 126 | Unipds | 8 | 1 | médio | Não confirmado | https://unipds.com.br/unipds-ia-funil/#hero |
| 127 | Migalhas | 8 | 1 | médio | Não confirmado | https://eventos.migalhas.com.br/evento/738/namoro-qualificado-e-uniao-estavel-ca |
| 128 | Tese Concursos | 8 | 1 | médio | Não confirmado | https://www.facebook.com/TESECONCURSOS/ |
| 129 | Curso Ênfase | 8 | 1 | médio | Não confirmado | https://www.facebook.com/cursoenfase/ |
| 130 | Sensei da Aprovação - Concursos Públicos | 8 | 1 | médio | Não confirmado | https://senseidaaprovacao.com.br/projetosenseicuritiba |

# Apêndice — Descartadas por não citarem concurso (128)

Vieram nas buscas (ex.: escritórios que citam o TRF como tribunal), mas o texto não tem nenhum termo de concurso. Confira se algo relevante caiu aqui por engano.

| Anunciante | Dias | Destino |
|---|---|---|
| Ato psicologia psicoterapias psicodrama e desenvolvimento humano | 142 | https://api.whatsapp.com/send |
| SERV FONE | 99 | https://www.facebook.com/servfone.servfone/ |
| KELLY VIANA | 99 | https://www.facebook.com/61558444803544/ |
| Reviva | 29 | https://renuva.com.br/pages/drenagem-linfatica |
| Godri Domingues Advocacia | 57 | https://www.facebook.com/godridomingues/ |
| Rita Bervig | 178 | https://www.facebook.com/100091834883862/ |
| Fernanda Diniz | 29 | https://renuva.com.br/pages/drenagem-linfatica |
| Danielle Bartoly | 170 | https://www.facebook.com/61577922862090/ |
| Aqui Tem Plano de Saúde | 63 | http://fb.me/ |
| Visão Química do Brasil | 57 | http://fb.me/ |
| Sementes Biomatrix | 56 | https://www.youtube.com/watch?v=CWapR4E8Kdo |
| Precatorial | 54 | http://fb.me/ |
| Dr. Paulo Leandro - Cirurgião Ortopedista | 13 | https://www.facebook.com/61590189522867/ |
| Dra. Gabriela Madeira | 10 | https://api.whatsapp.com/send |
| ShopRootvana | 10 | https://tryrootvana.com/pages/listicle-2 |
| Alibaba.com | 149 | https://www.alibaba.com/product-detail/haoge_10000022881599.html?src=cpm_fb&sub_ |
| Dr Bruno Guerra | 126 | https://www.facebook.com/61566645860434/ |
| Hematix - Hematite Bracelet | 125 | https://myhematix.com/products/hematix-strength-band |
| Clinica Osmilto Brandão | 72 | https://www.facebook.com/100093106637344/ |
| Flat & Hotel Executive | 65 | https://www.facebook.com/61584218885791/ |
| Prática e Pós CEISC | 64 | https://ceisc.com.br/categorias/pos-graduacao |
| ShopVantique | 58 | https://shopvantique.com/products/vantique-nad-supplement-for-men |
| Andrew Martin - Health & Performance Advisor | 57 | https://assess.secondprime.io/ |
| TSTemdia | 55 | https://lp.tstemdia.com.br/ |
| Heraclio Cunha | 51 | https://peritoem7dias.com.br/ |
| Bience Agriscience | 50 | https://www.facebook.com/bience.ag/ |
| JB Advocacia | 48 | https://janainabaptista.adv.br/ |
| Lucas Krausche - Desenrolado | 46 | https://cdr.lkrausche.com/ |
| ShopRootvana | 25 | https://tryrootvana.com/products/rootvana-l-carnitine-4000mg-liquid-spanish?utm_ |
| Central Sul de Leilões | 18 | https://www.centralsuldeleiloes.com.br/ |
| Verbo Carreiras Jurídicas | 15 | https://chat.whatsapp.com/Bsvp30MtbOTI4HDJuoMz89?mode=hqrt2 |
| Carlos Klein - Personal | 13 | https://oficialbarrigazero.protocolocarlos.com.br/quizz |
| Doctora Karito | 10 | https://trt.colorpack.online/ |
| Iridium Labs | 10 | https://www.iridiumlabs.com.br/products/zeus-extreme-pre-hormonal-60-comps |
| SECOM com Luciano do Secom | 9 | https://www.facebook.com/sousecom/ |
| Renuva | 8 | https://renuva.com.br/pages/drenagem-linfatica |
| Juri Digital | 156 | https://www.facebook.com/juridigitalcombr/ |
| CAEPE - Centro Avançado de Estudos Periciais com Erotilde Minharro | 152 | https://caepe.com.br/ |
| Editora Mizuno | 141 | https://www.editoramizuno.com.br/ |
| Bruto Brasil | 128 | https://www.youtube.com/watch?v=S9fODqC2kkw&feature=youtu.be |
| Douglas Prado - Servidor 30k com Servidores High Level | 124 | https://www.facebook.com/professorlucrativo/ |
| Dental Speed | 118 | https://www.dentalspeed.com/pasta-de-prova-relyx-try-in-3m-solventum-5351.html |
| Perville Construtora | 113 | https://www.facebook.com/PervilleConstrutora/ |
| LeClinic Odontologia | 112 | https://www.facebook.com/leclinicodontologia/ |
| Jerônimo E-Lance | 110 | https://www.facebook.com/jeronimodosleiloes/ |
| TSTemdia | 109 | https://www.facebook.com/61581193663516/ |
| Advocacia Miqueias Oliveira | 105 | https://www.facebook.com/61585245201416/ |
| 42pericias | 102 | https://www.42pericias.com.br/ |
| Duarte Advogados Associados | 101 | https://www.facebook.com/61555624388490/ |
| JQM Advocacia Especializada | 100 | https://www.facebook.com/61561436444397/ |
| Mitsubishi Motors Brasil | 97 | https://www.mitsubishimotors.com.br/picapes/nova-triton?utm_source=facebook&utm_ |
| EBM Goiás | 96 | http://fb.me/ |
| Fibra Pará | 94 | https://www.facebook.com/fibrapara/ |
| Dr. Kegel: For Men’s Health & Wellness | 93 | https://quiz.kegel-plan.me/pt-br/?cmpid=67b757a235e0d329de693d90&sub1=%7B%7Bad.i |
| pilateshiitflow com Riven Fitness for Life | 91 | https://www.instagram.com/_u/pilateshiitflow |
| Carreira de Perito | 88 | https://carreiradeperito.com.br/ |
| OAB Subseção Atibaia | 86 | https://api.whatsapp.com/send |
| Instituto Médico da Dor - IMD | 85 | https://www.facebook.com/61550152706355/ |
| IBCCRIM | 83 | https://jcc.ibccrim.org.br/ |
| Madervillas Madeireira . Lauro de Freitas | 76 | https://www.facebook.com/61577737911934/ |
| Start Electric - Instalação e Manutenção Elétrica | 73 | https://www.facebook.com/startelectric31/ |
| VCA Construtora e Incorporadora | 72 | http://fb.me/ |
| Instituto Doutrina Policial 2 | 71 | http://fb.me/ |
| Gestaodeclinica | 71 | https://minhaclinicamilionaria.com.br/?utm_source=facebook&utm_medium=cpc&utm_ca |
| Dr. Jordan Seabra de Oliveira - Advogado Trabalhista | 66 | https://www.facebook.com/61590618007101/ |
| UNDB Imperatriz | 66 | http://fb.me/ |
| Prompt8 AI | 66 | https://jusquant.ai/?utm_source=meta&utm_medium=paid_social&utm_campaign=trab_up |
| CSR Marketing e Mídias | 65 | http://fb.me/ |
| Diego Filipe Tulio com Grand Mercure Pinheiros | 65 | https://www.facebook.com/100083362727382/ |
| Servita Clinic | 65 | https://www.facebook.com/61582841670718/ |
| Gil Fernandes | 64 | https://www.facebook.com/gilfernandes01/ |
| Luiz Guedes | 64 | https://www.facebook.com/100068780851308/ |
| prof.eduardowaga | 62 | https://www.facebook.com/prof.eduardowaga/ |
| DramaBox - short drama2 | 60 | https://play.google.com/store/apps/details?id=com.storymatrix.drama |
| DramaBox - short drama1 | 60 | https://play.google.com/store/apps/details?id=com.storymatrix.drama |
| Amaro Alfaya Advogados | 59 | https://www.facebook.com/61591636236469/ |
| Juanita Restaurante | 59 | https://www.facebook.com/juanitarestaurante/ |
| Fernandez Pollito Advocacia | 58 | https://www.facebook.com/advocaciapollito/ |
| RAIR Silva | 57 | https://www.facebook.com/jornalistarairsilva/ |
| Viégas Filho | 57 | https://www.facebook.com/100094050184913/ |
| Judit | 56 | https://produto.judit.io/miner-precatorios |
| Aurora by Lidiane Kuhn | 56 | https://www.facebook.com/61590179524480/ |
| Oral Supreme | 55 | https://www.facebook.com/www.clinicaoralsupreme.com.br/ |
| Sicredi Sementes do Sul | 55 | https://www.linkedin.com/uas/login?session_redirect=https%3A%2F%2Fwww.linkedin.c |
| thainara.assistentesocial | 55 | https://www.instagram.com/_u/thainara.assistentesocial |
| BLL Compras com Licitações Municipais. | 52 | https://www.facebook.com/BLLCOMPRAS/ |
| Gabriela Franco | 52 | https://www.facebook.com/61575028750782/ |
| AnotherVoid | 52 | https://anothervoid.co/products/liquid-l-carnitine-4000mg?variant=49141411283179 |
| Bruno Pesca & Turismo Corumbá | 51 | https://brunopescaturismo.com.br/ |
| Benvindoadv Professor com Benvindoadv Previdenciário | 51 | https://www.facebook.com/100095299025661/ |
| Inovajur Capacitação Jurídica e IA | 51 | https://inovajur.com/nova-pratica-vsl/?utm_source=Facebook_ads&utm_medium=%7B%7B |
| Avante | 51 | https://www.facebook.com/61572155530930/ |
| MB Comunidade | 50 | https://comunidademb.com/lista-de-espera/ |
| Go Kursos | 50 | https://www.gokursos.com/go-oab---direito-penal---2%C2%AA-fase-30553/p |
| amandamoreno.sette | 49 | https://www.instagram.com/_u/amandamoreno.sette |
| Faloppa Advogados Associados | 48 | https://api.whatsapp.com/send |
| Grau Técnico Parnamirim | 48 | https://www.facebook.com/grautecnicoparnamirim/ |
| Dr. Paulo Cruz | 48 | https://www.facebook.com/61588916093349/ |
| Emily Verde | 47 | https://www.facebook.com/100092688495300/ |
| Velyon Energia Solar | 31 | https://api.whatsapp.com/send |
| Keylon Lucarelli - Nutrologia e Emagrecimento Saudável | 27 | https://www.facebook.com/100082746462251/ |
| ShopRootvana | 25 | https://tryrootvana.com/pages/listicle-1 |
| Muniz Auto Center Vitória da Conquista | 22 | https://www.facebook.com/munizvitoriadaconquista/ |
| Cellics Health | 21 | https://cellics.co/pages/appledroppers-2 |
| Experience True Nutra | 17 | https://truenutra.com/products/fb-en-us-mc001 |
| Eletricista a preço popular | 17 | https://wa.me/message/VUCK56R4WH35K1 |
| Alfa Viking | 16 | https://alfaviking.com.br/libi/ |
| Hospital Adventista de Belém | 16 | https://www.facebook.com/hospitalbelem/ |
| Start Veículos - Suzano/Sp | 15 | https://www.startveiculo.com.br/ |
| Morais Amaral Arquitetura | 15 | https://www.moraisamaral.arq.br/ |
| Vanguarda Visual Law | 14 | https://vanguardavisuallaw.com.br/kit-advocacia-trabalhista |
| Hormofy | 14 | https://hormofy.com/reposicao-hormonal/ |
| Benvindoadv Professor | 13 | https://www.facebook.com/100095299025661/ |
| Vinco Leilões | 13 | https://www.vinconews.com.br/Leiloes/2026/TRT2-SP |
| Rafael Amaral Adv | 12 | https://api.whatsapp.com/send |
| naylinnunes | 12 | https://www.instagram.com/_u/naylinnunes |
| True Nutra Plus | 12 | https://truenutra.com/products/fb-en-lc001 |
| Leandro Magalhães | 12 | https://www.facebook.com/AnalyticsBR/ |
| Vinícius Rocha | 10 | https://www.facebook.com/ViniciusRocha.casas.terrenos.chacaras.fazendas/ |
| Congresso TEA RP com gialbuquerquesp | 10 | https://payfast.greenn.com.br/sdq5zr4 |
| Previdas Saúde | 9 | https://provamedica3.previdas.com.br/?src=&utm_source=meta&utm_medium=%7B%7Badse |
| Aerocar Veículos | 9 | https://www.facebook.com/aerocarveiculos/ |
| Mundo das Capas Guaratinguetá | 9 | https://www.facebook.com/mundodascapasguara/ |
| Clinicaespacoter Connected Page | 9 | https://api.whatsapp.com/send |
| Gabriella Ibrahim | 8 | https://www.facebook.com/gabriellathomasibrahim/ |
| UroLages - Urologia Especializada | 8 | https://www.facebook.com/UroLages/ |
| Doseprimal Brasil | 8 | https://doseprimal.com/pages/doseprimalt |
| Nacional Utilidades | 8 | https://www.facebook.com/NacionalUtilidades/ |
