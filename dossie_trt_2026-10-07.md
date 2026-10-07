# Dossiê ConcursoRadar — Técnico Judiciário — TRT (07/10/2026)

## Métricas da Rodada
- **Buscas na Meta Ad Library:** `concurso TRT`, `tribunal regional do trabalho`, `justiça do trabalho concurso`, `técnico judiciário`, `TRT técnico judiciário`, `TRT2`, `TRT15`, `TRT1`, `TRT4`, `TRT3`, `concurso tribunal`
- **Filtro:** anúncios ativos no Brasil, no ar há 7+ dias (coleta ampla para achar padrões; a longevidade é analisada nas tabelas)
- **Ofertas do nicho:** 132 (de 347 anúncios; agrupadas por anunciante + página de destino)
- **Descartadas por não citarem concurso:** 75 (listadas no fim para auditoria)
- **Ofertas de foco direto:** 60 | adjacentes: 72
- **Sinal de tração:** 10 forte, 2 fraco, 120 médio
- **Landing pages lidas:** 83 de 132
- **Ticket confirmado no checkout:** 15 de 19 ofertas com checkout detectado (79%)
- **Tempo de processamento:** 798 segundos

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

Base: **347 anúncios de 96 anunciantes**; 128 estão no ar há 45+ dias (veteranos); mediana de 26 dias.

Como ler: **Anunciantes** = quantos produtores distintos usam (popularidade). **Veteranos** = quantos desses anúncios estão no ar há 45+ dias, e **% dos veteranos** = a fatia da categoria entre todos os veteranos. Se a fatia entre veteranos é maior que a fatia geral (% anúncios), a categoria aparece mais entre os que duram. Categoria com 1 ou 2 anunciantes é só um caso isolado.

A coleta junta duas amostras por busca (anúncios com 7+ dias e anúncios com 45+ dias), então a proporção de veteranos no total não é uma taxa de sobrevivência.

## Formato do criativo

Vídeo, imagem única ou carrossel.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| vídeo | 57 | 59% | 147 | 42% | 50 | 78 | 61% |
| imagem | 38 | 40% | 153 | 44% | 10 | 29 | 23% |
| carrossel | 24 | 25% | 47 | 14% | 29 | 21 | 16% |

## Proporção do criativo

Vertical (4:5 ou 9:16), quadrada (1:1) ou horizontal.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| vídeo vertical | 54 | 56% | 137 | 39% | 48 | 70 | 55% |
| imagem vertical | 31 | 32% | 137 | 39% | 10 | 21 | 16% |
| carrossel vertical | 17 | 18% | 36 | 10% | 35 | 17 | 13% |
| imagem quadrada | 9 | 9% | 14 | 4% | 48 | 8 | 6% |
| carrossel quadrada | 8 | 8% | 10 | 3% | 25 | 4 | 3% |
| vídeo quadrada | 3 | 3% | 4 | 1% | 67 | 3 | 2% |
| vídeo horizontal | 2 | 2% | 6 | 2% | 705 | 5 | 4% |
| imagem horizontal | 2 | 2% | 2 | 1% | 23 | 0 | 0% |
| carrossel horizontal | 1 | 1% | 1 | 0% | 8 | 0 | 0% |

## Duração dos vídeos

Só anúncios em vídeo.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| 31s a 1min | 29 | 51% | 61 | 41% | 51 | 35 | 45% |
| 1 a 2min | 25 | 44% | 49 | 33% | 29 | 21 | 27% |
| Mais de 2min | 13 | 23% | 21 | 14% | 91 | 14 | 18% |
| Até 30s | 8 | 14% | 16 | 11% | 53 | 8 | 10% |

## Botão (CTA)

Rótulo do botão exibido no anúncio.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| sem botão | 42 | 44% | 108 | 31% | 29 | 42 | 33% |
| Saiba mais | 38 | 40% | 146 | 42% | 21 | 44 | 34% |
| Ver detalhes | 17 | 18% | 39 | 11% | 48 | 23 | 18% |
| Enviar mensagem pelo WhatsApp | 11 | 11% | 18 | 5% | 10 | 0 | 0% |
| Visitar perfil do Instagram | 10 | 10% | 19 | 5% | 174 | 12 | 9% |
| Comprar agora | 6 | 6% | 12 | 3% | 30 | 6 | 5% |
| Enviar mensagem | 3 | 3% | 3 | 1% | 12 | 0 | 0% |
| Cadastre-se | 1 | 1% | 1 | 0% | 13 | 0 | 0% |
| Inscreva-se | 1 | 1% | 1 | 0% | 86 | 1 | 1% |

## Destino do clique

Para onde o anúncio leva.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Página própria (LP / site) | 66 | 69% | 257 | 74% | 24 | 87 | 68% |
| Página / formulário no Facebook | 33 | 34% | 81 | 23% | 29 | 36 | 28% |
| WhatsApp | 5 | 5% | 7 | 2% | 57 | 4 | 3% |
| Perfil do Instagram | 1 | 1% | 1 | 0% | 22 | 0 | 0% |
| Checkout direto | 1 | 1% | 1 | 0% | 49 | 1 | 1% |

## Tamanho da copy

Texto principal do anúncio.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Média (200 a 600) | 56 | 58% | 175 | 50% | 29 | 78 | 61% |
| Longa (mais de 600) | 42 | 44% | 113 | 33% | 22 | 44 | 34% |
| Curta (até 200 caracteres) | 13 | 14% | 58 | 17% | 10 | 6 | 5% |
| Sem texto | 1 | 1% | 1 | 0% | 12 | 0 | 0% |

## Tipo de gancho (1ª linha da copy)

Classificação por palavras-chave; um gancho pode cair em mais de um tipo.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos | Exemplo |
|---|---|---|---|---|---|---|---|---|
| Outro | 51 | 53% | 144 | 41% | 29 | 49 | 38% | 🚨 PROCURA-SE PEDAGOGOS🚨 — Caminho da Perícia |
| Notícia de concurso / edital | 23 | 24% | 65 | 19% | 10 | 21 | 16% | Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova? — MEQ Concursos |
| Pergunta | 19 | 20% | 38 | 11% | 59 | 26 | 20% | Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova? — MEQ Concursos |
| Número / lista | 14 | 15% | 44 | 13% | 10 | 10 | 8% | 3 cenários de APROVAÇÃO ✅️ — Caderno do Aprovado - Materiais para Concursos |
| Dor / erro do candidato | 13 | 14% | 26 | 7% | 17 | 11 | 9% | Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova? — MEQ Concursos |
| Prova social / autoridade | 12 | 12% | 22 | 6% | 57 | 13 | 10% | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? — Isaque Concursos |
| Oferta / desconto / urgência | 11 | 11% | 24 | 7% | 35 | 11 | 9% | "📚🆓 Curso Grátis TJ-SP 2026 - Escrevente Técnico Judiciário! 🆓📚 — Nova Concursos |
| Chamada direta ao público | 11 | 11% | 21 | 6% | 50 | 13 | 10% | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. — Tjteiros |
| Salário / estabilidade | 10 | 10% | 29 | 8% | 10 | 6 | 5% | ⚖️ Os próximos concursos de TRTs podem abrir excelentes oportunidades em diferentes regiões do país, com remunerações iniciais que podem chegar a cerca de R$ 16 — Concurseiro aos 40 |
| Promessa de método | 10 | 10% | 22 | 6% | 57 | 17 | 13% | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? — Isaque Concursos |
| Contraintuitivo / inimigo comum | 5 | 5% | 8 | 2% | 16 | 2 | 2% | Não é falta de dedicação. É falta de direção. — Supremo Concursos |

## Elementos da copy

Recursos presentes no texto; não são excludentes.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Usa emojis | 60 | 62% | 193 | 56% | 29 | 83 | 65% |
| Lista com marcadores (✔, ✅, •) | 23 | 24% | 83 | 24% | 29 | 34 | 27% |
| Hashtags | 22 | 23% | 44 | 13% | 38 | 22 | 17% |
| Cita valor em R$ | 21 | 22% | 60 | 17% | 10 | 9 | 7% |
| Link ou 'link na bio' no texto | 11 | 11% | 18 | 5% | 56 | 12 | 9% |
| Gancho em CAIXA ALTA | 10 | 10% | 35 | 10% | 29 | 1 | 1% |
| Cita bônus | 4 | 4% | 11 | 3% | 51 | 6 | 5% |
| Cita garantia | 4 | 4% | 4 | 1% | 53 | 2 | 2% |

## Sinais de público (ICP) citados na copy

Quem o anúncio diz atender, por palavras-chave. Indica a quem o mercado fala, não quem compra.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos | Exemplo |
|---|---|---|---|---|---|---|---|---|
| Motivado por salário / estabilidade | 27 | 28% | 72 | 21% | 11 | 17 | 13% | Se você quer chegar competitivo para ser aprovado e nomeado nas próximas provas de TRTs, a Imersão Aprova TRT pode ser um divisor de águas para conquistar a tão — Isaque Concursos |
| Esquece o que estuda / revisão | 24 | 25% | 54 | 16% | 21 | 17 | 13% | 📚 Quem quer disputar uma vaga de verdade precisa construir base, revisar com método, acompanhar o próprio desempenho e estudar com direção. — Concurseiro aos 40 |
| Trabalha / tem pouco tempo | 17 | 18% | 107 | 31% | 12 | 24 | 19% | Durante essa jornada de estudos, eu estudava de 2h a 3h por dia, já que estudava e trabalhava como CLT. — Isaque Concursos |
| Pré-edital / sair na frente | 12 | 12% | 25 | 7% | 29 | 11 | 9% | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. — Tjteiros |
| Dificuldade em discursiva / redação | 9 | 9% | 22 | 6% | 12 | 5 | 4% | Não para estudar mais um pouco. Para sentar, encarar 60 questões seguidas, matérias misturadas, discursiva e o relógio correndo. — MEQ Concursos |
| Estuda há tempo e não passa | 8 | 8% | 17 | 5% | 56 | 12 | 9% | Você estuda, se prepara, domina o conteúdo… mas ainda trava na hora da redação? 📝 — Professor Hansk |
| Começando do zero | 7 | 7% | 23 | 7% | 29 | 11 | 9% | • Esteja começando os estudos agora; — Isaque Concursos |
| Nível médio | 7 | 7% | 20 | 6% | 8 | 6 | 5% | Para você ter uma ideia, eu só me formei no ensino médio por meio do ENCCEJA, já que tinha repetido em todas as matérias. — Isaque Concursos |
| Reta final / pós-edital | 7 | 7% | 15 | 4% | 29 | 5 | 4% | Com estratégia, planejamento e acompanhamento, você consegue construir uma base mais forte agora e evitar a correria do pós-edital. — Concurseiro aos 40 |
| Nível superior / Direito | 5 | 5% | 5 | 1% | 21 | 2 | 2% | Trata-se de uma oportunidade de nível superior com MUITAS vagas, e uma remuneração inicial muito atrativa. — Concursos Ceisc |
| Erra questões / pegadinhas da banca | 4 | 4% | 6 | 2% | 25 | 2 | 2% | O que trava a maioria é achar que pra passar tem que saber a matéria inteira. Você abre o edital gigante, tenta decorar tudo e chega no dia da prova travado, po — Gustavo Nogueira - Aprovação Ágil |
| Mãe / família | 3 | 3% | 7 | 2% | 57 | 6 | 5% | Se isso não fosse o bastante, eu tive uma infância/adolescência bem difícil. Sou filho de ex -empregada doméstica e, por isso, não tínhamos condições financeira — Isaque Concursos |
| Perdido no excesso de conteúdo | 2 | 2% | 5 | 1% | 64 | 3 | 2% | O que trava a maioria é achar que pra passar tem que saber a matéria inteira. Você abre o edital gigante, tenta decorar tudo e chega no dia da prova travado, po — Gustavo Nogueira - Aprovação Ágil |

## Tipo de produto × ticket

Tipo identificado por palavras-chave na copy, no título do link e na headline (uma oferta pode ter vários). Ticket só entra quando foi lido no checkout.

| Tipo de produto | Anunciantes | Ofertas | Veteranas | Com ticket lido | Mínimo | Mediana | Máximo | Tickets lidos |
|---|---|---|---|---|---|---|---|---|
| Material em PDF / apostila / caderno | 46 | 52 | 27 | 4 | R$ 497 | R$ 547 | R$ 1.489 | Academia do Perito R$ 497; Caderno do Aprovado - Materiais para Concursos R$ 497; Caderno do Aprovado - Materiais para Concursos R$ 597; Discursiva na Prática R$ 1.489 |
| Curso em videoaulas | 23 | 34 | 20 | 4 | R$ 597 | R$ 1.158 | R$ 6.346 | Caderno do Aprovado - Materiais para Concursos R$ 597; Instituto INAPI R$ 827; Discursiva na Prática R$ 1.489; Ceisc Concursos R$ 6.346 |
| Isca gratuita / grupo VIP | 21 | 31 | 9 | 5 | R$ 497 | R$ 827 | R$ 6.346 | Isaque Concursos R$ 497; Caderno do Aprovado - Materiais para Concursos R$ 597; Instituto INAPI R$ 827; Jus Expert R$ 997; Ceisc Concursos R$ 6.346 |
| Mentoria / acompanhamento | 19 | 23 | 12 | 1 | R$ 497 | R$ 497 | R$ 497 | Isaque Concursos R$ 497 |
| Questões / simulados | 17 | 24 | 8 | 2 | R$ 597 | R$ 712 | R$ 827 | Caderno do Aprovado - Materiais para Concursos R$ 597; Instituto INAPI R$ 827 |
| Não identificado | 16 | 18 | 7 | 4 | R$ 1.725 | R$ 1.961 | R$ 2.197 | Escola Trabalhista R$ 1.725; prof.camilasabongi com Escola Trabalhista R$ 1.725; Escola Trabalhista R$ 2.197; prof.camilasabongi com Escola Trabalhista R$ 2.197 |
| Cronograma / plano de estudos | 14 | 19 | 7 | 1 | R$ 497 | R$ 497 | R$ 497 | Isaque Concursos R$ 497 |
| Discursiva / redação | 8 | 9 | 3 | 2 | R$ 597 | R$ 1.043 | R$ 1.489 | Caderno do Aprovado - Materiais para Concursos R$ 597; Discursiva na Prática R$ 1.489 |
| Lei seca / legislação | 8 | 9 | 5 | 2 | R$ 497 | R$ 498 | R$ 500 | Caderno do Aprovado - Materiais para Concursos R$ 497; minhajornadadeconcurseira com Decorando a Lei Seca Cursos Para Concursos E OAB R$ 500 |
| Assinatura / clube / vitalício | 4 | 4 | 2 | 3 | R$ 500 | R$ 598 | R$ 1.489 | minhajornadadeconcurseira com Decorando a Lei Seca Cursos Para Concursos E OAB R$ 500; Mapas da Lulu Concurseira com Laura Amorim R$ 598; Discursiva na Prática R$ 1.489 |
| Mapas mentais / esquemas | 4 | 4 | 2 | 2 | R$ 497 | R$ 547 | R$ 598 | Caderno do Aprovado - Materiais para Concursos R$ 497; Mapas da Lulu Concurseira com Laura Amorim R$ 598 |

## Expressões repetidas entre anunciantes

Sequências de 2 ou 3 palavras (sem acento) usadas na copy por 3 ou mais anunciantes distintos.

`clique em saiba` (19), `tecnico judiciario` (12), `garanta sua vaga` (11), `concurso publico` (9), `edital sair` (8), `analista judiciario` (8), `agora mesmo` (8), `remuneracao inicial` (7), `realmente cai` (7), `concursos publicos` (7), `tribunal de contas` (6), `sair para comecar` (6), `quem quer` (6), `pre edital` (6), `novo concurso` (6), `link da bio` (6), `concurso do trt` (6), `tribunal regional` (5), `tribunal de justica` (5), `toque em saiba` (5), `tj sp` (5), `pos edital` (5), `pode sair` (5), `nivel superior` (5), `lei seca` (5), `ensino medio` (5), `direito do trabalho` (5), `curso completo` (5), `clique no link` (5), `1o lugar` (5)

## Arquivo de ganchos (anúncios mais replicados e mais antigos)

| Anunciante | Dias | Cópias | Formato | Botão | Gancho (1ª linha) | Título do link |
|---|---|---|---|---|---|---|
| MEQ Concursos | 8 | 8 | imagem | sem botão | Se o edital do seu TRT saísse amanhã, você estaria pronto para fazer a prova? |  |
| Isaque Concursos | 57 | 4 | vídeo | sem botão | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? |  |
| Caminho da Perícia | 29 | 4 | imagem | Saiba mais | 🚨 PROCURA-SE PEDAGOGOS🚨 | Vagas para profissionais formados |
| Caminho da Perícia | 29 | 4 | imagem | Saiba mais | 🚨 PROCURA-SE VETERINÁRIOS🚨 | Vagas para profissionais formados |
| Caminho da Perícia | 29 | 4 | vídeo | sem botão | 🚨 PROCURA-SE ENGENHEIROS AGRÔNOMOS🚨 | Vagas para profissionais formados |
| Caminho da Perícia | 29 | 4 | vídeo | Saiba mais | 🚨 PROCURA-SE ENGENHEIROS CIVIS🚨 | Vagas para profissionais formados |
| Caminho da Perícia | 29 | 4 | imagem | Saiba mais | 🚨 PROCURA-SE ADVOGADOS! 🚨 | Vagas para profissionais formados |
| Clube do Perito | 14 | 4 | imagem | sem botão | 🚨 PROCURA-SE FISIOTERAPEUTAS🚨 |  |
| Clube do Perito | 13 | 4 | imagem | sem botão | 🚨 PROCURA-SE PSICÓLOGOS🚨 |  |
| EnfConcursos | 891 | 3 | vídeo | sem botão | Curso Completo com Mentoria e Aulas Diários para o Concurso da EBSERH |  |
| Nova Concursos | 47 | 3 | imagem | sem botão | "📚🆓 Curso Grátis TJ-SP 2026 - Escrevente Técnico Judiciário! 🆓📚 |  |
| Supremo Concursos | 32 | 3 | imagem | sem botão | Não é falta de dedicação. É falta de direção. |  |
| Concurseiro aos 40 | 22 | 3 | imagem | sem botão | ⚖️ Os próximos concursos de TRTs podem abrir excelentes oportunidades em diferentes regiões do país, com remunerações iniciais que podem chegar a cerca de R$ 16 mil. |  |
| Professor Fabiano Pereira | 16 | 3 | vídeo | sem botão | 👀 CONCURSOS DE TRTs EM 2026! |  |
| Gazeta dos Concursos | 13 | 3 | vídeo | sem botão | Atravessei a faculdade de Direito decorando manual, virando noites, com a sensação de que estudar é sofrer. Quando comecei a pensar em TRT, achei que ia ser mais do mesmo. |  |
| Concurseiro aos 40 | 10 | 3 | vídeo | sem botão | 🔥 O TRT-MG já começou a se movimentar para um novo concurso em 2027. |  |
| Metodo.Gafanhoto | 10 | 3 | vídeo | sem botão | INDICAÇÃO CONCURSO PARA MULHERES QUE NÃO TEM BASE NOS ESTUDOS |  |
| Professor Hansk | 8 (baixo volume) | 3 | vídeo | sem botão | Você estuda, se prepara, domina o conteúdo… mas ainda trava na hora da redação? 📝 |  |
| Trteiros | 120 | 2 | vídeo | sem botão | 🚨Informações sobre o TRT/MG |  |
| Trteiros | 120 | 2 | vídeo | sem botão | 🚨Informações sobre o TRT/BA |  |
| Tjteiros | 96 | 2 | vídeo | sem botão | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. |  |
| Central de Concursos | 85 | 2 | vídeo | sem botão | O concurso do Tribunal de Justiça de São Paulo (TJ-SP) é uma das maiores oportunidades para quem tem apenas o ensino médio completo. Além de um excelente salário inicial, você conquista estabilidade financeira, benefício |  |
| Estratégia Concursos | 83 | 2 | vídeo | sem botão | 📢 O professor Herbert Almeida indica: vale a pena estudar para CGU e Tribunal de Contas da União! |  |
| Venâncio & Delgado - Advogados | 57 | 2 | vídeo | sem botão | ⚖️ A banca examinadora pode mudar de entendimento e te eliminar como PCD? Saiba o que o Superior Tribunal de Justiça (STJ) decidiu! |  |
| Milena Correia Advocacia | 22 | 2 | vídeo | sem botão | Irregularidades em concursos públicos podem arruinar seus sonhos! |  |
| Concurseiro aos 40 | 16 | 2 | imagem | sem botão | 🔥 Começar depois dos 40 não significa estar atrasado. |  |
| Gustavo Nogueira - Aprovação Ágil | 13 | 2 | vídeo | sem botão | Funciona — e melhor: não é sorte, é conta. |  |
| Sensei da Aprovação - Concursos Públicos | 12 | 2 | vídeo | sem botão | Edital da Prefeitura de Curitiba publicado! 🚨 |  |
| EG Raiz - I.A | 10 | 2 | vídeo | sem botão | 🚨 HOJE TEM LIVE PRIVADA COM EVANDRO GUEDES! 🚨 |  |
| minhajornadadeconcurseira com Decorando a Lei Seca Cursos Para Concursos E OAB | 10 | 2 | vídeo | sem botão | A Lei Seca sempre foi uma das minhas maiores aliadas nos estudos. Foi através dela que consegui várias aprovações em concursos - inclusive a que garantiu a minha nomeação. |  |
| Meirelles Quintella Escritório de Advocacia | 9 | 2 | vídeo | sem botão | Alguns profissionais da área da saúde atuam em hospitais públicos sem ter ingressado por concurso. |  |
| Advogado de concurso | 9 | 2 | vídeo | sem botão | 🚨 Fez a prova discursiva do TCE-RS? |  |
| Caderno do Aprovado - Materiais para Concursos | 923 | 1 | imagem | sem botão | A matéria para concurso já é grande e os cursinhos ainda complicam mais: centenas de horas de videoaulas e milhares de páginas de PDFs. | Simbora Concursos |
| Simbora Concursos | 923 | 1 | carrossel | Visitar perfil do Instagram | Quando eu comecei a estudar para Tribunais, ficar "nas cabeças" era algo inimaginável... 1º lugar, então? Era coisa de maluco, extraterrestre, etc. |  |
| Caderno do Aprovado - Materiais para Concursos | 833 | 1 | carrossel | Visitar perfil do Instagram | Lançados em junho de 2024 |  |
| Caderno do Aprovado - Materiais para Concursos | 784 | 1 | carrossel | Visitar perfil do Instagram | Lançados em agosto de 2024 |  |
| Caderno do Aprovado - Materiais para Concursos | 709 | 1 | carrossel | Visitar perfil do Instagram | Lançados em outubro de 2024 |  |
| Caderno do Aprovado - Materiais para Concursos | 615 | 1 | vídeo | sem botão | 3 cenários de APROVAÇÃO ✅️ |  |
| Caderno do Aprovado - Materiais para Concursos | 615 | 1 | vídeo | sem botão | O caderno de Português do 1º lugar no TRT-PI, com toda a teoria organizada de forma objetiva + questões comentadas das 3 principais bancas de concurso (FCC, FGV e Cespe/Cebraspe). |  |
| Caderno do Aprovado - Materiais para Concursos | 611 | 1 | carrossel | Visitar perfil do Instagram | Lançados em fevereiro de 2025 |  |

---

# Parte 1 — Ofertas de foco direto (60)

---
id_oferta: 001
anunciante: "Concurseiro aos 40"
url_destino: "https://form.respondi.app/CN2Wk6Lk"
ad_library_url: "https://www.facebook.com/ads/library/?id=1085157223929037"
dias_ativo: 22
anuncios_coletados: 11
anuncios_ativos_estimados: 29
anuncios_com_baixo_volume_de_impressoes: 2
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, justica do trabalho"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "vídeo (4), imagem (7)"
botoes: "sem botão (11)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
- 🔥 O TRT-MG já começou a se movimentar para um novo concurso em 2027.
- ⚖️ Os próximos concursos de TRTs podem abrir excelentes oportunidades em diferentes regiões do país, com remunerações iniciais que podem chegar a cerca de R$ 16 mil.
- 🔥 Começar depois dos 40 não significa estar atrasado.

### Landing Page: Headline & Promessa Central
"Inicie o passo mais importante rumo à sua aprovação no Concurso do TRT"

### Entregáveis / Formato (termos encontrados na LP)
- Mentoria


========================================

---
id_oferta: 002
anunciante: "Leandro Reinhardt l Estudos & Concursos"
url_destino: "https://leandroreinhardt.com.br/trt-desafio-nucleo-duro-tjaa/?utm_source=meta-ads&utm_medium=%7B%7Badset.name%7D%7D%7C%7B%7Badset.id%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D%7C%7B%7Bcampaign.id%7D%7D&utm_content=%7B%7Bad.name%7D%7D%7C%7B%7Bad.id%7D%7D&utm_term=%7B%7Bplacement%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1667286944925819"
dias_ativo: 10
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
dias_distintos_coletado: 1
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
id_oferta: 003
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://www.facebook.com/simboraconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=436273172079349"
dias_ativo: 923
anuncios_coletados: 20
anuncios_ativos_estimados: 20
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trt, tst"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Cronograma / plano de estudos"
formatos_dos_anuncios: "carrossel (13), vídeo (4), imagem (3)"
botoes: "Visitar perfil do Instagram (8), sem botão (12)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
- Não sei se a ficha já caiu por aí, mas vocês serão servidores públicos do Poder Judiciário cearense. 😮🙏👏
- Lançados em agosto de 2025
- Lançados em fevereiro de 2025
- 3 cenários de APROVAÇÃO ✅️
- O caderno de Português do 1º lugar no TRT-PI, com toda a teoria organizada de forma objetiva + questões comentadas das 3 principais bancas de concurso (FCC, FGV e Cespe/Cebraspe).
- Lançados em outubro de 2024

### Títulos do link nos anúncios
- Beto (José Humberto) - Caderno Do Aprovado - TRT/TST/TJ/MP (@cadernoaprovado) • Instagram photos and videos
- Beto - Caderno Do Aprovado - TRT, TST e TJ - José Humberto (@cadernoaprovado) • Instagram photos and videos
- Simbora Concursos

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 004
anunciante: "MEQ Concursos"
url_destino: "https://meqconcursos.com.br/concurso-simulado-meq-2-analista-trt-v2-l/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1621902522644946"
dias_ativo: 8
anuncios_coletados: 6
anuncios_ativos_estimados: 20
anuncios_com_baixo_volume_de_impressoes: 1
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados, Discursiva / redação, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (6)"
botoes: "sem botão (2), Saiba mais (4)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
id_oferta: 005
anunciante: "Leandro Reinhardt l Estudos & Concursos"
url_destino: "https://leandroreinhardt.com.br/trt-desafio-nucleo-duro/?utm_source=meta-ads&utm_medium=%7B%7Badset.name%7D%7D%7C%7B%7Badset.id%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D%7C%7B%7Bcampaign.id%7D%7D&utm_content=%7B%7Bad.name%7D%7D%7C%7B%7Bad.id%7D%7D&utm_term=%7B%7Bplacement%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1383702350413675"
dias_ativo: 10
anuncios_coletados: 16
anuncios_ativos_estimados: 16
anuncios_com_baixo_volume_de_impressoes: 5
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados"
formatos_dos_anuncios: "imagem (16)"
botoes: "Saiba mais (16)"
precos_exibidos_na_lp: "R$ 297 | R$ 97 | 12x de R$ 9,70"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"<100
De R$ 297 por R$ 97, menos de R$ 1,40 por dia
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
id_oferta: 006
anunciante: "Isaque Concursos"
url_destino: "https://projetotrt.com.br/imersao1v1/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1556242356236977"
dias_ativo: 61
anuncios_coletados: 5
anuncios_ativos_estimados: 15
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tecnico judiciario"
plataforma_checkout: "onprofit"
ticket_principal: "R$ 497,00"
fonte_ticket: "checkout"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (5)"
botoes: "sem botão (4), Saiba mais (1)"
parcelas: "12x R$ 42,99"
precos_exibidos_na_lp: "R$ 9.776,71 | R$ 90,00 | R$ 11.928 | R$ 0 | R$ 997 | R$ 100 | R$ 497 | R$ 397"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
id_oferta: 007
anunciante: "Portal & OAB"
url_destino: "https://olympus.cursosdoportal.com.br/o-adm-trt-pa/?utm_source=%7B%7Bsite_source_name%7D%7D&utm_medium=%7B%7Badset.name%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D&utm_term=%7B%7Bplacement%7D%7D&utm_content=%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1074976398625545"
dias_ativo: 9
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
dias_distintos_coletado: 1
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
anunciante: "Nova Concursos"
url_destino: "https://aprovacao.novaconcursos.com.br/curso-gratis-tj-sp-escrevente-ads-ca2"
ad_library_url: "https://www.facebook.com/ads/library/?id=1621019016255950"
dias_ativo: 48
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
dias_distintos_coletado: 1
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
id_oferta: 009
anunciante: "Trteiros"
url_destino: "https://www.facebook.com/61560675890210/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1931729394374222"
dias_ativo: 166
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
dias_distintos_coletado: 1
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
id_oferta: 010
anunciante: "Professor Fabiano Pereira"
url_destino: "https://aprovatte.com.br/mentoria-start90-2025/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2193225251609967"
dias_ativo: 16
anuncios_coletados: 2
anuncios_ativos_estimados: 6
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento"
formatos_dos_anuncios: "vídeo (2)"
botoes: "sem botão (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"👀 CONCURSOS DE TRTs EM 2026!
Se você está de olho em um concurso de tribunal do trabalho, aqui vai uma informação importante: em 2026, vencem concursos importantes de vários TRTs, como TRT-PI, TRT-PR, TRT-RS e TRT-MT.
E o sinal de alerta já foi dado: o TRT-RS autorizou um novo concurso antes mesmo do atual expirar. Isso deixa claro que quem deixar para estudar só depois do edital vai sair atrás.
Nos últimos concursos de TRTs aprovamos centenas de alunos, incluindo o Roberto Frois, que conquistou o 1º lugar para Analista Judiciário do TRT MT, errando apenas uma questão na prova.
Se você quer estar entre os próximos aprovados, o melhor momento para começar é agora.
👉 Clique em SAIBA MAIS e receba todas as informações sobre a minha mentoria, que é completa e foi pensada exatamente para quem quer passar em concursos de TRTs."

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
id_oferta: 011
anunciante: "Decorando a Lei Seca Cursos Para Concursos E OAB"
url_destino: "https://www.facebook.com/decorandoaleisecaconcursoseoab/"
ad_library_url: "https://www.facebook.com/ads/library/?id=792696320220760"
dias_ativo: 185
anuncios_coletados: 5
anuncios_ativos_estimados: 5
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trt, tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Assinatura / clube / vitalício, Material em PDF / apostila / caderno"
formatos_dos_anuncios: "carrossel (3), imagem (2)"
botoes: "Visitar perfil do Instagram (3), sem botão (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O art. 6º da Lei 14.133/2021 é, hoje, um dos dispositivos mais cobrados em concursos públicos. Só em provas da FGV e do CEBRASPE, já apareceu mais de 40 vezes.
Alguns exemplos recentes:
FGV 2025 – Juiz de Direito (TJ-MS)
CEBRASPE 2023 – Promotor de Justiça (MPE-AM)
CEBRASPE 2022 – Defensor Público (DPE-SE)
CEBRASPE 2022 – Técnico Processual (PGE-RJ)
CEBRASPE 2022 – Delegado de Polícia (PC-RO)
FGV 2022 – Analista Judiciário (TRT-16)
FGV 2022 – Analista Judiciário (TRT-13)
FGV 2022 – Técnico Judiciário (TJ-TO)
E não é algo recente: esse dispositivo já vem sendo explorado há anos — principalmente por FGV e CEBRASPE.
A leitura é simples: quem estuda os artigos mais cobrados, sai na frente.
E é exatamente isso que o VMQ entrega:
um direcionamento claro, baseado em provas, mostrando o que realmente importa na sua preparação.
Quer estudar com mais estratégia e foco no que mais cai?
Clica no link da bio e aproveita a promoção de Aniversário para entrar na Ilimitada 🚀"

### Ganchos das variações (1ª linha de cada anúncio)
- O art. 319 do Código Penal caiu no concurso para Promotor do MP-GO!
- O art. 30 do Código Penal é daqueles dispositivos curtos, mas que a banca adora explorar em prova objetiva.
- ⚠️ Uma palavra pode mudar completamente o gabarito da questão.
- O art. 6º da Lei 14.133/2021 é, hoje, um dos dispositivos mais cobrados em concursos públicos. Só em provas da FGV e do CEBRASPE, já apareceu mais de 40 vezes.

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 012
anunciante: "MEQ Concursos"
url_destino: "https://www.facebook.com/61586241338760/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1652434139167708"
dias_ativo: 140
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
dias_distintos_coletado: 1
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
- Lançados em maio de 2026
- “TRT não vale a pena…”

### Títulos do link nos anúncios
- www.instagram.com

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 013
anunciante: "Isaque Concursos"
url_destino: "https://projetotrt.com.br/vsl1v1/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1023281740551609"
dias_ativo: 61
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
dias_distintos_coletado: 1
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
id_oferta: 014
anunciante: "Instituto INAPI"
url_destino: "https://cursos.inapionline.com.br/pre-trt-pi"
ad_library_url: "https://www.facebook.com/ads/library/?id=1364004345923443"
dias_ativo: 51
anuncios_coletados: 5
anuncios_ativos_estimados: 5
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tecnico judiciario"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 827,00"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Questões / simulados, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (4), imagem (1)"
botoes: "Saiba mais (4), Ver detalhes (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
id_oferta: 015
anunciante: "Escola Trabalhista"
url_destino: "https://escolatrabalhista.com.br/preparacao-acesso-total-trt-tst/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1290097296395901"
dias_ativo: 184
anuncios_coletados: 4
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trt, tst, tecnico judiciario"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 2.197,32"
fonte_ticket: "checkout"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "vídeo (3), imagem (1)"
botoes: "Saiba mais (2), Comprar agora (2)"
parcelas: "12x de R$ 227,26"
precos_exibidos_na_lp: "R$ 1,00 | R$ 2.746,65 | 12x de R$ 284,07"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
id_oferta: 016
anunciante: "Gazeta dos Concursos"
url_destino: "https://lp.aprovacaoagil.com.br/vsl-white-trt-noticia"
ad_library_url: "https://www.facebook.com/ads/library/?id=1356534065929557"
dias_ativo: 75
anuncios_coletados: 4
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tst"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno, Lei seca / legislação"
formatos_dos_anuncios: "vídeo (4)"
botoes: "Saiba mais (4)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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

### Títulos do link nos anúncios
- Melhor tribunal pra começar hoje
- A enxurrada de TRTs começou
- O caminho mais rápido pra R$11.500
- TRT dá com 2 horas por dia?

### Landing Page: Headline & Promessa Central
"Título"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 017
anunciante: "Verbo Carreiras Jurídicas"
url_destino: "https://www.facebook.com/verbocarreirasjuridicas/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1068545759364006"
dias_ativo: 14
anuncios_coletados: 4
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 1
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Curso em videoaulas, Material em PDF / apostila / caderno, Questões / simulados"
formatos_dos_anuncios: "vídeo (3), imagem (1)"
botoes: "Enviar mensagem pelo WhatsApp (4)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Seu próximo passo pode começar agora!
Os concursos dos Tribunais Regionais do Trabalho estão entre as grandes oportunidades para quem busca estabilidade, boa remuneração e uma carreira no serviço público.
Prepare-se com um curso completo, focado nos conteúdos mais importantes para a sua aprovação no TRT Brasil.
📚 Aulas gravadas
🎯 Preparação estratégica
📝 Conteúdo direcionado para concurso
Não espere o edital sair para começar. Antecipe sua preparação!
👉 Comece agora e saia na frente.
WHATSAPP
🚨 Prepare-se para o TRT Brasil
Sobre o curso: 50 encontros, 10 mentorias de Direito do Trabalho e Processo do Trabalho via Zoom; 2 simulados; Grupo exclusivo da turma; Aulas de resoluções de questões ao vivo; Super Revisão."

### Ganchos das variações (1ª linha de cada anúncio)
- Língua Portuguesa e Redação com quem entende de aprovação para o concurso do TRT-4
- <100
- Seu próximo passo pode começar agora!

### Títulos do link nos anúncios
- Por menos de R$5,00 ao dia você aprende Língua Portuguesa para o concurso do TRT-4!
- Se prepare com quem entende de APROVAÇÃO!

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 018
anunciante: "Prime Curso"
url_destino: "https://sala.concurseiroprime.com.br/buscar?query=trt"
ad_library_url: "https://www.facebook.com/ads/library/?id=1129411490041604"
dias_ativo: 12
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
dias_distintos_coletado: 1
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
id_oferta: 019
anunciante: "Nova Concursos"
url_destino: "https://aprovacao.novaconcursos.com.br/curso-gratis-tj-sp-escrevente-ads-great"
ad_library_url: "https://www.facebook.com/ads/library/?id=2193053974942953"
dias_ativo: 8
anuncios_coletados: 4
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Questões / simulados, Cronograma / plano de estudos, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (4)"
botoes: "Ver detalhes (4)"
precos_exibidos_na_lp: "R$ 297,00 | R$ 0,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
id_oferta: 020
anunciante: "prof.camilasabongi com Escola Trabalhista"
url_destino: "https://escolatrabalhista.com.br/preparacao-acesso-total-trt-tst/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1278772247787449"
dias_ativo: 180
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trt, tst, tecnico judiciario"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 2.197,32"
fonte_ticket: "checkout"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "vídeo (3)"
botoes: "Saiba mais (2), Comprar agora (1)"
parcelas: "12x de R$ 227,26"
precos_exibidos_na_lp: "R$ 1,00 | R$ 2.746,65 | 12x de R$ 284,07"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
id_oferta: 021
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2089-concurso-trt-4-club-analista-judiciario-area-judiciaria"
ad_library_url: "https://www.facebook.com/ads/library/?id=1574927696942677"
dias_ativo: 165
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trt, tribunal regional do trabalho, trt 4"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "imagem (3)"
botoes: "Saiba mais (2), Ver detalhes (1)"
precos_exibidos_na_lp: "R$ 16 | R$ 16.041,21 | R$ 10 | R$ 2.137,00 | R$ 1.389,05 | 12x de R$ 115,75"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"A sua oportunidade de atuar no estado do Rio Grande do Sul, pelo Tribunal Regional do Trabalho, está chegando!
O último concurso expira sua validade em outubro e, segundo o histórico do Tribunal, o próximo já deve ser anunciado em breve.
Este é o momento ideal para iniciar sua preparação, com um curso que conhece a fundo o órgão e suas exigências. Quem inicia antes do edital vai mais longe!
Entenda como se preparar antecipadamente."

### Ganchos das variações (1ª linha de cada anúncio)
- A sua oportunidade de atuar no estado do Rio Grande do Sul, pelo Tribunal Regional do Trabalho, está chegando!
- O TRT-4 pode estar prestes a anunciar um novo concurso!
- Se preparar para tribunais exige método.

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
id_oferta: 022
anunciante: "Meirelles Quintella Escritório de Advocacia"
url_destino: "https://www.facebook.com/100090050235471/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2118332055398747"
dias_ativo: 154
anuncios_coletados: 2
anuncios_ativos_estimados: 3
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
dias_distintos_coletado: 1
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
id_oferta: 023
anunciante: "Supremo Concursos"
url_destino: "https://www.supremotv.com.br/analista-judiciario-e-oficial-de-justica-trt-3"
ad_library_url: "https://www.facebook.com/ads/library/?id=1519897813487712"
dias_ativo: 32
anuncios_coletados: 1
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt 3"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (1)"
botoes: "sem botão (1)"
precos_exibidos_na_lp: "R$ 1.197,00 | R$ 797,00 | 12x de R$ 79,70"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Não é falta de dedicação. É falta de direção.
A maioria dos concurseiros passa meses abrindo PDF, assistindo aula aleatória e repetindo o ciclo, sem saber se está no caminho certo para a aprovação.
O Supremo resolve exatamente isso: cronogramas estruturados, aulas na sequência certa e professores que já foram aprovados nas carreiras que você quer seguir.
Método muda resultado.
Aperte em Saiba Mais e começa do jeito certo."

### Landing Page: Headline & Promessa Central
"Analista Judiciário e Oficial de Justiça TRT 3ª Região (Direito) 2026 / 2027 - Pré-Edital — 🎯 TRT 3ª Região Direito (Analista Judiciário e Oficial de Justiça) 2026 / 2027 - Pré-Edital"

### Seções da Landing Page (títulos, na ordem)
- 🎯 TRT 3ª Região Direito (Analista Judiciário e Oficial de Justiça) 2026 / 2027 - Pré-Edital

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- PDF


========================================

---
id_oferta: 024
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://cadernodoaprovado.com/trt-v2/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1474311188085385"
dias_ativo: 26
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, justica do trabalho, tst"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 597,00"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno, Questões / simulados, Discursiva / redação, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "carrossel (3)"
botoes: "sem botão (3)"
precos_exibidos_na_lp: "R$ 9.776,71 | R$ 1.089,00 | 12x de R$ 49,75 | R$ 16.040,88 | R$ 1.188,00 | 12x de R$ 53,92 | R$ 1.386,00 | 12x de R$ 62,25"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps:
  - nome: "[REDAÇÃO IMBATÍVEL] Guia de redação dissertativa-argumentativa para concursos"
    valor: "R$ 149,00"
  - nome: "[COMBO TRF-3] Técnico Judiciário - Área Administrativa (Nível"
    valor: "R$ 547,00"
  - nome: "[COMBO TRF-3] Analista Judiciário - Área Judiciária (Nível"
    valor: "R$ 647,00"
  - nome: "[COMBO TJ-SP] Escrevente Técnico Judiciário (Nível Médio) 78%"
    valor: "R$ 447,00"
  - nome: "[COMBO MP-PE] Técnico Ministerial - Área Administrativa (Nível"
    valor: "R$ 497,00"
  - nome: "[COMBO MP-PE] Analista Ministerial - Área Jurídica (Nível"
    valor: "R$ 497,00"
---
### Copy do Anúncio (Gancho de Entrada)
"Como se preparar em alto nível para os próximos concursos de TRT:
✅ Meus cadernos completos das 6 principais disciplinas para TRT (Português, Constitucional, Administrativo, Adm.Pública, Trabalho e Processo).
✅️ Guia de estudos com 100 metas para vencer o edital.
✅ Planilha de controle de revisões e questões.
✅ Videoaulas gratuitas de cada tema com os melhores professores.
✅ Módulo sobre prova discursiva, com meu resumo de redação, dicas de preparação e materiais extras.
✅ Todas as provas recentes de TRT organizadas e com correção em vídeo.
✅ Regimento interno grifado e destacado.
✅ Súmulas e OJs organizadas por assunto.
✅ E muito mais.
Clique em saiba mais para receber todas as informações e amostras."

### Títulos do link nos anúncios
- See Details

### Landing Page: Headline & Promessa Central
"Combos TRT e TST – Caderno do Aprovado (v2 – longa – campeã) – Caderno do Aprovado – Materiais de estudos para concursos públicos — Estude para os próximos concursos da Justiça do Trabalho com o 1º lugar ."

### Seções da Landing Page (títulos, na ordem)
- Estude para os próximos concursos da Justiça do Trabalho com o 1º lugar .
- 1º lugar
- O Caderno do Aprovado resolve isso organizando tudo em um só lugar.
- Tudo pronto para estudar, revisar e avançar.
- Conheça por dentro.
- A diferença está em quem faz e em como é feito.
- Oi, eu sou o Beto.
- Quais serão os próximos concursos de TRTs?
- Minas Gerais
- Rio Grande do Sul
- Pará e Amapá
- Mato Grosso
- Prepare-se em alto nível para os próximos concursos da Justiça do Trabalho.
- (Sem juros)
- GUIA DE ESTUDOS
- Bônus 2 - Planilha de controle de estudos
- Bônus 3 - Súmulas e OJs organizadas por assunto
- Bônus 3 - Provas anteriores
- Bônus 4 - Atualizações a cada edital
- Sem riscos, com garantia de 7 dias para ter certeza.
- O material de estudos dos primeiros colocados!
- Estudar sozinho x Estudar com o Caderno do Aprovado
- Para ficar despreocupado(a) pelos próximos 2 anos
- 12x de R$ 116,42
- Dúvidas frequentes e suas respostas.
- Outras dúvidas?
- Prefere escolher apenas algumas disciplinas?

### Entregáveis / Formato (termos encontrados na LP)
- Caderno de erros
- Cronograma
- Discursiva / redação
- PDF
- Resumos
- Simulados
- Videoaulas


========================================

---
id_oferta: 025
anunciante: "Concursos Ceisc"
url_destino: "https://lp.ceisc.com.br/material-concurso-trt-4-projeto-nomeacao/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2481638218987806"
dias_ativo: 26
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt 4"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (3)"
botoes: "Saiba mais (3)"
precos_exibidos_na_lp: "R$ 14"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Muitos concursos de Tribunais são esperados para 2026.
Uma dessas oportunidades será do TRT-4 (RS), com previsão de 300 vagas destinadas às carreiras de Analista e Técnico.
Com o Ceisc, você já pode SAIR NA FRENTE da concorrência SEM PAGAR NADA.
O Projeto Nomeação TRT-4 está oficialmente aberto.
Toque no botão e garanta a sua vaga para receber conteúdos exclusivos do concurso iminente! 🚀
Material Gratuito"

### Ganchos das variações (1ª linha de cada anúncio)
- Saia na frente em um dos concursos mais esperados do Sul do Brasil.
- Muitos concursos de Tribunais são esperados para 2026.
- A comissão organizadora do novo concurso do TRT-4 (RS) já foi formada.

### Landing Page: Headline & Promessa Central
"E foi feito por quem já garantiu: — Conte com o time dos sonhos para guiar você até a nomeação!"

### Seções da Landing Page (títulos, na ordem)
- Saia na frente em um dos concursos mais esperados do Sul do Brasil em 2026.
- Aulas Disponíveis
- Inscreva-se e participe!
- E MUITO MAIS CONTEÚDO GRATUITO
- A oportunidade que pode mudar a sua vida começa agora!
- Mais de 300 vagas previstas para Analista e Técnico
- Remuneração inicial de até R$ 14,8 mil/mês
- Estabilidade e plano de carreira sólido
- Último concurso nomeou mais de 500 aprovados
- A Preparação para o TRT-4 começa com direcionamento: baixe gratuitamente o plano de estudos.
- Ganhe tempo
- Exclusivo para inscritos
- ✅ Garantiram 100% de aprovação dos alunos da PC-SP Prova Oral
- ✅ 7 dos 10 primeiros colocados do TJ-RS foram nossos alunos
- ✅ Entregaram 70% das questões do TJ-SP Escrevente durante a Revisão Turbo

### Entregáveis / Formato (termos encontrados na LP)
- PDF


========================================

---
id_oferta: 026
anunciante: "Professor Fabiano Pereira"
url_destino: "https://www.facebook.com/professorfp/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1622749052884640"
dias_ativo: 16
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
dias_distintos_coletado: 1
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
anunciante: "Gazeta dos Concursos"
url_destino: "https://lp.aprovacaoagil.com.br/vsl-white-trt-rs"
ad_library_url: "https://www.facebook.com/ads/library/?id=935737822481545"
dias_ativo: 13
anuncios_coletados: 1
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tst"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados, Lei seca / legislação, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (1)"
botoes: "sem botão (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
id_oferta: 028
anunciante: "Escola Trabalhista"
url_destino: "https://conteudos.escolatrabalhista.com.br/raio-x"
ad_library_url: "https://www.facebook.com/ads/library/?id=1566347627818236"
dias_ativo: 247
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tst"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (2)"
botoes: "Saiba mais (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"❌ Estudar tudo não te aprova em TRT.
✅ Estudar o núcleo certo, sim.
O edital muda nos detalhes.
O que decide a prova quase nunca muda.
📘 Baixe grátis o Raio-X Analista Judiciário TRTs
e estude com foco no que realmente cai em TRT e TST.
👉 Download gratuito."

### Landing Page: Headline & Promessa Central
"Raio X - Escola Trabalhista"

### Entregáveis / Formato (termos encontrados na LP)
- PDF


========================================

---
id_oferta: 029
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2092-concurso-tj-sp-club-escrevente-tecnico-judiciario?utm_source=meta_ads&utm_medium=cpc&utm_campaign=vendas_tj_sp_escrevente"
ad_library_url: "https://www.facebook.com/ads/library/?id=864887869547603"
dias_ativo: 131
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
precos_exibidos_na_lp: "R$ 6 | R$ 6.345,94 | R$ 1.797,00 | R$ 1.078,20 | 12x de R$ 89,85"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
id_oferta: 030
anunciante: "Ceisc Concursos"
url_destino: "https://lp.ceisc.com.br/projeto-nomeacao-tj-sp/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2095494471007965"
dias_ativo: 86
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "sympla"
ticket_principal: "R$ 6.345,94"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (2)"
botoes: "Ver detalhes (1), Inscreva-se (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
id_oferta: 031
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2138-concurso-trt-4-club-tecnico-judiciario-area-administrativa?utm_source=meta_ads&utm_medium=cpc&utm_campaign=vendas_trt_4_club_tec_judiciario&utm_term=advantage"
ad_library_url: "https://www.facebook.com/ads/library/?id=1020843757391368"
dias_ativo: 84
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
dias_distintos_coletado: 1
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
id_oferta: 032
anunciante: "Prof. Bruno Klippel"
url_destino: "http://www.brunoklippel.com.br/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1660718711665340"
dias_ativo: 76
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
dias_distintos_coletado: 1
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
id_oferta: 033
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://cadernodoaprovado.com/trf-tj-mp/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1533733075435407"
dias_ativo: 64
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
dias_distintos_coletado: 1
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
id_oferta: 034
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://cadernodoaprovado.com/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1808412633912288"
dias_ativo: 29
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
dias_distintos_coletado: 1
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
id_oferta: 035
anunciante: "Supremo Concursos"
url_destino: "https://www.supremotv.com.br/"
ad_library_url: "https://www.facebook.com/ads/library/?id=38412951095018403"
dias_ativo: 21
anuncios_coletados: 1
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (1)"
botoes: "sem botão (1)"
precos_exibidos_na_lp: "R$ 1.997,00 | R$ 1.497,00 | 12x de R$ 149,70 | R$ 1.197,00 | 12x de R$ 119,70 | R$ 997,00 | 12x de R$ 99,70 | R$ 3.997,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Não é falta de dedicação. É falta de direção.
A maioria dos concurseiros passa meses abrindo PDF, assistindo aula aleatória e repetindo o ciclo, sem saber se está no caminho certo para a aprovação.
O Supremo resolve exatamente isso: cronogramas estruturados, aulas na sequência certa e professores que já foram aprovados nas carreiras que você quer seguir.
Método muda resultado.
Aperte em Saiba Mais e começa do jeito certo."

### Landing Page: Headline & Promessa Central
"Supremo TV - De mãos dadas até a aprovação! — Escolha por categoria"

### Seções da Landing Page (títulos, na ordem)
- Escolha por categoria
- Cursos em Destaque
- Delegado de Polícia Civil Minas Gerais 2027 - Edital Confirmado
- Investigador de Polícia Civil Minas Gerais 2027 - Edital Confirmado
- Procurador do Município de Belo Horizonte 2026 / 2027 - Pré-Edital
- Delegado de Polícia Civil Pernambuco 2026 - Edital Publicado
- Procurador do Município de Curitiba - Edital Publicado 2026
- Procurador do Município de Santa Luzia - Edital Publicado 2026
- Clube da Casa do Delegado 2026 / 2027
- Carreiras Jurídicas
- Analista Judiciário e Oficial de Justiça TRT 3ª Região (Direito) 2026 / 2027 - Pré-Edital
- Hora H Delegado de Polícia Civil do Paraná
- Delegado de Polícia Civil Rio de Janeiro 2026/2027 - Pré-edital
- AGU 3x1: Advogado da União, Procurador Federal e Procurador da Fazenda Nacional 2026/27 - Pre-Edital
- Delegado de Polícia Civil São Paulo 2026 / 2027 - Pré-edital
- Oficial Judiciário (nível médio) TJMG 2026 /2027 - Pré-edital
- Delegado de Polícia Civil Bahia 2026 - Edital Publicado

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 036
anunciante: "Gustavo Nogueira - Aprovação Ágil"
url_destino: "https://lp.aprovacaoagil.com.br/vsl-white-trt-pa-ap"
ad_library_url: "https://www.facebook.com/ads/library/?id=1076791055219421"
dias_ativo: 13
anuncios_coletados: 1
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tst"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (1)"
botoes: "sem botão (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
id_oferta: 037
anunciante: "GG Concursos"
url_destino: "https://ggconcursos.com.br/cursos/trt4/?cupom=GG-30"
ad_library_url: "https://www.facebook.com/ads/library/?id=2193032804613934"
dias_ativo: 12
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
dias_distintos_coletado: 1
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
id_oferta: 038
anunciante: "Hugo de Freitas"
url_destino: "https://www.facebook.com/hugoconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1567356078474323"
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
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "carrossel (2)"
botoes: "Visitar perfil do Instagram (1), sem botão (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
id_oferta: 039
anunciante: "Simbora Concursos"
url_destino: "https://www.facebook.com/simboraconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=3157233831074462"
dias_ativo: 923
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
dias_distintos_coletado: 1
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
id_oferta: 040
anunciante: "Escola Trabalhista"
url_destino: "https://escolatrabalhista.com.br/preparacao-extensiva-analista-judiciario-do-trt-area-judiciaria/"
ad_library_url: "https://www.facebook.com/ads/library/?id=971307882122417"
dias_ativo: 184
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
dias_distintos_coletado: 1
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
id_oferta: 041
anunciante: "prof.camilasabongi com Escola Trabalhista"
url_destino: "https://escolatrabalhista.com.br/preparacao-extensiva-analista-judiciario-do-trt-area-judiciaria/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1284621483770100"
dias_ativo: 180
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
dias_distintos_coletado: 1
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

### Títulos do link nos anúncios
- prof.camilasabongi

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
id_oferta: 042
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2292-concurso-trt-nacional-club-analista-judiciario-area-judiciaria"
ad_library_url: "https://www.facebook.com/ads/library/?id=2005552620380372"
dias_ativo: 165
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Curso em videoaulas, Questões / simulados"
formatos_dos_anuncios: "vídeo (1)"
botoes: "sem botão (1)"
precos_exibidos_na_lp: "R$ 16 | R$ 11 | R$ 3.710,00 | R$ 2.411,50 | 12x de R$ 200,96"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Um preparatório para diversos concursos de Tribunais Regionais do Trabalho? 🚨
Isso mesmo, otimize seus estudos e tenha um preparo para diversos editais de 2026. 🚀
O TRT Nacional Club oferece mentorias, simulados, conteúdos atualizados pós-editais e muito mais.
Dê o próximo passo rumo ao cargo de Analista Judiciário clicando abaixo!
Equipe de Especialistas
Ceisc
See Details"

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
id_oferta: 043
anunciante: "Concurseiro aos 40"
url_destino: "https://www.facebook.com/61564214427286/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1330662368927610"
dias_ativo: 159
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
dias_distintos_coletado: 1
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
id_oferta: 044
anunciante: "Pódio Procuradorias"
url_destino: "https://cronosconcursos.com.br/livro-fichamento/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1023341813683635"
dias_ativo: 126
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
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"⚖️Fichar é pensar o Direito com estratégia
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
id_oferta: 045
anunciante: "nomaderachel com Focus Concursos Públicos"
url_destino: "https://focusconcursos.com.br/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1937040066929154"
dias_ativo: 82
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
dias_distintos_coletado: 1
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
id_oferta: 046
anunciante: "Nomade Rachel com Focus Concursos Públicos"
url_destino: "https://focusconcursos.com.br:443/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1071730625255558"
dias_ativo: 47
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
dias_distintos_coletado: 1
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
id_oferta: 047
anunciante: "MEQ Concursos"
url_destino: "https://meqconcursos.com.br/amostra-pre-edital/"
ad_library_url: "https://www.facebook.com/ads/library/?id=938466562639552"
dias_ativo: 42
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
dias_distintos_coletado: 1
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
id_oferta: 048
anunciante: "Gustavo Nogueira - Aprovação Ágil"
url_destino: "https://lp.aprovacaoagil.com.br/vsl-white-trt-noticia"
ad_library_url: "https://www.facebook.com/ads/library/?id=1058146883624666"
dias_ativo: 42
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
dias_distintos_coletado: 1
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
id_oferta: 049
anunciante: "Editora Instituto CDT"
url_destino: "https://editora.institutocdt.com.br/produto/libido-masculina-da-fisiologia-a-prescricao"
ad_library_url: "https://www.facebook.com/ads/library/?id=1345385987351355"
dias_ativo: 37
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
dias_distintos_coletado: 1
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
id_oferta: 050
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://lp.cadernodoaprovado.com/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1607407254411907"
dias_ativo: 29
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
dias_distintos_coletado: 1
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
id_oferta: 051
anunciante: "Pratique Concursos"
url_destino: "https://ti.pratiqueconcursos.com.br/fcti/main.html"
ad_library_url: "https://www.facebook.com/ads/library/?id=2307143873373354"
dias_ativo: 27
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
dias_distintos_coletado: 1
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
"Aumente suas chances de aprovação nos concursos de TI — Aprovações em concursos:"

### Seções da Landing Page (títulos, na ordem)
- FCTI - Formação Concursado de TI
- Guia para Concursos (GRÁTIS)
- DATAPREV
- Transpetro
- TCE GO - Técnico de Controle Externo (TI)
- SEPLAG RJ - EPPGG (TI)
- SEFAZ AL - Auditor Fiscal
- Discursivas de TI
- TCE SP Pós Edital
- Curso Regular
- TI para Fiscal e Controle
- Super Intensivo CGU Pré-Edital
- Super Intensivo Perito TI Pré-Edital
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
id_oferta: 052
anunciante: "Portal & OAB"
url_destino: "https://olympus.cursosdoportal.com.br/o-adm-trt-mg/?utm_source=%7B%7Bsite_source_name%7D%7D&utm_medium=%7B%7Badset.name%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D&utm_term=%7B%7Bplacement%7D%7D&utm_content=%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1117950040913904"
dias_ativo: 21
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tribunal regional do trabalho, tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (1)"
botoes: "sem botão (1)"
precos_exibidos_na_lp: "R$ 9.776,71 | R$ 16.040,88"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"O Tribunal Regional do Trabalho de Minas Gerais (TRT/MG) está com novo concurso público confirmado, com previsão de mais de 450 vagas. As oportunidades serão destinadas a candidatos de nível superior, com salários acima de R$ 10 mil.
O concurso segue em fase de preparação, e novas informações sobre cargos, banca, inscrições e demais etapas serão divulgadas com o avanço do certame.
No grupo de estudos, você terá acesso a materiais gratuitos, orientações de estudo, resolução de questões e atualizações sobre edital, cargos, inscrições, provas e todas as etapas do concurso.
Clique em “Saiba Mais” e entre no grupo de WhatsApp para receber materiais gratuitos e acompanhar todas as novidades do concurso do TRT/MG.
See Details"

### Landing Page: Headline & Promessa Central
"Seu próximo capítulo: TRT-MG. Comece a escrever a sua aprovação. — Entre no grupo de estudos GRATUITO e avance com foco disciplina e direção."

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
id_oferta: 053
anunciante: "Nação Jurídica com GGS Advogados Associados"
url_destino: "https://guimasilvadvogados.com.br/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1295807189831029"
dias_ativo: 16
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
dias_distintos_coletado: 1
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
id_oferta: 054
anunciante: "Glaycon Michels -"
url_destino: "https://lp.plenitudeeducacao.com.br/mhorm-lp-tf/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1112538725063936"
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
tipos_produto: "Mentoria / acompanhamento"
formatos_dos_anuncios: "imagem (1)"
botoes: "Ver detalhes (1)"
precos_exibidos_na_lp: "R$ 1.000,00 | 12x de R$ 3.000,00 | R$ 25.200"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🩺 **EXCLUSIVO PARA MÉDICOS**
🔥 **Pós-Graduação em Medicina Hormonal Presencial**
Com **Glaycon Michels**, desenvolva um raciocínio clínico estruturado para conduzir os principais casos da medicina hormonal, de **TRT à saúde hormonal feminina**.
Você vai dominar:
✔️ Fisiologia endócrina e eixo HHG
✔️ Esteroidogênese, metabolismo e farmacocinética
✔️ Avaliação clínica, laboratorial e por imagem
✔️ Hipogonadismo masculino e TRT
✔️ Saúde hormonal feminina
✔️ Manejo clínico dentro dos limites éticos do CFM e da SBEM
🎓 **360 horas de formação**
📍 **Presencial — São Paulo/SP**
📅 **Início: 14 de novembro**
⏱️ **12 meses de duração**
👨‍⚕️ **Mentorias quinzenais + ambulatórios presenciais**
🏅 **Diploma reconhecido pelo MEC**
⚠️ **Vagas limitadas para acompanhamento próximo e prática em ambulatório.**
👉 **Garanta sua matrícula na Pós-Graduação em Medicina Hormonal.**"

### Títulos do link nos anúncios
- Pós-Graduação em Medicina Hormonal Aplicada à Prática Clínica – Plenitude Educação

### Landing Page: Headline & Promessa Central
"Pós-Graduação em Medicina Hormonal Presencial com Glaycon Michels — Domine o raciocínio clínico estruturado para conduzir com segurança os principais casos da medicina hormonal, de TRT a saúde hormonal feminina."

### Seções da Landing Page (títulos, na ordem)
- Glaycon Michels apresenta a Pós-Graduação em Medicina Hormonal
- O que você vai dominar?
- Como funciona a pós-graduação?
- Quem vai te ensinar?
- Tudo o que você recebe ao garantir sua matrícula:
- Perguntas Frequentes
- Preencha com as Informações

### Entregáveis / Formato (termos encontrados na LP)
- Mentoria
- PDF


========================================

---
id_oferta: 055
anunciante: "Verbo Carreiras Jurídicas"
url_destino: "https://api.whatsapp.com/send"
ad_library_url: "https://www.facebook.com/ads/library/?id=1098210225904481"
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
tipos_produto: "Mentoria / acompanhamento, Curso em videoaulas, Lei seca / legislação"
formatos_dos_anuncios: "vídeo (1)"
botoes: "Ver detalhes (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
id_oferta: 056
anunciante: "Weverton Reis"
url_destino: "https://www.facebook.com/100070415432523/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1069790249007641"
dias_ativo: 13
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
botoes: "Enviar mensagem pelo WhatsApp (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
📲 Entre em contato e agende sua visita."

### Títulos do link nos anúncios
- Custo-benefício no Bueno

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
dias_ativo: 13
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
dias_distintos_coletado: 1
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
anunciante: "Mentoria Tribunal em Foco"
url_destino: "https://www.facebook.com/61565895506139/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1776370023638757"
dias_ativo: 12
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Material em PDF / apostila / caderno"
formatos_dos_anuncios: "carrossel (1)"
botoes: "Enviar mensagem (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Ser aprovado no concurso do TRT exige mais do que força de vontade.
Exige clareza e método.
Com a Mentoria Tribunal em Foco, você se prepara para os cargos de Analista e Técnico Judiciário sabendo exatamente:
✔ o que estudar
✔ quando revisar
✔ como passar
Com a MTF, você não estuda no escuro.
👉 Envie MUDANÇA no direct e conheça o método que pode te levar à aprovação em 2026."

### Títulos do link nos anúncios
- Converse conosco

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 059
anunciante: "Malditafcc"
url_destino: "https://www.facebook.com/malditafcc/"
ad_library_url: "https://www.facebook.com/ads/library/?id=4717861935137850"
dias_ativo: 8
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
dias_distintos_coletado: 1
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
id_oferta: 060
anunciante: "Benito Soluções Judiciais"
url_destino: "https://wa.me/5519999192010"
ad_library_url: "https://www.facebook.com/ads/library/?id=1975498909788817"
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
tipos_produto: "Não identificado"
formatos_dos_anuncios: "imagem (1)"
botoes: "Enviar mensagem pelo WhatsApp (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Captura de Lead (WhatsApp / Grupo VIP)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 OPORTUNIDADE IMPERDÍVEL! 🚨
🏭 VENDA JUDICIAL – IMÓVEL INDUSTRIAL EM SÃO MANUEL/SP
📍 Distrito de Aparecida de São Manuel – Município e Comarca de São Manuel/SP
💰 LANCE INICIAL: R$ 2.500.000,00
✔ Possibilidade de parcelamento
✅ Área do terreno: 7.571,16 m²
✅ Área construída aproximada: 2.300 m²
✅ Galpão em alvenaria com aproximadamente 3.500 m²
📄 Matrícula nº 7.727
📌 Localização estratégica:
• Município com infraestrutura completa;
• Próximo a supermercados, bancos, universidades e amplo comércio;
• Fácil acesso às principais vias da região;
• Excelente logística para atividades industriais, comerciais e de armazenamento.
💼 Excelente oportunidade para investidores, empresas, indústrias ou para expansão de operações.
⏳ Não perca a oportunidade de adquirir um imóvel de grande porte, em localização estratégica e com excelente potencial de valorização por meio de venda judicial.
📄 Consulte o edital para mais informações.
📲 WhatsApp: (19) 99919-2010
🔗 https://wa.me/5519999192010
🌐 https://benitosolucoesjudiciais.com.br/
📌 Corretor Judicial habilitado junto ao TRT-15
📑 CRECI/SP nº 78.903-F"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

# Parte 2 — Ofertas adjacentes (72)

Apareceram nas buscas, mas não citam os termos do foco. Servem para comparar formatos e preços de outros nichos de concurso; algumas não são de concurso.

---
id_oferta: 061
anunciante: "Caminho da Perícia"
url_destino: "https://lp.vagasjustica.com.br/wpj/diario/engagro/c?utm_source=meta_%7B%7Bsite_source_name%7D%7D&utm_medium=cpc_%7B%7Bplacement%7D%7D&utm_campaign=%7B%7Bcampaign.id%7D%7D_%7B%7Bcampaign.name%7D%7D&utm_content=%7B%7Badset.id%7D%7D_%7B%7Badset.name%7D%7D&utm_term=%7B%7Bad.id%7D%7D_%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1742185740345778"
dias_ativo: 29
anuncios_coletados: 7
anuncios_ativos_estimados: 28
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (3), imagem (4)"
botoes: "sem botão (3), Saiba mais (4)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 PROCURA-SE ENGENHEIROS AGRÔNOMOS🚨
👉 Se você deseja trabalhar para a Justiça sem prestar concurso público, ter renda extra de casa e atuar com laudos dentro da sua área de formação,
essa é a sua grande oportunidade!
✅ Participe do AULÃO ON-LINE e GRATUITO, HOJE, às 20h, e descubra como ingressar nessa área e conquistar sua independência profissional.
Clique em "SAIBA MAIS" e garanta sua vaga!"

### Títulos do link nos anúncios
- Vagas para profissionais formados

### Landing Page: Headline & Promessa Central
[não capturada — status da LP: fetch_failed]

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 062
anunciante: "Caminho da Perícia"
url_destino: "https://lp.vagasjustica.com.br/wpj/diario/veterinario/c/?utm_source=meta_%7B%7Bsite_source_name%7D%7D&utm_medium=cpc_%7B%7Bplacement%7D%7D&utm_campaign=%7B%7Bcampaign.id%7D%7D_%7B%7Bcampaign.name%7D%7D&utm_content=%7B%7Badset.id%7D%7D_%7B%7Badset.name%7D%7D&utm_term=%7B%7Bad.id%7D%7D_%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1543166304518493"
dias_ativo: 29
anuncios_coletados: 6
anuncios_ativos_estimados: 24
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (4), vídeo (2)"
botoes: "Saiba mais (4), sem botão (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 PROCURA-SE VETERINÁRIOS🚨
👉 Se você deseja trabalhar para a Justiça sem prestar concurso público, ter renda extra de casa e atuar com laudos dentro da sua área de formação,
essa é a sua grande oportunidade!
✅ Participe do AULÃO ON-LINE e GRATUITO, HOJE, às 20h, e descubra como ingressar nessa área e conquistar sua independência profissional.
Clique em "SAIBA MAIS" e garanta sua vaga!"

### Títulos do link nos anúncios
- Vagas para profissionais formados

### Landing Page: Headline & Promessa Central
[não capturada — status da LP: fetch_failed]

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 063
anunciante: "Caminho da Perícia"
url_destino: "https://lp.vagasjustica.com.br/wpai/diario/engcivil/c?utm_source=meta_%7B%7Bsite_source_name%7D%7D&utm_medium=cpc_%7B%7Bplacement%7D%7D&utm_campaign=%7B%7Bcampaign.id%7D%7D_%7B%7Bcampaign.name%7D%7D&utm_content=%7B%7Badset.id%7D%7D_%7B%7Badset.name%7D%7D&utm_term=%7B%7Bad.id%7D%7D_%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1032013706481536"
dias_ativo: 29
anuncios_coletados: 5
anuncios_ativos_estimados: 20
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (2), imagem (3)"
botoes: "Saiba mais (5)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 PROCURA-SE ENGENHEIROS CIVIS🚨
👉 Se você deseja trabalhar para a Justiça sem prestar concurso público, ter renda extra de casa e atuar com laudos dentro da sua área de formação,
essa é a sua grande oportunidade!
✅ Participe do AULÃO ON-LINE e GRATUITO, HOJE, às 20h, e descubra como ingressar nessa área e conquistar sua independência profissional.
Clique em "SAIBA MAIS" e garanta sua vaga!"

### Títulos do link nos anúncios
- Vagas para profissionais formados

### Landing Page: Headline & Promessa Central
[não capturada — status da LP: fetch_failed]

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 064
anunciante: "EnfConcursos"
url_destino: "https://www.preparaenfermagem.com.br/cursos/curso-de-enfermagem-para-concursos/?utm_source=face_ads&utm_medium=%7B%7Bcampaign.name%7D%7D&utm_campaign=quente&utm_content=%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1600336774097728"
dias_ativo: 891
anuncios_coletados: 6
anuncios_ativos_estimados: 16
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Curso em videoaulas, Material em PDF / apostila / caderno, Mapas mentais / esquemas, Questões / simulados, Lei seca / legislação, Cronograma / plano de estudos"
formatos_dos_anuncios: "vídeo (6)"
botoes: "sem botão (6)"
precos_exibidos_na_lp: "12x de R$ 38,62 | R$ 397,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Área da Saúde"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Curso Completo com Mentoria e Aulas Diários para o Concurso da EBSERH
✅ Curso Completo das Básicas e Específicas
✅ Plano de Estudos Diário
✅ Aula de 100% dos Tópicos do Edital
✅ Mentorias Diárias com os Professores
✅ Simulados com Resultado e Avaliação Individual de Desempenho
✅ Mapas Mentais e Resumos Prontos
✅ 1.800 Questões Comentadas em Vídeo
✅ Acompanhamento com Tutor e Relatório de Desempenho
✅ Resolução Semanal de Provas Anteriores de Português, SUS, Legislação da EBSERH, Raciocínio Lógico e Específicas"

### Landing Page: Headline & Promessa Central
"Curso Completo de Enfermagem para Concursos - Prepara Enfermagem — IMPORTANTE! ANTES DE VOCÊ CONTINUAR, ASSISTA AO VÍDEO RÁPIDO ABAIXO"

### Seções da Landing Page (títulos, na ordem)
- IMPORTANTE! ANTES DE VOCÊ CONTINUAR, ASSISTA AO VÍDEO RÁPIDO ABAIXO
- CURSO COMPLETO DE ENFERMAGEM PARA CONCURSOS: Assinatura Ilimitada com tudo que você precisa pra passar
- Curso Completo de Enfermagem para Concursos + Plano de Estudos 365 Dias + Turbo 12 Semanas – Todas as Carreiras
- CURSO COMPLETO EM VÍDEO AULAS
- MENTORIAS DIÁRIAS COM OS PROFESSORES
- PLANO DE ESTUDOS ORGANIZADO E FOCADO PARA 365 DIAS DO ANO
- MAPAS MENTAIS DE TODO CONTEÚDO DE ENFERMAGEM
- RESUMO DO CONTEÚDO ESTUDADO
- PLANO DIÁRIO COM QR CODE LEVANDO PARA OS MAPAS MENTAIS E REVISÕES
- PREPARAÇÃO COMPLETO E FOCADA EM CONCURSOS DE ENFERMAGEM
- 100% do Conteúdo do Edital em disciplinas básicas e específicas em vídeo aulas
- Salas de Mentoria via Zoom Ao Vivo com os Professores
- Mapas Mentais prontos de todos conteúdo de enfermagem
- Resumos do Conteúdo de Enfermagem
- Listas de Exercícios separadas por assunto
- Aprenda Português e Interpretação de Texto
- Análise de Desempenho Individual da Evolução com Questões
- 52 Simulados
- Assista as aulas de onde estiver pelo celular, tablet ou computador
- Confira alguns dos principais concursos que estão inclusos em nossa plataforma.
- MENTORIA EXCLUSIVA COM OS MELHORES ESPECIALISTAS DA ÁREA
- PREPARE-SE PARA DAR O PRÓXIMO PASSO
- PRA QUEM É A TURMA PREMIUM?
- Enfermeiro ou Técnico de Enfermagem
- Recém formados que vão fazer o 1º concurso
- Quem já tentou estudar sozinho
- CONHEÇA O CONTEÚDO DOS MÓDULOS ESPECÍFICOS DE ENFERMAGEM PARA CONCURSOS
- A ESTRATÉGIA DE PREPARAÇÃO QUE APROVOU MAIS DE 10.000 PROFISSIONAIS DE ENFERMAGEM
- TUDO QUE VOCÊ VAI RECEBER
- GARANTIA INCONDICIONAL DE 7 DIAS

### Entregáveis / Formato (termos encontrados na LP)
- Discursiva / redação
- Mapas mentais
- Mentoria
- Planner
- Questões comentadas
- Resumos
- Simulados
- Videoaulas


========================================

---
id_oferta: 065
anunciante: "Caminho da Perícia"
url_destino: "http://lp.vagasjustica.com.br/wpg/diario/pedagogo/c/?utm_source=meta_%7B%7Bsite_source_name%7D%7D&utm_medium=cpc_%7B%7Bplacement%7D%7D&utm_campaign=%7B%7Bcampaign.id%7D%7D_%7B%7Bcampaign.name%7D%7D&utm_content=%7B%7Badset.id%7D%7D_%7B%7Badset.name%7D%7D&utm_term=%7B%7Bad.id%7D%7D_%7B%7Bad.name%7D%7Dl"
ad_library_url: "https://www.facebook.com/ads/library/?id=2116002109306739"
dias_ativo: 29
anuncios_coletados: 3
anuncios_ativos_estimados: 12
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (1), vídeo (2)"
botoes: "Saiba mais (3)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 PROCURA-SE PEDAGOGOS🚨
👉 Se você deseja trabalhar para a Justiça sem prestar concurso público, ter renda extra de casa e atuar com laudos dentro da sua área de formação,
essa é a sua grande oportunidade!
✅ Participe do AULÃO ON-LINE e GRATUITO, HOJE, às 20h, e descubra como ingressar nessa área e conquistar sua independência profissional.
Clique em "SAIBA MAIS" e garanta sua vaga!"

### Títulos do link nos anúncios
- Vagas para profissionais formados

### Landing Page: Headline & Promessa Central
[não capturada — status da LP: fetch_failed]

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 066
anunciante: "Caminho da Perícia"
url_destino: "https://lp.vagasjustica.com.br/wpg/diario/advogado/c/?utm_source=meta_%7B%7Bsite_source_name%7D%7D&utm_medium=cpc_%7B%7Bplacement%7D%7D&utm_campaign=%7B%7Bcampaign.id%7D%7D_%7B%7Bcampaign.name%7D%7D&utm_content=%7B%7Badset.id%7D%7D_%7B%7Badset.name%7D%7D&utm_term=%7B%7Bad.id%7D%7D_%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1095659739820201"
dias_ativo: 29
anuncios_coletados: 3
anuncios_ativos_estimados: 12
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (2), vídeo (1)"
botoes: "Saiba mais (3)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Carreiras Jurídicas / OAB"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 PROCURA-SE ADVOGADOS! 🚨
👉 Se você deseja trabalhar para a Justiça sem prestar concurso público, ter renda extra de casa e atuar com laudos dentro da sua área de formação,
essa é a sua grande oportunidade!
✅ Participe do AULÃO ON-LINE e GRATUITO, HOJE, às 20h, e descubra como ingressar nessa área e conquistar sua independência profissional.
Clique em "SAIBA MAIS" e garanta sua vaga!"

### Títulos do link nos anúncios
- Vagas para profissionais formados

### Landing Page: Headline & Promessa Central
[não capturada — status da LP: fetch_failed]

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 067
anunciante: "Pratique Concursos"
url_destino: "https://ti.pratiqueconcursos.com.br/fcti/tce-go.html"
ad_library_url: "https://www.facebook.com/ads/library/?id=1427104632716607"
dias_ativo: 8
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
dias_distintos_coletado: 1
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
id_oferta: 068
anunciante: "Metodo.Gafanhoto"
url_destino: "https://metodogafanhoto.com/quizz117"
ad_library_url: "https://www.facebook.com/ads/library/?id=1097069556027495"
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
tipos_produto: "Não identificado"
formatos_dos_anuncios: "vídeo (2)"
botoes: "sem botão (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
id_oferta: 069
anunciante: "Professor Hansk"
url_destino: "https://hanskcarvalho.com/melhor-que-blackfriday-pago/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1335871585123913"
dias_ativo: 8
anuncios_coletados: 2
anuncios_ativos_estimados: 6
anuncios_com_baixo_volume_de_impressoes: 2
sinal_tracao: "fraco"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Discursiva / redação, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (2)"
botoes: "sem botão (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
id_oferta: 070
anunciante: "Matheus Santos - Eu concursado"
url_destino: "https://seraprovado.com/mentoria-matheussantos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1059387566661056"
dias_ativo: 71
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
dias_distintos_coletado: 1
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
id_oferta: 071
anunciante: "Ser Aprovado"
url_destino: "https://www.facebook.com/seraprovadoconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2504298076719444"
dias_ativo: 9
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
id_oferta: 072
anunciante: "Estratégia Concursos"
url_destino: "https://www.facebook.com/EstrategiaConcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=977003848724493"
dias_ativo: 83
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
dias_distintos_coletado: 1
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
id_oferta: 073
anunciante: "Clube do Perito"
url_destino: "https://lp.vagasjustica.com.br/wpj/diario/fisioterapeuta/c/?utm_source=meta_%7B%7Bsite_source_name%7D%7D&utm_medium=cpc_%7B%7Bplacement%7D%7D&utm_campaign=%7B%7Bcampaign.id%7D%7D_%7B%7Bcampaign.name%7D%7D&utm_content=%7B%7Badset.id%7D%7D_%7B%7Badset.name%7D%7D&utm_term=%7B%7Bad.id%7D%7D_%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1404455104491303"
dias_ativo: 14
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
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
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
[não capturada — status da LP: fetch_failed]

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 074
anunciante: "Clube do Perito"
url_destino: "https://lp.vagasjustica.com.br/wpj/diario/psicologo/c/?utm_source=meta_%7B%7Bsite_source_name%7D%7D&utm_medium=cpc_%7B%7Bplacement%7D%7D&utm_campaign=%7B%7Bcampaign.id%7D%7D_%7B%7Bcampaign.name%7D%7D&utm_content=%7B%7Badset.id%7D%7D_%7B%7Badset.name%7D%7D&utm_term=%7B%7Bad.id%7D%7D_%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1617178199956947"
dias_ativo: 13
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
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 PROCURA-SE PSICÓLOGOS🚨
👉 Se você deseja trabalhar para a Justiça sem prestar concurso público, ter renda extra de casa e atuar com laudos dentro da sua área de formação,
essa é a sua grande oportunidade!
✅ Participe do AULÃO ON-LINE e GRATUITO, HOJE, às 20h, e descubra como ingressar nessa área e conquistar sua independência profissional.
Clique em "SAIBA MAIS" e garanta sua vaga!"

### Landing Page: Headline & Promessa Central
[não capturada — status da LP: fetch_failed]

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 075
anunciante: "Advogado de concurso"
url_destino: "https://olivaesouza.com.br/tce-rs-discursiva/"
ad_library_url: "https://www.facebook.com/ads/library/?id=861868490346562"
dias_ativo: 9
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
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Fiscal e Controle"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 Fez a prova discursiva do TCE-RS?
📋 A nota recebida não conta toda a história. É preciso entender como a banca chegou até ela.
🔎 O espelho de correção, os critérios previstos no edital e a pontuação atribuída em cada item precisam ser analisados.
⚠️ Pontos que não foram considerados, critérios aplicados de forma inadequada ou inconsistências na correção podem justificar um questionamento.
⚖️ Faça uma análise técnica da sua prova discursiva e entenda se existem fundamentos para contestar a correção."

### Landing Page: Headline & Promessa Central
[não capturada — status da LP: fetch_failed]

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

## Demais adjacentes (resumo)

| id | Anunciante | Dias | Anúncios | Tração | Ticket (checkout) | Destino |
|---|---|---|---|---|---|---|
| 076 | Pódio Tribunais | 197 | 3 | forte | Não confirmado | https://cronosconcursos.com.br/tribunais/?utm_source=meta&utm_medium=ig-ads&utm_ |
| 077 | Caderno Mapeado | 57 | 3 | médio | Não confirmado | https://cadernomapeado.com.br/tce-ma-cmlm/?src=&utm_source=facebook-ads&utm_medi |
| 078 | Alan Matos | 50 | 3 | médio | Não confirmado | https://concursotcdf.editorainovedigital.com/ |
| 079 | Joy Braga Concursos | 12 | 3 | médio | Não confirmado | https://detoxconcursos.com.br/tribunais/?src=a2d330ebaa55430aaa643cc71bc84863&ut |
| 080 | Victor Ribeiro | 9 | 3 | médio | Não confirmado | https://fureafila.com.br/comomemorizartudo/ |
| 081 | Gaby no Tribunal | 9 | 3 | médio | Não confirmado | https://gabynotribunal.com.br/cve/ |
| 082 | Concursos Ceisc | 190 | 2 | médio | Não confirmado | https://ceisc.com.br/cursos/2067-concurso-tj-sp-club-oficial-de-justica?utm_sour |
| 083 | Pódio Tribunais | 170 | 2 | médio | Não confirmado | https://api.whatsapp.com/send |
| 084 | Felipe Sgarbossa Advocacia Criminal | 165 | 2 | médio | Não confirmado | https://www.facebook.com/felipesgarbossa/ |
| 085 | Prof.carlosgoncalves | 120 | 2 | médio | Não confirmado | https://typebot.co/plataformaanalistadetribunais |
| 086 | Tjteiros | 96 | 2 | médio | Não confirmado | https://www.facebook.com/61582438800580/ |
| 087 | Rafael Amaral Adv | 93 | 2 | médio | Não confirmado | https://www.facebook.com/cleytonrafaelamaral/ |
| 088 | Central de Concursos | 85 | 2 | médio | Não confirmado | https://centraldeconcursos.com.br/concursos/concurso-tj-sp-escrevente?utm_source |
| 089 | Ludy Sena | 82 | 2 | médio | Não confirmado | https://www.facebook.com/ludysena.perita/ |
| 090 | LH no pódio | 76 | 2 | médio | Não confirmado | https://typebot.co/mentoria-zeroaopodio |
| 091 | Eccos Cursos | 75 | 2 | médio | Não confirmado | https://eccosedu.com/laser-transdermico/ |
| 092 | Venâncio & Delgado - Advogados | 57 | 2 | médio | Não confirmado | https://api.whatsapp.com/send |
| 093 | Venâncio & Delgado - Advogados | 57 | 2 | médio | Não confirmado | https://www.facebook.com/venancioedelgadoadvogados/ |
| 094 | Milena Correia Advocacia | 22 | 2 | médio | Não confirmado | https://api.whatsapp.com/send |
| 095 | Academia do Perito | 21 | 2 | médio | R$ 497,00 | https://lp.academiadoperito.com/peju-dor?utm_source=facebook&utm_medium=paid&utm |
| 096 | Memorização Bruno Campos Concursos | 20 | 2 | médio | Não confirmado | https://www.facebook.com/100088833677510/ |
| 097 | Estudo e Memorização | 16 | 2 | médio | Não confirmado | https://estudomemorizacao.com.br/pv-video-v2/ |
| 098 | Sensei da Aprovação - Concursos Públicos | 12 | 2 | médio | Não confirmado | https://senseidaaprovacao.com.br/projetoprefeituracuritiba |
| 099 | EG Raiz - I.A | 10 | 2 | médio | Não confirmado | https://concursa-paginas.vercel.app/live-privada/ |
| 100 | minhajornadadeconcurseira com Decorando a Lei Seca Cursos Para Concursos E OAB | 10 | 2 | médio | R$ 499,99 | https://www.decorandoaleiseca.com.br/assinatura-ilimitada |
| 101 | Mapas da Lulu Concurseira com Laura Amorim | 9 | 2 | médio | R$ 597,90 | https://paginas.mapasdalulu.com.br/lp-pacote/ |
| 102 | Projeto Caveira | 324 | 1 | médio | Não confirmado | https://www.facebook.com/projetocaveiraprf/ |
| 103 | Concursos Ceisc | 190 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2070-concurso-tj-ba-analista-judiciario-area-judicia |
| 104 | Gaby no Tribunal | 174 | 1 | médio | Não confirmado | https://www.facebook.com/100090566482087/ |
| 105 | Discursiva na Prática | 125 | 1 | médio | R$ 1.489,00 | https://discursivanapratica.com.br/assinaturacontrole/?utm_source=facebook&utm_m |
| 106 | Douglas Prado - Servidor 30k | 102 | 1 | médio | Não confirmado | https://odouglasprado.com.br/plano-servidor-30k/ |
| 107 | Fauth e Freitas Sociedade de Advogados com Adriane Fauth | 91 | 1 | médio | Não confirmado | https://www.facebook.com/61573224123970/ |
| 108 | mamae_concurseira6 com Decorando a Lei Seca Cursos Para Concursos E OAB | 84 | 1 | médio | Não confirmado | https://www.decorandoaleiseca.com.br/ |
| 109 | Atleta dos Concursos | 82 | 1 | médio | Não confirmado | https://atletadosconcursos.com.br/kit-aprovacao-enam/?sck=facebook%7Cads%7Cconve |
| 110 | Mege | 65 | 1 | médio | Não confirmado | https://concurcity.mege.com.br/explorar |
| 111 | Themas Cartórios | 63 | 1 | médio | Não confirmado | http://www.themas.com.br/ |
| 112 | Concurseiro Fora da Caixa | 56 | 1 | médio | Não confirmado | https://concurseiroforadacaixa.com.br/collections/todos-os-materiais |
| 113 | Professora Amanda Aires | 53 | 1 | médio | Não confirmado | https://www.amandaaires.com.br/curso/%5B2026%5D-economia-para-o-tcu/345 |
| 114 | Rô Santtana - OAB | 50 | 1 | médio | Não confirmado | https://rosanttana.com.br/captacao/lp-discursiva-oab.html |
| 115 | Concursos Ceisc | 49 | 1 | médio | Não confirmado | https://www.sympla.com.br/produtor/ceisc |
| 116 | IPOG Salvador | 48 | 1 | médio | Não confirmado | https://ipog.edu.br/cursos/pos-graduacao/psicologia-juridica-com-enfase-em-peric |
| 117 | Jus Expert | 25 | 1 | médio | R$ 997,00 | https://pages.jusexpert.com/vsl-grafotecnica-principal |
| 118 | padadvocacia | 22 | 1 | médio | Não confirmado | https://www.instagram.com/_u/padadvocacia |
| 119 | Prof. Herbert Almeida | 22 | 1 | médio | Não confirmado | https://herbertalmeida.com.br/mentoria-cgu/ |
| 120 | Marco Cursos Preparatórios | 12 | 1 | médio | Não confirmado | https://www.facebook.com/marcocursos/ |
| 121 | danielvieira_2 | 12 | 1 | médio | Não confirmado | https://hotmart.com/pt-br/marketplace/produtos/hagsxd-o-jogo-da-aprovacao-z99mi/ |
| 122 | Aprovação na prova | 12 | 1 | médio | Não confirmado | https://www.facebook.com/61591237817325/ |
| 123 | Memoriza-aí Concursos | 11 | 1 | médio | Não confirmado | https://memorizaai.com.br/unioeste-pr-revisao-vespera/?src=&utm_source=facebook- |
| 124 | Treine Subjetivas | 10 | 1 | médio | Não confirmado | https://treinesubjetivas.com.br/ |
| 125 | Mentoria Próximo Nível | 10 | 1 | médio | Não confirmado | https://www.facebook.com/61550731887681/ |
| 126 | Dr. Thiago Braga | 10 | 1 | médio | Não confirmado | https://www.facebook.com/dr.thiagobraga/ |
| 127 | KAAIF Concursos | 9 | 1 | médio | Não confirmado | https://chronosdock.com/form/acompanhamento-individual |
| 128 | UniEVANGÉLICA | 9 | 1 | médio | Não confirmado | https://selecao.unievangelica.edu.br/direito |
| 129 | Pedro Auar Advocacia | 8 | 1 | médio | Não confirmado | https://www.facebook.com/pedroauar/ |
| 130 | Paulo Afonso Advocacia | 8 | 1 | fraco | Não confirmado | https://www.facebook.com/61582851535500/ |
| 131 | Gtcar | 8 | 1 | médio | Não confirmado | https://www.facebook.com/61556284626069/ |
| 132 | Pratique Concursos | 8 | 1 | médio | Não confirmado | https://www.facebook.com/61551019732654/ |

# Apêndice — Descartadas por não citarem concurso (75)

Vieram nas buscas (ex.: escritórios que citam o TRF como tribunal), mas o texto não tem nenhum termo de concurso. Confira se algo relevante caiu aqui por engano.

| Anunciante | Dias | Destino |
|---|---|---|
| Reviva | 28 | https://renuva.com.br/pages/drenagem-linfatica |
| SERV FONE | 98 | https://www.facebook.com/servfone.servfone/ |
| Magnali Health | 13 | https://magnali.com/pages/charlesanderson |
| Rita Bervig | 177 | https://www.facebook.com/100091834883862/ |
| Fernanda Diniz | 28 | https://renuva.com.br/pages/drenagem-linfatica |
| Previdas Saúde | 9 | https://provamedica3.previdas.com.br/?src=&utm_source=meta&utm_medium=%7B%7Badse |
| Danielle Bartoly | 169 | https://www.facebook.com/61577922862090/ |
| Precatorial | 53 | http://fb.me/ |
| Dr. Paulo Leandro - Cirurgião Ortopedista | 12 | https://www.facebook.com/61590189522867/ |
| Carlos Klein - Personal | 19 | https://oficialbarrigazero.protocolocarlos.com.br/quizz |
| Dra. Gabriela Madeira | 9 | https://api.whatsapp.com/send |
| ShopRootvana | 9 | https://tryrootvana.com/pages/listicle-2 |
| Editora Mizuno | 251 | https://www.editoramizuno.com.br/ |
| Ato psicologia psicoterapias psicodrama e desenvolvimento humano | 141 | https://api.whatsapp.com/send |
| Dr Bruno Guerra | 125 | https://www.facebook.com/61566645860434/ |
| Hematix - Hematite Bracelet | 124 | https://myhematix.com/products/hematix-strength-band |
| ShopVantique | 57 | https://shopvantique.com/products/vantique-nad-supplement-for-men |
| Andrew Martin - Health & Performance Advisor | 56 | https://assess.secondprime.io/ |
| Heraclio Cunha | 50 | https://peritoem7dias.com.br/ |
| Rafael Amaral Adv | 28 | https://api.whatsapp.com/send |
| ShopRootvana | 24 | https://tryrootvana.com/products/rootvana-l-carnitine-4000mg-liquid-spanish?utm_ |
| Central Sul de Leilões | 17 | https://www.centralsuldeleiloes.com.br/ |
| Verbo Carreiras Jurídicas | 14 | https://chat.whatsapp.com/Bsvp30MtbOTI4HDJuoMz89?mode=hqrt2 |
| Sublime Medicina Integrada | 13 | https://api.whatsapp.com/send |
| Justa Pena BR | 11 | https://conteudo.justapenabr.com.br/destravando-seeu/ |
| Doctora Karito | 9 | https://trt.colorpack.online/ |
| Iridium Labs | 9 | https://www.iridiumlabs.com.br/products/zeus-extreme-pre-hormonal-60-comps |
| Bruto Brasil | 127 | https://www.youtube.com/watch?v=S9fODqC2kkw&feature=youtu.be |
| Douglas Prado - Servidor 30k com Servidores High Level | 123 | https://www.facebook.com/professorlucrativo/ |
| Dental Speed | 117 | https://www.dentalspeed.com/carregador-universal-fotopolimerizador-elipar-deepcu |
| Jerônimo E-Lance | 109 | https://www.facebook.com/jeronimoelance/ |
| TSTemdia | 108 | https://www.facebook.com/61581193663516/ |
| EBM Goiás | 95 | http://fb.me/ |
| Fibra Pará | 93 | https://www.facebook.com/fibrapara/ |
| Instituto Médico da Dor - IMD | 84 | https://www.facebook.com/61550152706355/ |
| Madervillas Madeireira . Lauro de Freitas | 75 | https://www.facebook.com/61577737911934/ |
| VCA Construtora e Incorporadora | 71 | http://fb.me/ |
| Prompt8 AI | 65 | https://jusquant.ai/?utm_source=meta&utm_medium=paid_social&utm_campaign=trab_up |
| Servita Clinic | 64 | https://www.facebook.com/61582841670718/ |
| Viégas Filho | 56 | https://www.facebook.com/100094050184913/ |
| thainara.assistentesocial | 54 | https://www.instagram.com/_u/thainara.assistentesocial |
| Gabriela Franco | 51 | https://www.facebook.com/61575028750782/ |
| AnotherVoid | 51 | https://anothervoid.co/products/liquid-l-carnitine-4000mg?variant=49141411283179 |
| Inovajur Capacitação Jurídica e IA | 50 | https://inovajur.com/nova-pratica-vsl/?utm_source=Facebook_ads&utm_medium=%7B%7B |
| Avante | 50 | https://www.facebook.com/61572155530930/ |
| Go Kursos | 49 | https://www.gokursos.com/go-oab---direito-penal---2%C2%AA-fase-30553/p |
| Dra Yanka Guirado / Fisioterapeuta especializada na saúde da mulher e bebê | 33 | https://www.facebook.com/Dra-Yanka-Guirado-Fisioterapeuta-especializada-na-sa%C3 |
| Velyon Energia Solar | 30 | https://api.whatsapp.com/send |
| Keylon Lucarelli - Nutrologia e Emagrecimento Saudável | 26 | https://www.facebook.com/100082746462251/ |
| ShopRootvana | 24 | https://tryrootvana.com/pages/listicle-1 |
| Muniz Auto Center Vitória da Conquista | 21 | https://www.facebook.com/munizvitoriadaconquista/ |
| Dr. Murilo M. Murata | 21 | https://www.facebook.com/61554937077888/ |
| Cellics Health | 20 | https://cellics.co/pages/appledroppers-2 |
| M3 Parts Kawasaki | 20 | https://www.facebook.com/m3PartsKawasaki/ |
| Experience True Nutra | 16 | https://truenutra.com/products/fb-en-us-mc001 |
| Eletricista a preço popular | 16 | https://wa.me/message/VUCK56R4WH35K1 |
| Alfa Viking | 15 | https://alfaviking.com.br/libi/ |
| Hospital Adventista de Belém | 15 | https://www.facebook.com/hospitalbelem/ |
| Morais Amaral Arquitetura | 14 | https://www.moraisamaral.arq.br/ |
| Start Veículos - Suzano/Sp | 14 | https://www.startveiculo.com.br/ |
| Vanguarda Visual Law | 13 | https://vanguardavisuallaw.com.br/kit-advocacia-trabalhista |
| Hormofy | 13 | https://hormofy.com/reposicao-hormonal/ |
| Benvindoadv Professor | 12 | https://www.facebook.com/100095299025661/ |
| Vinco Leilões | 12 | https://www.vinconews.com.br/Leiloes/2026/TRT2-SP |
| Congresso Uninassau | 12 | https://vendyno.goexplosion.com/checkout/vii-congresso-piauiense-de-direito |
| naylinnunes | 11 | https://www.instagram.com/_u/naylinnunes |
| True Nutra Plus | 11 | https://truenutra.com/products/fb-en-lc001 |
| Leandro Magalhães | 11 | https://www.facebook.com/AnalyticsBR/ |
| Zambroni Advogados | 9 | https://www.facebook.com/zambroniaraujoadv/ |
| Vinícius Rocha | 9 | https://www.facebook.com/ViniciusRocha.casas.terrenos.chacaras.fazendas/ |
| Congresso TEA RP com gialbuquerquesp | 9 | https://payfast.greenn.com.br/sdq5zr4 |
| Felipe Almeida | 9 | https://www.facebook.com/felipealmeidaseudividendo/ |
| Aerocar Veículos | 8 | https://www.facebook.com/aerocarveiculos/ |
| Mundo das Capas Guaratinguetá | 8 | https://www.facebook.com/mundodascapasguara/ |
| Clinicaespacoter Connected Page | 8 | https://api.whatsapp.com/send |
