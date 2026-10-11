# Dossiê ConcursoRadar — Técnico Judiciário — TRT (11/10/2026)

## Métricas da Rodada
- **Buscas na Meta Ad Library:** `concurso TRT`, `tribunal regional do trabalho`, `justiça do trabalho concurso`, `técnico judiciário`, `TRT técnico judiciário`, `TRT2`, `TRT15`, `TRT1`, `TRT4`, `TRT3`, `concurso tribunal`
- **Filtro:** anúncios ativos no Brasil, no ar há 7+ dias (coleta ampla para achar padrões; a longevidade é analisada nas tabelas)
- **Ofertas do nicho:** 151 (de 408 anúncios; agrupadas por anunciante + página de destino)
- **Descartadas por não citarem concurso:** 170 (listadas no fim para auditoria)
- **Ofertas de foco direto:** 75 | adjacentes: 76
- **Sinal de tração:** 11 forte, 1 fraco, 139 médio
- **Landing pages lidas:** 99 de 151
- **Ticket confirmado no checkout:** 24 de 26 ofertas com checkout detectado (92%)
- **Tempo de processamento:** 1033 segundos

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

Base: **408 anúncios de 115 anunciantes**; 164 estão no ar há 45+ dias (veteranos); mediana de 19 dias.

Como ler: **Anunciantes** = quantos produtores distintos usam (popularidade). **Veteranos** = quantos desses anúncios estão no ar há 45+ dias, e **% dos veteranos** = a fatia da categoria entre todos os veteranos. Se a fatia entre veteranos é maior que a fatia geral (% anúncios), a categoria aparece mais entre os que duram. Categoria com 1 ou 2 anunciantes é só um caso isolado.

A coleta junta duas amostras por busca (anúncios com 7+ dias e anúncios com 45+ dias), então a proporção de veteranos no total não é uma taxa de sobrevivência.

## Formato do criativo

Vídeo, imagem única ou carrossel.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| vídeo | 63 | 55% | 174 | 43% | 39 | 87 | 53% |
| imagem | 47 | 41% | 163 | 40% | 14 | 47 | 29% |
| carrossel | 34 | 30% | 71 | 17% | 32 | 30 | 18% |

## Proporção do criativo

Vertical (4:5 ou 9:16), quadrada (1:1) ou horizontal.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| vídeo vertical | 59 | 51% | 163 | 40% | 33 | 79 | 48% |
| imagem vertical | 40 | 35% | 146 | 36% | 14 | 36 | 22% |
| carrossel vertical | 26 | 23% | 49 | 12% | 33 | 24 | 15% |
| carrossel quadrada | 9 | 8% | 13 | 3% | 33 | 6 | 4% |
| imagem quadrada | 8 | 7% | 16 | 4% | 57 | 11 | 7% |
| vídeo quadrada | 4 | 3% | 5 | 1% | 62 | 3 | 2% |
| vídeo horizontal | 2 | 2% | 6 | 1% | 709 | 5 | 3% |
| carrossel horizontal | 1 | 1% | 9 | 2% | 11 | 0 | 0% |
| imagem horizontal | 1 | 1% | 1 | 0% | 11 | 0 | 0% |

## Duração dos vídeos

Só anúncios em vídeo.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| 31s a 1min | 28 | 44% | 78 | 45% | 27 | 38 | 44% |
| 1 a 2min | 25 | 40% | 46 | 26% | 46 | 26 | 30% |
| Até 30s | 16 | 25% | 31 | 18% | 13 | 9 | 10% |
| Mais de 2min | 11 | 17% | 19 | 11% | 131 | 14 | 16% |

## Botão (CTA)

Rótulo do botão exibido no anúncio.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| sem botão | 50 | 43% | 142 | 35% | 13 | 52 | 32% |
| Saiba mais | 46 | 40% | 143 | 35% | 33 | 64 | 39% |
| Ver detalhes | 20 | 17% | 48 | 12% | 33 | 22 | 13% |
| Visitar perfil do Instagram | 20 | 17% | 33 | 8% | 48 | 19 | 12% |
| Enviar mensagem pelo WhatsApp | 9 | 8% | 21 | 5% | 11 | 1 | 1% |
| Comprar agora | 7 | 6% | 13 | 3% | 15 | 4 | 2% |
| Solicitar agora | 2 | 2% | 3 | 1% | 8 | 1 | 1% |
| Cadastre-se | 2 | 2% | 3 | 1% | 17 | 0 | 0% |
| Baixar | 1 | 1% | 1 | 0% | 8 | 0 | 0% |
| Inscreva-se | 1 | 1% | 1 | 0% | 90 | 1 | 1% |

## Destino do clique

Para onde o anúncio leva.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Página própria (LP / site) | 74 | 64% | 293 | 72% | 15 | 112 | 68% |
| Página / formulário no Facebook | 45 | 39% | 104 | 25% | 22 | 45 | 27% |
| WhatsApp | 4 | 3% | 7 | 2% | 61 | 4 | 2% |
| Perfil do Instagram | 2 | 2% | 2 | 0% | 56 | 2 | 1% |
| Checkout direto | 2 | 2% | 2 | 0% | 31 | 1 | 1% |

## Tamanho da copy

Texto principal do anúncio.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Média (200 a 600) | 61 | 53% | 179 | 44% | 48 | 102 | 62% |
| Longa (mais de 600) | 55 | 48% | 166 | 41% | 12 | 55 | 34% |
| Curta (até 200 caracteres) | 17 | 15% | 62 | 15% | 14 | 6 | 4% |
| Sem texto | 1 | 1% | 1 | 0% | 46 | 1 | 1% |

## Tipo de gancho (1ª linha da copy)

Classificação por palavras-chave; um gancho pode cair em mais de um tipo.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos | Exemplo |
|---|---|---|---|---|---|---|---|---|
| Outro | 57 | 50% | 145 | 36% | 33 | 68 | 41% | 🔥 A sua aprovação em Concursos Públicos não depende dos Materiais! Depende de direcionamento correto. — Gustavo Dias |
| Notícia de concurso / edital | 37 | 32% | 117 | 29% | 11 | 28 | 17% | Tem edital que passa. E tem edital que muda a sua vida. 💙 — MEQ Concursos |
| Pergunta | 24 | 21% | 48 | 12% | 61 | 33 | 20% | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? — Isaque Concursos |
| Número / lista | 16 | 14% | 31 | 8% | 14 | 6 | 4% | A Ana Flávia chegou até mim faltando apenas 15 dias para o concurso do Tribunal de Justiça do Rio de Janeiro. — Prof. Ronaldo Santos |
| Dor / erro do candidato | 14 | 12% | 24 | 6% | 14 | 9 | 5% | Qual desses apps & sites você ainda não conhecia? Algum usa no seu dia a dia? Ah, se tiver uma outra indicação pode deixar nos comentários, amo descobrir novos  — Gaby no Tribunal |
| Salário / estabilidade | 13 | 11% | 34 | 8% | 12 | 8 | 5% | O TJ-SP Escrevente é uma grande oportunidade para quem busca estabilidade e carreira pública com nível médio. — Central de Concursos |
| Oferta / desconto / urgência | 12 | 10% | 22 | 5% | 51 | 17 | 10% | "📚🆓 Curso Grátis TJ-SP 2026 - Escrevente Técnico Judiciário! 🆓📚 — Nova Concursos |
| Prova social / autoridade | 10 | 9% | 23 | 6% | 61 | 17 | 10% | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? — Isaque Concursos |
| Chamada direta ao público | 9 | 8% | 20 | 5% | 89 | 15 | 9% | O TJ-SP Escrevente é uma grande oportunidade para quem busca estabilidade e carreira pública com nível médio. — Central de Concursos |
| Promessa de método | 8 | 7% | 23 | 6% | 61 | 22 | 13% | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? — Isaque Concursos |
| Contraintuitivo / inimigo comum | 4 | 3% | 6 | 1% | 14 | 2 | 1% | Três anos no cursinho jurídico. Sete apostilões de Direito. E fiquei em cadastro de reserva no primeiro TRT que eu prestei. — Gustavo Nogueira - Aprovação Ágil |

## Elementos da copy

Recursos presentes no texto; não são excludentes.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos |
|---|---|---|---|---|---|---|---|
| Usa emojis | 74 | 64% | 222 | 54% | 33 | 99 | 60% |
| Cita valor em R$ | 36 | 31% | 101 | 25% | 11 | 17 | 10% |
| Lista com marcadores (✔, ✅, •) | 33 | 29% | 110 | 27% | 33 | 44 | 27% |
| Hashtags | 25 | 22% | 50 | 12% | 42 | 25 | 15% |
| Gancho em CAIXA ALTA | 12 | 10% | 38 | 9% | 11 | 3 | 2% |
| Link ou 'link na bio' no texto | 12 | 10% | 27 | 7% | 11 | 10 | 6% |
| Cita bônus | 4 | 3% | 9 | 2% | 48 | 5 | 3% |
| Cita garantia | 3 | 3% | 4 | 1% | 128 | 3 | 2% |

## Sinais de público (ICP) citados na copy

Quem o anúncio diz atender, por palavras-chave. Indica a quem o mercado fala, não quem compra.

| Categoria | Anunciantes | % anunciantes | Anúncios | % anúncios | Mediana de dias | Veteranos | % dos veteranos | Exemplo |
|---|---|---|---|---|---|---|---|---|
| Motivado por salário / estabilidade | 40 | 35% | 121 | 30% | 11 | 37 | 23% | 💰 Concursos com salários de até R$20.000 estão ao seu alcance — mas você precisa do caminho certo. — Gustavo Dias |
| Esquece o que estuda / revisão | 27 | 23% | 64 | 16% | 17 | 19 | 12% | 📚 Quem quer disputar uma vaga de verdade precisa construir base, revisar com método, acompanhar o próprio desempenho e estudar com direção. — Concurseiro aos 40 |
| Trabalha / tem pouco tempo | 21 | 18% | 91 | 22% | 20 | 31 | 19% | Durante essa jornada de estudos, eu estudava de 2h a 3h por dia, já que estudava e trabalhava como CLT. — Isaque Concursos |
| Pré-edital / sair na frente | 17 | 15% | 46 | 11% | 13 | 18 | 11% | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. — Tjteiros |
| Reta final / pós-edital | 17 | 15% | 40 | 10% | 9 | 9 | 5% | Você não precisa enfrentar essa reta final sozinho(a). No AprovaMEQ TRT-8 você tem: — MEQ Concursos |
| Começando do zero | 12 | 10% | 45 | 11% | 16 | 17 | 10% | • Esteja começando os estudos agora; — Isaque Concursos |
| Dificuldade em discursiva / redação | 12 | 10% | 29 | 7% | 11 | 8 | 5% | 📅 Cronogramas de 3h ou 5h por dia para Analista (AJAJ) e Técnico (TJAA)� 📘 PDMEQuinhos, VadeMEQ e Regimento Interno� ✍🏼 3 simulados completos com estudo de caso — MEQ Concursos |
| Perdido no excesso de conteúdo | 11 | 10% | 27 | 7% | 11 | 8 | 5% | Se você tá perdido sem saber como começar ou já estuda mas sente que não evolui, está correndo um sério risco de ficar anos sem a sua aprovação. — Gustavo Dias |
| Nível superior / Direito | 11 | 10% | 22 | 5% | 9 | 5 | 3% | Trata-se de uma oportunidade de nível superior com MUITAS vagas, e uma remuneração inicial muito atrativa. — Concursos Ceisc |
| Nível médio | 9 | 8% | 27 | 7% | 61 | 23 | 14% | Para você ter uma ideia, eu só me formei no ensino médio por meio do ENCCEJA, já que tinha repetido em todas as matérias. — Isaque Concursos |
| Mãe / família | 6 | 5% | 19 | 5% | 61 | 13 | 8% | Talvez seja a vaga que você espera há anos. A que vai trazer tranquilidade pra sua família e orgulho pra quem sempre acreditou em você. — MEQ Concursos |
| Estuda há tempo e não passa | 6 | 5% | 11 | 3% | 75 | 10 | 6% | Lógico que na maioria das vezes estive no cenário de REPROVADO (que é o mais NORMAL) 😅😅😅 — Caderno do Aprovado - Materiais para Concursos |
| Erra questões / pegadinhas da banca | 5 | 4% | 8 | 2% | 25 | 3 | 2% | Não tem pegadinha, esse preparatório é gratuito. — Ceisc Concursos |

## Tipo de produto × ticket

Tipo identificado por palavras-chave na copy, no título do link e na headline (uma oferta pode ter vários). Ticket só entra quando foi lido no checkout.

| Tipo de produto | Anunciantes | Ofertas | Veteranas | Com ticket lido | Mínimo | Mediana | Máximo | Tickets lidos |
|---|---|---|---|---|---|---|---|---|
| Material em PDF / apostila / caderno | 60 | 68 | 33 | 6 | R$ 260 | R$ 497 | R$ 1.489 | Professor José Maria R$ 260; Brabo Editora R$ 397; Academia do Perito R$ 497; Caderno do Aprovado - Materiais para Concursos R$ 497; Caderno do Aprovado - Materiais para Concursos R$ 597; Discursiva na Prática R$ 1.489 |
| Questões / simulados | 32 | 40 | 16 | 7 | R$ 5 | R$ 260 | R$ 827 | 123passei com Hugo de Freitas R$ 5; Aprovando Concurseiro R$ 58; Thállius Moraes com Esquadrão de Elite R$ 247; Professor José Maria R$ 260; Brabo Editora R$ 397; Caderno do Aprovado - Materiais para Concursos R$ 597; Instituto INAPI R$ 827 |
| Curso em videoaulas | 31 | 42 | 24 | 7 | R$ 247 | R$ 597 | R$ 6.346 | Thállius Moraes com Esquadrão de Elite R$ 247; Brabo Editora R$ 397; Professor Raphael Reis R$ 450; Caderno do Aprovado - Materiais para Concursos R$ 597; Instituto INAPI R$ 827; Discursiva na Prática R$ 1.489; Ceisc Concursos R$ 6.346 |
| Isca gratuita / grupo VIP | 23 | 28 | 12 | 6 | R$ 260 | R$ 712 | R$ 6.346 | Professor José Maria R$ 260; Isaque Concursos R$ 497; Caderno do Aprovado - Materiais para Concursos R$ 597; Instituto INAPI R$ 827; Jus Expert R$ 997; Ceisc Concursos R$ 6.346 |
| Mentoria / acompanhamento | 22 | 27 | 14 | 2 | R$ 497 | R$ 497 | R$ 497 | Isaque Concursos R$ 497; Isaque Concursos R$ 497 |
| Cronograma / plano de estudos | 21 | 25 | 10 | 3 | R$ 247 | R$ 497 | R$ 497 | Thállius Moraes com Esquadrão de Elite R$ 247; Isaque Concursos R$ 497; Isaque Concursos R$ 497 |
| Não identificado | 17 | 19 | 12 | 7 | R$ 197 | R$ 1.725 | R$ 2.747 | Uniforenses Instituto de Pericias Forenses R$ 197; Decorando a Lei Seca Cursos Para Concursos E OAB R$ 397; Jus Expert R$ 997; Escola Trabalhista R$ 1.725; prof.camilasabongi com Escola Trabalhista R$ 1.725; Escola Trabalhista R$ 2.747; prof.camilasabongi com Escola Trabalhista R$ 2.747 |
| Discursiva / redação | 12 | 15 | 6 | 4 | R$ 247 | R$ 524 | R$ 1.489 | Thállius Moraes com Esquadrão de Elite R$ 247; Professor Raphael Reis R$ 450; Caderno do Aprovado - Materiais para Concursos R$ 597; Discursiva na Prática R$ 1.489 |
| Lei seca / legislação | 11 | 12 | 7 | 3 | R$ 58 | R$ 247 | R$ 497 | Aprovando Concurseiro R$ 58; Thállius Moraes com Esquadrão de Elite R$ 247; Caderno do Aprovado - Materiais para Concursos R$ 497 |
| Mapas mentais / esquemas | 5 | 5 | 2 | 2 | R$ 17 | R$ 257 | R$ 497 | Marcelomapas R$ 17; Caderno do Aprovado - Materiais para Concursos R$ 497 |
| Assinatura / clube / vitalício | 3 | 3 | 1 | 1 | R$ 1.489 | R$ 1.489 | R$ 1.489 | Discursiva na Prática R$ 1.489 |
| Flashcards | 1 | 1 | 1 | 0 | — | — | — |  |

## Expressões repetidas entre anunciantes

Sequências de 2 ou 3 palavras (sem acento) usadas na copy por 3 ou mais anunciantes distintos.

`clique em saiba` (18), `tecnico judiciario` (16), `analista judiciario` (12), `nivel superior` (11), `garanta sua vaga` (11), `tribunal regional` (10), `regional do trabalho` (10), `r$ 16` (10), `edital sair` (9), `concurso do trt` (9), `8a regiao` (9), `quem quer` (8), `pre edital` (8), `edital publicado` (8), `concursos publicos` (8), `concurso publico` (8), `tribunal de justica` (7), `tj sp` (7), `r$ 16 040` (7), `pos edital` (7), `nivel medio` (7), `agora mesmo` (7), `sair para comecar` (6), `reta final` (6), `remuneracao inicial` (6), `realmente importa` (6), `quem comeca` (6), `publicacao do edital` (6), `novo concurso` (6), `link da bio` (6)

## Arquivo de ganchos (anúncios mais replicados e mais antigos)

| Anunciante | Dias | Cópias | Formato | Botão | Gancho (1ª linha) | Título do link |
|---|---|---|---|---|---|---|
| Gustavo Dias | 9 | 10 | imagem | sem botão | 🔥 A sua aprovação em Concursos Públicos não depende dos Materiais! Depende de direcionamento correto. |  |
| MEQ Concursos | 8 | 8 | imagem | sem botão | Tem edital que passa. E tem edital que muda a sua vida. 💙 |  |
| Isaque Concursos | 65 | 4 | vídeo | sem botão | TRT / Como estudar em alto nível e ser aprovado para o cargo de Técnico Judiciário? |  |
| Caminho da Perícia | 33 | 4 | imagem | Saiba mais | 🚨 PROCURA-SE PEDAGOGOS🚨 | Vagas para profissionais formados |
| Caminho da Perícia | 33 | 4 | imagem | Saiba mais | 🚨 PROCURA-SE VETERINÁRIOS🚨 | Vagas para profissionais formados |
| Caminho da Perícia | 33 | 4 | vídeo | sem botão | 🚨 PROCURA-SE ENGENHEIROS AGRÔNOMOS🚨 | Vagas para profissionais formados |
| Caminho da Perícia | 33 | 4 | vídeo | Saiba mais | 🚨 PROCURA-SE ENGENHEIROS CIVIS🚨 | Vagas para profissionais formados |
| Clube do Perito | 18 | 4 | imagem | sem botão | 🚨 PROCURA-SE FISIOTERAPEUTAS🚨 |  |
| Thállius Moraes com Esquadrão de Elite | 9 | 4 | imagem | sem botão | Saiu o edital do TRT 8 — comece sua preparação agora |  |
| EnfConcursos | 895 | 3 | vídeo | sem botão | Curso Completo com Mentoria e Aulas Diários para o Concurso da EBSERH |  |
| Central de Concursos | 89 | 3 | vídeo | sem botão | O TJ-SP Escrevente é uma grande oportunidade para quem busca estabilidade e carreira pública com nível médio. |  |
| Nova Concursos | 51 | 3 | imagem | sem botão | "📚🆓 Curso Grátis TJ-SP 2026 - Escrevente Técnico Judiciário! 🆓📚 |  |
| Concurseiro aos 40 | 26 | 3 | imagem | sem botão | ⚖️ Os próximos concursos de TRTs podem abrir excelentes oportunidades em diferentes regiões do país, com remunerações iniciais que podem chegar a cerca de R$ 16 mil. |  |
| Meirelles Quintella Escritório de Advocacia | 11 | 3 | vídeo | sem botão | Alguns profissionais da área da saúde atuam em hospitais públicos sem ter ingressado por concurso. |  |
| Tjteiros | 100 | 2 | vídeo | sem botão | O concurseiro de alto nível não nasce no pós-edital. Ele se forma no pré-edital. |  |
| Brabo Concursos | 95 | 2 | vídeo | sem botão | O TJ-SP tem um novo concurso previsto para 2026, são mais de 3.300 cargos vagos de Escrevente Técnico Judiciário, temos contrato assinado com a banca organizadora e recentemente foram criados novas 720 vagas de Escrevent |  |
| Central de Concursos | 89 | 2 | vídeo | sem botão | O concurso do Tribunal de Justiça de São Paulo (TJ-SP) é uma das maiores oportunidades para quem tem apenas o ensino médio completo. Além de um excelente salário inicial, você conquista estabilidade financeira, benefício |  |
| Estratégia Concursos | 87 | 2 | vídeo | sem botão | 📢 O professor Herbert Almeida indica: vale a pena estudar para CGU e Tribunal de Contas da União! |  |
| Venâncio & Delgado - Advogados | 61 | 2 | vídeo | sem botão | ⚖️ A banca examinadora pode mudar de entendimento e te eliminar como PCD? Saiba o que o Superior Tribunal de Justiça (STJ) decidiu! |  |
| Lucas Viégas | 47 | 2 | vídeo | sem botão | Concurso TCE GO: Edital Publicado hoje! Provas em janeiro, como será a sua preparação até o dia da prova? |  |
| Milena Correia Advocacia | 26 | 2 | vídeo | sem botão | Irregularidades em concursos públicos podem arruinar seus sonhos! |  |
| Concurseiro aos 40 | 14 (baixo volume) | 2 | imagem | sem botão | 🔥 O TRT-MG já começou a se movimentar para um novo concurso em 2027. |  |
| Monica Freitas MTE | 11 | 2 | imagem | sem botão | ⚖️ O próximo concurso do TRT do Rio Grande do Sul já está em preparação, e esperar o edital sair para começar pode custar um tempo precioso. |  |
| Prof. Ronaldo Santos | 11 | 2 | imagem | sem botão | A Ana Flávia chegou até mim faltando apenas 15 dias para o concurso do Tribunal de Justiça do Rio de Janeiro. |  |
| Gustavo Nogueira - Aprovação Ágil | 11 | 2 | vídeo | sem botão | Três anos no cursinho jurídico. Sete apostilões de Direito. E fiquei em cadastro de reserva no primeiro TRT que eu prestei. |  |
| GG Concursos | 10 | 2 | imagem | Comprar agora | Vai deixar essa oportunidade passar? | Assine o GG Play 360 |
| Isaque Concursos | 9 | 2 | vídeo | sem botão | ATENÇÃO! EDITAL PUBLICADO: TRT-8 (PA/AP) |  |
| Giovanna Carranza Desenvolvimento Profissional | 9 | 2 | imagem | sem botão | Concurso TRT8! |  |
| Sou Concurseiro | 9 | 2 | vídeo | sem botão | Cada vez mais gente com 40, 50 anos está estudando para o TJ-AM: salário acima de R$ 15 mil e jornada das 8h às 14h. |  |
| Sou Concurseiro | 9 | 2 | vídeo | sem botão | Acabou a faculdade ou vai se formar este ano? O concurso do TJ-AM pode ser o seu próximo passo. |  |
| Sou Concurseiro | 9 | 2 | vídeo | sem botão | Qualquer curso superior, salário acima de R$ 15 mil e jornada das 8h às 14h: esse é o concurso do TJ-AM. |  |
| Sou Concurseiro | 9 | 2 | vídeo | sem botão | Acha que já passou da idade para estudar? No TJ-AM tem gente de 30, 40 e 50 anos se preparando agora. |  |
| Sou Concurseiro | 9 | 2 | vídeo | sem botão | Mais de 30 ou 40 anos e ensino superior? Presta atenção no concurso do TJ-AM: 400 vagas e jornada das 8h às 14h. |  |
| Sou Concurseiro | 9 | 2 | vídeo | sem botão | Mais de 40 anos, ensino superior e vontade de mudar de carreira? Conheça o concurso do TJ-AM: 400 vagas. |  |
| Sou Concurseiro | 9 | 2 | vídeo | sem botão | Tem mais de 30, 40 ou 50 anos e já tem ensino superior? O Tribunal de Justiça do Amazonas pode ser a sua transição de carreira. |  |
| Delta Fabio Silva | 8 | 2 | vídeo | sem botão | E aí vamos cair de cabeça nesses CONCURSOS POLICIAIS DO AMAZONAS? |  |
| Flávio Britto Advocacia | 8 | 2 | vídeo | sem botão | Quer saber quais questões são passíveis de anulação pela via judicial no concurso da PPRN? |  |
| Caderno do Aprovado - Materiais para Concursos | 927 | 1 | imagem | sem botão | A matéria para concurso já é grande e os cursinhos ainda complicam mais: centenas de horas de videoaulas e milhares de páginas de PDFs. | Simbora Concursos |
| Simbora Concursos | 927 | 1 | carrossel | Visitar perfil do Instagram | Quando eu comecei a estudar para Tribunais, ficar "nas cabeças" era algo inimaginável... 1º lugar, então? Era coisa de maluco, extraterrestre, etc. |  |
| Caderno do Aprovado - Materiais para Concursos | 837 | 1 | carrossel | Visitar perfil do Instagram | Lançados em junho de 2024 |  |

---

# Parte 1 — Ofertas de foco direto (75)

---
id_oferta: 001
anunciante: "Isaque Concursos"
url_destino: "https://projetotrt.com.br/imersao1v1/"
ad_library_url: "https://www.facebook.com/ads/library/?id=3249712645216747"
dias_ativo: 65
anuncios_coletados: 10
anuncios_ativos_estimados: 33
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tecnico judiciario"
plataforma_checkout: "onprofit"
ticket_principal: "R$ 497,00"
fonte_ticket: "checkout"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (10)"
botoes: "sem botão (9), Saiba mais (1)"
parcelas: "12x R$ 42,99"
precos_exibidos_na_lp: "R$ 9.776,71 | R$ 90,00 | R$ 11.928 | R$ 0 | R$ 997 | R$ 100 | R$ 497 | R$ 397"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
anunciante: "Portal & OAB"
url_destino: "https://olympus.cursosdoportal.com.br/o-adm-trt-pa/?utm_source=%7B%7Bsite_source_name%7D%7D&utm_medium=%7B%7Badset.name%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D&utm_term=%7B%7Bplacement%7D%7D&utm_content=%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1074976398625545"
dias_ativo: 13
anuncios_coletados: 21
anuncios_ativos_estimados: 21
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tribunal regional do trabalho, trt 8, tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados, Cronograma / plano de estudos, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (6), imagem (15)"
botoes: "Ver detalhes (6), sem botão (15)"
precos_exibidos_na_lp: "R$ 9.776,71 | R$ 16.040,88"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://www.facebook.com/simboraconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=436273172079349"
dias_ativo: 927
anuncios_coletados: 20
anuncios_ativos_estimados: 20
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trt, tst"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Discursiva / redação"
formatos_dos_anuncios: "carrossel (16), vídeo (2), imagem (2)"
botoes: "Visitar perfil do Instagram (11), sem botão (9)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
- Lançados em agosto de 2025
- Lançados em fevereiro de 2025
- 3 cenários de APROVAÇÃO ✅️
- O caderno de Português do 1º lugar no TRT-PI, com toda a teoria organizada de forma objetiva + questões comentadas das 3 principais bancas de concurso (FCC, FGV e Cespe/Cebraspe).
- Lançados em outubro de 2024
- Lançados em agosto de 2024

### Títulos do link nos anúncios
- Beto - Caderno Do Aprovado - TRT, TST e TJ - José Humberto (@cadernoaprovado) • Instagram photos and videos
- Simbora Concursos
- Beto (José Humberto) - Caderno Do Aprovado - TRT/TST/TJ/MP (@cadernoaprovado) • Instagram photos and videos
- Beto - Caderno Do Aprovado - TRT e TRE/TSE - José Humberto (@cadernoaprovado) • Instagram photos and videos

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 004
anunciante: "Leandro Reinhardt l Estudos & Concursos"
url_destino: "https://leandroreinhardt.com.br/trt-desafio-nucleo-duro-tjaa/?utm_source=meta-ads&utm_medium=%7B%7Badset.name%7D%7D%7C%7B%7Badset.id%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D%7C%7B%7Bcampaign.id%7D%7D&utm_content=%7B%7Bad.name%7D%7D%7C%7B%7Bad.id%7D%7D&utm_term=%7B%7Bplacement%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=3626400700862360"
dias_ativo: 14
anuncios_coletados: 15
anuncios_ativos_estimados: 15
anuncios_com_baixo_volume_de_impressoes: 1
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tjaa"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados"
formatos_dos_anuncios: "imagem (15)"
botoes: "Saiba mais (15)"
precos_exibidos_na_lp: "R$ 297 | R$ 97 | 12x de R$ 9,70"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
anunciante: "MEQ Concursos"
url_destino: "https://meqconcursos.com.br/aprovameq-trt-8/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1654328612881726"
dias_ativo: 8
anuncios_coletados: 5
anuncios_ativos_estimados: 15
anuncios_com_baixo_volume_de_impressoes: 1
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt 8, tjaa"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Questões / simulados, Discursiva / redação, Cronograma / plano de estudos"
formatos_dos_anuncios: "vídeo (3), imagem (2)"
botoes: "sem botão (4), Saiba mais (1)"
precos_exibidos_na_lp: "R$ 16.040,88 | R$ 997 | 12x de R$ 58,08 | R$ 627,30 | R$ 1.394,00 | 12x de R$ 83,03 | R$ 897,30"
primeira_coleta_propria: "2026-10-11"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"<100
Tem edital que passa. E tem edital que muda a sua vida. 💙
O TRT-8 saiu com remuneração de até R$ 16.040,88, estabilidade e prova marcada para 17/01/2027.
Talvez seja a vaga que você espera há anos. A que vai trazer tranquilidade pra sua família e orgulho pra quem sempre acreditou em você.
Você não precisa enfrentar essa reta final sozinho(a). No AprovaMEQ TRT-8 você tem:
📅 Cronogramas de 3h ou 5h por dia para Analista (AJAJ) e Técnico (TJAA)� 📘 PDMEQuinhos, VadeMEQ e Regimento Interno� ✍🏼 3 simulados completos com estudo de caso e redação� 👥 Mentoria mensal e grupo no WhatsApp com o prof. Breno Lenza
👉 Clique em Saiba mais e comece hoje a sua preparação para o TRT-8."

### Ganchos das variações (1ª linha de cada anúncio)
- Tem edital que passa. E tem edital que muda a sua vida. 💙
- <100

### Títulos do link nos anúncios
- Clique em Saiba mais e comece hoje a sua preparação para o TRT-8

### Landing Page: Headline & Promessa Central
"A sua preparação completa para o TRT-8 — Do edital até a prova, o MEQ te entrega tudo o que você precisa para chegar mais preparado até a prova do TRT 8 e conquistar a estabilidade com um salário de R$ 16.040,88"

### Seções da Landing Page (títulos, na ordem)
- Curso de Reta Final COMPLETO
- 3 Simulados completos para cada carreira
- TUDO que você vai receber no AprovaMEQ TRT-8:
- 2 Opções de Cronograma para cada Carreira – AJAJ e TJAA:
- Materiais completos e direcionados:
- Videoaulas de temas selecionados das principais matérias:
- 03 simulados completos de cada carreira:
- Comece hoje a sua Reta Final
- Finalize sua preparação
- Dados confirmados!

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
primeira_coleta_propria: "2026-10-08"
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
id_oferta: 007
anunciante: "Concurseiro aos 40"
url_destino: "https://form.respondi.app/CN2Wk6Lk"
ad_library_url: "https://www.facebook.com/ads/library/?id=1085157223929037"
dias_ativo: 26
anuncios_coletados: 4
anuncios_ativos_estimados: 11
anuncios_com_baixo_volume_de_impressoes: 1
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, justica do trabalho"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "imagem (4)"
botoes: "sem botão (4)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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

### Landing Page: Headline & Promessa Central
"Inicie o passo mais importante rumo à sua aprovação no Concurso do TRT"

### Entregáveis / Formato (termos encontrados na LP)
- Mentoria


========================================

---
id_oferta: 008
anunciante: "Portal Concursos"
url_destino: "https://oportalconcursos.com.br/h-adm-trt-mt/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1436015981795868"
dias_ativo: 11
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
formatos_dos_anuncios: "vídeo (1), imagem (10)"
botoes: "Saiba mais (11)"
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
id_oferta: 009
anunciante: "Monica Freitas MTE"
url_destino: "https://form.respondi.app/yLeg4HU6"
ad_library_url: "https://www.facebook.com/ads/library/?id=4497844090493414"
dias_ativo: 11
anuncios_coletados: 6
anuncios_ativos_estimados: 10
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Questões / simulados, Cronograma / plano de estudos"
formatos_dos_anuncios: "imagem (6)"
botoes: "sem botão (4), Saiba mais (2)"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 4
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
id_oferta: 010
anunciante: "Isaque Concursos"
url_destino: "https://projetotrt.com.br/vsl1v1/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1023281740551609"
dias_ativo: 65
anuncios_coletados: 9
anuncios_ativos_estimados: 9
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tecnico judiciario"
plataforma_checkout: "onprofit"
ticket_principal: "R$ 497,00"
fonte_ticket: "checkout"
tipos_produto: "Mentoria / acompanhamento, Cronograma / plano de estudos"
formatos_dos_anuncios: "vídeo (9)"
botoes: "Saiba mais (9)"
parcelas: "12x R$ 42,99"
precos_exibidos_na_lp: "12x de R$ 43 | R$ 9.776,71 | R$ 90,00 | R$ 11.928 | R$ 0 | R$ 997 | R$ 100 | R$ 497"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
- Total organização e direcionamento paraestudar em alto nível para qualquer TRT do Brasil com o Projeto TRT 🔥
- Tenha organização e direcionamento para
- Tenha tudo que você precisa para estudar em alto nível para qualquer TRT do Brasil com o Projeto TRT🔥

### Títulos do link nos anúncios
- Projeto TRT: Ecossistema Completo para TRTs
- TRTs: Organização e Direcionamento
- TRT: Estude em Alto Nível

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
id_oferta: 011
anunciante: "Vinco Leilões"
url_destino: "https://www.vincoleiloes.com.br/lote.php?idLote=7315"
ad_library_url: "https://www.facebook.com/ads/library/?id=1749137523049974"
dias_ativo: 11
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
dias_distintos_coletado: 4
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
id_oferta: 012
anunciante: "Thállius Moraes com Esquadrão de Elite"
url_destino: "https://lp.oesquadraodeelite.com.br/curso-intensivo-trt-8-reta-final"
ad_library_url: "https://www.facebook.com/ads/library/?id=1842940127056507"
dias_ativo: 9
anuncios_coletados: 3
anuncios_ativos_estimados: 9
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt 8, tecnico judiciario, tjaa"
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
id_oferta: 013
anunciante: "Leandro Reinhardt l Estudos & Concursos"
url_destino: "https://leandroreinhardt.com.br/trt-desafio-nucleo-duro/?utm_source=meta-ads&utm_medium=%7B%7Badset.name%7D%7D%7C%7B%7Badset.id%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D%7C%7B%7Bcampaign.id%7D%7D&utm_content=%7B%7Bad.name%7D%7D%7C%7B%7Bad.id%7D%7D&utm_term=%7B%7Bplacement%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1106077182358238"
dias_ativo: 14
anuncios_coletados: 8
anuncios_ativos_estimados: 8
anuncios_com_baixo_volume_de_impressoes: 2
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Questões / simulados"
formatos_dos_anuncios: "imagem (8)"
botoes: "Saiba mais (8)"
precos_exibidos_na_lp: "R$ 297 | R$ 97 | 12x de R$ 9,70"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"<100
Domine o núcleo duro dos TRTs em 70 dias
70 dias, 1 hora por dia, com o Mapa de Engenharia Reversa da FCC."

### Ganchos das variações (1ª linha de cada anúncio)
- Domine o núcleo duro dos TRTs em 70 dias
- Não falta tempo. Falta direção.
- 29 tópicos concentram 72% das específicas
- <100

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
id_oferta: 014
anunciante: "Isaque Concursos"
url_destino: "https://projetotrt.com.br/trt8/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1400478538904369"
dias_ativo: 9
anuncios_coletados: 4
anuncios_ativos_estimados: 8
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt8, tecnico judiciario"
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
id_oferta: 015
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
primeira_coleta_propria: "2026-10-08"
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
id_oferta: 016
anunciante: "MEQ Concursos"
url_destino: "https://www.facebook.com/61586241338760/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1652434139167708"
dias_ativo: 144
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
id_oferta: 017
anunciante: "Gazeta dos Concursos"
url_destino: "https://lp.aprovacaoagil.com.br/vsl-white-trt-noticia"
ad_library_url: "https://www.facebook.com/ads/library/?id=2150289195888138"
dias_ativo: 79
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
id_oferta: 018
anunciante: "Mentoria Tribunal do Trabalho"
url_destino: "https://www.professoreduardojose.com.br/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1153138433958818"
dias_ativo: 8
anuncios_coletados: 5
anuncios_ativos_estimados: 5
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, justica do trabalho"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento"
formatos_dos_anuncios: "vídeo (5)"
botoes: "Saiba mais (5)"
primeira_coleta_propria: "2026-10-11"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Você está a um clique de estudar com um plano 100% guiado por mim até sua aprovação no TRT.
Faça sua aplicação agora."

### Títulos do link nos anúncios
- Mentoria Individual TRT

### Landing Page: Headline & Promessa Central
"Mentoria TRT - Prof. Eduardo José — Olá, Futuro(a) Técnico(a) ou Analista da Justiça do Trabalho!"

### Seções da Landing Page (títulos, na ordem)
- Olá, Futuro(a) Técnico(a) ou Analista da Justiça do Trabalho!
- As 7 entregas da mentoria que te colocam em nível de nomeação no TRT:
- Alguns Spoilers:

### Entregáveis / Formato (termos encontrados na LP)
- Cronograma
- Mapas mentais
- Mentoria
- PDF
- Resumos
- Videoaulas


========================================

---
id_oferta: 019
anunciante: "Escola Trabalhista"
url_destino: "https://escolatrabalhista.com.br/preparacao-acesso-total-trt-tst/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1290097296395901"
dias_ativo: 188
anuncios_coletados: 4
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "forte"
foco_direto: sim
termos_foco_encontrados: "trt, tst, tecnico judiciario"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 2.746,65"
fonte_ticket: "checkout"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "vídeo (3), imagem (1)"
botoes: "Saiba mais (2), Comprar agora (2)"
parcelas: "12x de R$ 284,07"
precos_exibidos_na_lp: "R$ 1,00 | R$ 2.746,65 | 12x de R$ 284,07"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
id_oferta: 020
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2089-concurso-trt-4-club-analista-judiciario-area-judiciaria"
ad_library_url: "https://www.facebook.com/ads/library/?id=2796129990724803"
dias_ativo: 169
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
precos_exibidos_na_lp: "R$ 16 | R$ 16.041,21 | R$ 9.007,67 | R$ 2.137,00 | R$ 1.495,90 | 12x de R$ 124,66"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
id_oferta: 021
anunciante: "Meirelles Quintella Escritório de Advocacia"
url_destino: "https://www.facebook.com/100090050235471/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2118332055398747"
dias_ativo: 158
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
dias_distintos_coletado: 5
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
id_oferta: 022
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
dias_distintos_coletado: 5
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
id_oferta: 023
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://cadernodoaprovado.com/trf-tj-mp/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1533733075435407"
dias_ativo: 68
anuncios_coletados: 4
anuncios_ativos_estimados: 4
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 497,00"
fonte_ticket: "checkout"
tipos_produto: "Material em PDF / apostila / caderno, Mapas mentais / esquemas, Lei seca / legislação"
formatos_dos_anuncios: "carrossel (3), imagem (1)"
botoes: "Saiba mais (2), Ver detalhes (1), sem botão (1)"
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

### Ganchos das variações (1ª linha de cada anúncio)
- 🚨 O concurso do MP-PE está previsto e quem começa agora larga na frente.
- 🚨 O edital do TRF-3 pode sair a qualquer momento!

### Títulos do link nos anúncios
- Combo MP-PE
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
id_oferta: 024
anunciante: "prof.camilasabongi com Escola Trabalhista"
url_destino: "https://escolatrabalhista.com.br/preparacao-acesso-total-trt-tst/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1278772247787449"
dias_ativo: 184
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
dias_distintos_coletado: 5
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
id_oferta: 025
anunciante: "Instituto INAPI"
url_destino: "https://cursos.inapionline.com.br/pre-trt-pi"
ad_library_url: "https://www.facebook.com/ads/library/?id=1364004345923443"
dias_ativo: 55
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tecnico judiciario"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 827,00"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Questões / simulados, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (2), imagem (1)"
botoes: "Saiba mais (2), Ver detalhes (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
id_oferta: 026
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
dias_distintos_coletado: 5
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
id_oferta: 027
anunciante: "Verbo Carreiras Jurídicas"
url_destino: "https://www.facebook.com/verbocarreirasjuridicas/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1110449348094847"
dias_ativo: 18
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
dias_distintos_coletado: 5
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
anunciante: "Prime Curso"
url_destino: "https://sala.concurseiroprime.com.br/buscar?query=trt"
ad_library_url: "https://www.facebook.com/ads/library/?id=1635879998169503"
dias_ativo: 16
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tribunal regional do trabalho, trt8, trt22, tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "imagem (3)"
botoes: "Comprar agora (3)"
precos_exibidos_na_lp: "R$ 42,00 | 10x de R$ 42,00 | R$ 1200 | R$ 378,00 | R$ 49,00 | 10x de R$ 49,00 | R$ 1400 | R$ 441,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
id_oferta: 029
anunciante: "Professor Raphael Reis"
url_destino: "https://www.facebook.com/profraphaelreis/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1494830749215441"
dias_ativo: 11
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
- Concorda com a classificação do Prof. Rapha? rsrs

### Títulos do link nos anúncios
- instagram.com

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 030
anunciante: "Memoriza-aí Concursos"
url_destino: "https://memorizaai.com.br/trt-8/?src=&utm_source=facebook-ads&utm_medium=%7B%7Badset.name%7D%7D&utm_content=%7B%7Bad.name%7D%7D&utm_campaign=%7B%7Bcampaign.name%7D%7D&utm_term=%7B%7Bplacement%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1412217740406316"
dias_ativo: 9
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tribunal regional do trabalho, trt 8"
plataforma_checkout: "eduzz"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "imagem (2), carrossel (1)"
botoes: "Saiba mais (3)"
precos_exibidos_na_lp: "R$ 18.380 | R$ 18.380,17 | R$ 16.040,88 | R$ 9.776,71 | R$ 11.202,48 | R$ 39,90 | R$ 0,00 | R$ 27,00"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 Concurso Tribunal Regional do Trabalho - 8ª Região com edital publicado! Salário de até R$18 mil.
Mas atenção: em um concurso deste nível, o maior erro é tentar estudar tudo sem prioridade.
Com o Memoriza.ai, você estuda com foco no que realmente importa:
✅ Material direto ao ponto para o cargo escolhido
✅ Conteúdo organizado para revisão estratégica
✅ Direcionamento pelos temas mais relevantes
✅ Linguagem objetiva, sem excesso desnecessário
✅ Estrutura pensada para acelerar sua preparação até a prova
👉 Clique em Saiba Mais e comece sua preparação hoje."

### Títulos do link nos anúncios
- Concurso TRT 8 - Edital publicado!

### Landing Page: Headline & Promessa Central
"edital publicado: tribunal regional do trabalho DA 8ª região SÃO 24 cargos em cr E SALÁRIO DE ATÉ — Estude com um material objetivo e direcionado aos principais pontos do edital e organize sua preparação para disputar uma das vagas do TRT."

### Seções da Landing Page (títulos, na ordem)
- O segredo dos aprovados no TRT 8
- POR QUE DEVO ESTUDAR COM O MEMORIZA.AI?
- UMA AMOSTRA DO MATERIAL REAL
- QUEM JÁ USOU NOSSOS MATERIAIS APROVA.
- ALÉM DO MATERIAL, VOCÊ AINDA LEVA 5 BÔNUS ESPECIAIS
- DO ZERO À APROVAÇÃO
- CADERNO DE ERROS DA RETA FINAL
- MANUAL DA RESOLUÇÃO DE QUESTÕES
- CRONOGRAMA DE 30 DIAS
- RAIO X DA FCC
- VEJA POR QUE O MEMORIZA.AI — TRT - 8ª REGIÃO É O CAMINHO CERTO PARA SUA PREPARAÇÃO
- COMECE AGORA SUA preparação
- Perguntas Frequentes
- Você está inseguro com a compra?
- Memoriza-aí | Concursos Públicos
- Redes sociais:

### Entregáveis / Formato (termos encontrados na LP)
- Caderno de erros
- Cronograma
- Discursiva / redação
- PDF


========================================

---
id_oferta: 031
anunciante: "Decorando a Lei Seca Cursos Para Concursos E OAB"
url_destino: "https://www.decorandoaleiseca.com.br/retafinal/analista-judiciario-area-judiciaria-trt-8-regiao"
ad_library_url: "https://www.facebook.com/ads/library/?id=1807015203847696"
dias_ativo: 9
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt 8, tecnico judiciario"
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
id_oferta: 032
anunciante: "cadernodoconcurseiro"
url_destino: "https://cadernodoconcurseiro.com.br/produto/combo-trt-8-tecnico-judiciario-area-administrativa/"
ad_library_url: "https://www.facebook.com/ads/library/?id=3497705397069418"
dias_ativo: 8
anuncios_coletados: 3
anuncios_ativos_estimados: 3
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tribunal regional do trabalho, trt 8, tecnico judiciario"
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
id_oferta: 033
anunciante: "Escola Trabalhista"
url_destino: "https://conteudos.escolatrabalhista.com.br/raio-x"
ad_library_url: "https://www.facebook.com/ads/library/?id=1566347627818236"
dias_ativo: 251
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
dias_distintos_coletado: 4
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
id_oferta: 034
anunciante: "Trteiros"
url_destino: "https://www.facebook.com/61560675890210/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1931729394374222"
dias_ativo: 170
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Curso em videoaulas, Material em PDF / apostila / caderno"
formatos_dos_anuncios: "imagem (1), vídeo (1)"
botoes: "sem botão (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
- A metodologia do curso TRTeiros é o que está faltando na sua aprovação 🧡📚🚀

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 035
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2292-concurso-trt-nacional-club-analista-judiciario-area-judiciaria"
ad_library_url: "https://www.facebook.com/ads/library/?id=2005552620380372"
dias_ativo: 169
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Curso em videoaulas, Material em PDF / apostila / caderno, Questões / simulados"
formatos_dos_anuncios: "vídeo (1), imagem (1)"
botoes: "sem botão (1), Saiba mais (1)"
precos_exibidos_na_lp: "R$ 16 | R$ 9.007,67 | R$ 3.710,00 | R$ 2.597,00 | 12x de R$ 216,42"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
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

### Ganchos das variações (1ª linha de cada anúncio)
- Um preparatório para diversos concursos de Tribunais Regionais do Trabalho? 🚨
- Lançados em abril de 2026

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
id_oferta: 036
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
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
id_oferta: 037
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
primeira_coleta_propria: "2026-10-08"
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
id_oferta: 038
anunciante: "Concursos Ceisc"
url_destino: "https://ceisc.com.br/cursos/2138-concurso-trt-4-club-tecnico-judiciario-area-administrativa?utm_source=meta_ads&utm_medium=cpc&utm_campaign=vendas_trt_4_club_tec_judiciario&utm_term=advantage"
ad_library_url: "https://www.facebook.com/ads/library/?id=1020843757391368"
dias_ativo: 88
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
precos_exibidos_na_lp: "R$ 9 | R$ 9.776,71 | R$ 9.007,67 | R$ 1.797,00 | R$ 1.257,90 | 12x de R$ 104,83"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
id_oferta: 039
anunciante: "Gustavo Nogueira - Aprovação Ágil"
url_destino: "https://lp.aprovacaoagil.com.br/vsl-white-trt-noticia"
ad_library_url: "https://www.facebook.com/ads/library/?id=1327405757117765"
dias_ativo: 47
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tst"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Lei seca / legislação"
formatos_dos_anuncios: "vídeo (2)"
botoes: "Saiba mais (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
""Quero muito passar num TRT, começo por onde?"
Você está no melhor momento pra começar. Qualquer graduação te habilita pro técnico — R$11.500 iniciais, jornada de 35 horas. Somando os 24 TRTs e o TST, são 25 portas abertas na mesma matéria.
Só que começar não é sentar num apostilão de cursinho. É virar a ordem: questão comentada, gabarito destrinchado, lei seca e súmula do TST.
Foi assim que o Walter fechou o TRT-4 em 23º lugar pra analista. Não cadastro de reserva. Nomeado.
Assiste o vídeo e clica no botão — a ordem exata pra você começar hoje."

### Ganchos das variações (1ª linha de cada anúncio)
- Qual o melhor concurso de tribunal pra você começar hoje?
- "Quero muito passar num TRT, começo por onde?"

### Títulos do link nos anúncios
- Melhor tribunal pra começar hoje
- Quero passar num TRT — por onde?

### Landing Page: Headline & Promessa Central
"Título"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 040
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://cadernodoaprovado.com/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1808412633912288"
dias_ativo: 33
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
dias_distintos_coletado: 5
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
id_oferta: 041
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://cadernodoaprovado.com/trt-v2/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1995131297827496"
dias_ativo: 30
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, justica do trabalho, tst"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 597,00"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno, Questões / simulados, Discursiva / redação, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "carrossel (2)"
botoes: "sem botão (2)"
precos_exibidos_na_lp: "R$ 9.776,71 | R$ 1.089,00 | 12x de R$ 49,75 | R$ 16.040,88 | R$ 1.188,00 | 12x de R$ 53,92 | R$ 1.386,00 | 12x de R$ 62,25"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
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
id_oferta: 042
anunciante: "Professor Fabiano Pereira"
url_destino: "https://www.facebook.com/professorfp/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1622749052884640"
dias_ativo: 20
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Material em PDF / apostila / caderno, Questões / simulados"
formatos_dos_anuncios: "carrossel (1), vídeo (1)"
botoes: "Visitar perfil do Instagram (1), sem botão (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
id_oferta: 043
anunciante: "Weverton Reis"
url_destino: "https://www.facebook.com/100070415432523/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1069790249007641"
dias_ativo: 17
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
dias_distintos_coletado: 5
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
id_oferta: 044
anunciante: "Markup Inc."
url_destino: "http://fb.me/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1327471585972272"
dias_ativo: 17
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Não identificado"
formatos_dos_anuncios: "vídeo (1), imagem (1)"
botoes: "Cadastre-se (2)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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

### Títulos do link nos anúncios
- Clique e receba mais informações

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 045
anunciante: "Malditafcc"
url_destino: "https://www.facebook.com/malditafcc/"
ad_library_url: "https://www.facebook.com/ads/library/?id=4717861935137850"
dias_ativo: 12
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt3, trt4, trt8, trt18"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "carrossel (2)"
botoes: "sem botão (1), Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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

### Ganchos das variações (1ª linha de cada anúncio)
- Saiu o edital do TRT 8 e eu já te adianto: dá tempo, sim!
- Os TRTs estão se mexendo e tem muita gente que só vai perceber quando o edital sair.

### Títulos do link nos anúncios
- Mateus Alves (@malditafcc) • Instagram photos and videos

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 046
anunciante: "Professor Raphael Reis"
url_destino: "https://www.professorraphaelreis.com.br/curso/curso-de-redacao-trt-8-tecnico/"
ad_library_url: "https://www.facebook.com/ads/library/?id=4394209337506519"
dias_ativo: 11
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt8, trt 8"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 450,00"
fonte_ticket: "checkout"
tipos_produto: "Curso em videoaulas, Discursiva / redação"
formatos_dos_anuncios: "carrossel (2)"
botoes: "Saiba mais (1), sem botão (1)"
precos_exibidos_na_lp: "12x de R$ 49,32 | R$ 450,00"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 4
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps:
  - nome: "Agente de I.A: Bruxinho da Redação Tenha o"
    valor: "R$ 21,90"
  - nome: "Mapas Mentais para usar na Redação Revise com"
    valor: "R$ 61,00"
---
### Copy do Anúncio (Gancho de Entrada)
"Saiu o danado do edital do TRT-8 - eu falei que seria o primeiro do ciclo de TRTs ;)
Quer buscar a nota 10 e ficar mais perto de sua aprovação?
Então, venha estudar comigo! Digite TRT8 nos comentários e receba o link do curso
#concursospublicos #concursotrt8 #trt8 #redação #magodaredação"

### Ganchos das variações (1ª linha de cada anúncio)
- Saiu o danado do edital do TRT-8 - eu falei que seria o primeiro do ciclo de TRTs ;)
- Aprenda com quem é referência nacional em redação para concursos e transforme a discursiva em um dos seus maiores diferenciais.

### Títulos do link nos anúncios
- Curso de Redação TRT-8 - Mago da Redação
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
id_oferta: 047
anunciante: "Gustavo Nogueira - Aprovação Ágil"
url_destino: "https://pages.aprovacaoagil.com.br/vsl/trt/v01"
ad_library_url: "https://www.facebook.com/ads/library/?id=1762089464999221"
dias_ativo: 11
anuncios_coletados: 1
anuncios_ativos_estimados: 2
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
dias_distintos_coletado: 4
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
id_oferta: 048
anunciante: "Papa Concursos"
url_destino: "https://www.facebook.com/papaconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1122974903503846"
dias_ativo: 9
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, justica do trabalho"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Material em PDF / apostila / caderno, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (1), vídeo (1)"
botoes: "sem botão (1), Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"📌 A projeção considera:
✅ Ampliação do número de cargos ofertados;
✅ Retorno de carreiras muito aguardadas, como Polícia Judicial e Oficial de Justiça;
✅ Inclusão de novas especialidades;
✅ Alto interesse pelos concursos da Justiça do Trabalho.
Isso significa que a disputa deve ser ainda mais acirrada.
Mas vale lembrar: mais inscritos não significa mais concorrentes preparados.
A sua classificação depende da qualidade da sua preparação, não apenas do número de pessoas que farão a prova.
Comente TRT e entre na lista de espera do curso Revisão Final TRT-4 e TRT-8 e seja um dos primeiros a saber quando as turmas forem abertas."

### Ganchos das variações (1ª linha de cada anúncio)
- 📌 A projeção considera:
- Pré-edital é um estado de espírito. 🫠 Enquanto o TRT-4 e TRT-8 não saem, seguimos no mood “Alto em”: motivação, foco na FCC e estudo até a nomeação com a Revisão Final fazendo parte dessa rotina. 📚

### Títulos do link nos anúncios
- instagram.com

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 049
anunciante: "Site RP"
url_destino: "https://www.trt8.jus.br/noticias/2026/edital-para-concurso-publico-do-trt-8-e-publicado"
ad_library_url: "https://www.facebook.com/ads/library/?id=2510089052822709"
dias_ativo: 9
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tribunal regional do trabalho, trt8, trt 8, tecnico judiciario"
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
id_oferta: 050
anunciante: "Giovanna Carranza Desenvolvimento Profissional"
url_destino: "https://carranzacursos.com.br/trf8/?utm_source=mta-ads"
ad_library_url: "https://www.facebook.com/ads/library/?id=1567253011343102"
dias_ativo: 9
anuncios_coletados: 1
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tribunal regional do trabalho, trt8, trt 8"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (1)"
botoes: "sem botão (1)"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
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
id_oferta: 051
anunciante: "cadernodoconcurseiro"
url_destino: "https://www.facebook.com/100064118526627/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1101272539160972"
dias_ativo: 9
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tribunal regional do trabalho, tecnico judiciario"
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
id_oferta: 052
anunciante: "Mentoria Tribunal do Trabalho"
url_destino: "https://www.facebook.com/61566455297489/"
ad_library_url: "https://www.facebook.com/ads/library/?id=4055303854772265"
dias_ativo: 8
anuncios_coletados: 2
anuncios_ativos_estimados: 2
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Mentoria / acompanhamento, Material em PDF / apostila / caderno"
formatos_dos_anuncios: "imagem (1), carrossel (1)"
botoes: "sem botão (1), Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-11"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Se o seu objetivo é ser Técnico ou Analista do TRT, olha a quantidade de oportunidades que podem surgir nos próximos anos. 👀
São 17 TRTs com concursos cuja validade termina até 2028. Conforme essas validades chegam ao fim, novas oportunidades de concurso podem surgir.
Quem começa a se preparar antes do edital tem mais tempo para construir uma base realmente competitiva.
Quer começar sua preparação para os próximos TRTs com um plano estruturado?
Link na minha bio! 🚀
-
-
-
-
-
#concursotrt #trteiros #analistatrt #técnicotrt #mentoriatrt"

### Ganchos das variações (1ª linha de cada anúncio)
- Se o seu objetivo é ser Técnico ou Analista do TRT, olha a quantidade de oportunidades que podem surgir nos próximos anos. 👀
- A nomeação não compra status. Compra paz 🙏

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 053
anunciante: "Simbora Concursos"
url_destino: "https://www.facebook.com/simboraconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=3157233831074462"
dias_ativo: 927
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
dias_distintos_coletado: 5
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
id_oferta: 054
anunciante: "Escola Trabalhista"
url_destino: "https://escolatrabalhista.com.br/preparacao-extensiva-analista-judiciario-do-trt-area-judiciaria/"
ad_library_url: "https://www.facebook.com/ads/library/?id=971307882122417"
dias_ativo: 188
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
dias_distintos_coletado: 5
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
id_oferta: 055
anunciante: "prof.camilasabongi com Escola Trabalhista"
url_destino: "https://escolatrabalhista.com.br/preparacao-extensiva-analista-judiciario-do-trt-area-judiciaria/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1284621483770100"
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
dias_distintos_coletado: 4
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
id_oferta: 056
anunciante: "Concurseiro aos 40"
url_destino: "https://www.facebook.com/61564214427286/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1330662368927610"
dias_ativo: 163
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
dias_distintos_coletado: 5
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
id_oferta: 057
anunciante: "Pódio Procuradorias"
url_destino: "https://cronosconcursos.com.br/livro-fichamento/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1023341813683635"
dias_ativo: 130
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
dias_distintos_coletado: 5
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
id_oferta: 058
anunciante: "Concursosmeucurso"
url_destino: "https://meucurso.com.br/cursos/concursos-publicos"
ad_library_url: "https://www.facebook.com/ads/library/?id=1542521100851019"
dias_ativo: 81
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tecnico judiciario"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "carrossel (1)"
botoes: "Saiba mais (1)"
precos_exibidos_na_lp: "R$ 350 | R$ 699,00 | 12x de R$ 29,08 | R$ 349,00 | 12x de R$ 40,78 | R$ 489,30 | R$ 999,00 | 12x de R$ 66,58"
primeira_coleta_propria: "2026-10-08"
dias_distintos_coletado: 4
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
id_oferta: 059
anunciante: "BZP Bancários"
url_destino: "http://fb.me/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2249586425882185"
dias_ativo: 54
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
dias_distintos_coletado: 4
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
id_oferta: 060
anunciante: "Temas Repetitivos do TST"
url_destino: "https://www.facebook.com/61572339242984/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1058098680253103"
dias_ativo: 48
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tst"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "carrossel (1)"
botoes: "Visitar perfil do Instagram (1)"
primeira_coleta_propria: "2026-10-09"
dias_distintos_coletado: 3
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Concursos Gerais / Educacional"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Comente TEMAS e eu te envio no direct o link para conhecer o e-book dinâmico Temas Repetitivos do TST. Nele, cada Tema vem com tese, contexto, fundamentos, aplicação e infográfico. O e-book é acompanhado por um agente de IA exclusivo (Radar dos Temas do TST) para identificação de Temas Repetitivos e explicações sobre seu contexto e temas correlatos.
Tudo isso para ter segurança na prática trabalhista e na preparação para concursos públicos. Domine os Temas Repetitivos do TST!"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 061
anunciante: "123passei com Hugo de Freitas"
url_destino: "https://go.123passei.com.br/protocolo-questoes-trt/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1381997997479894"
dias_ativo: 47
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tst"
plataforma_checkout: "eduzz"
ticket_principal: "R$ 5,17"
fonte_ticket: "checkout"
tipos_produto: "Questões / simulados"
formatos_dos_anuncios: "vídeo (1)"
botoes: "Saiba mais (1)"
precos_exibidos_na_lp: "R$ 27 | R$ 300 | R$ 500 | R$ 800 | R$ 27,90"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps:
  - nome: "Oferta única : Essa chance não volta. É"
    valor: "R$ 69,90"
---
### Copy do Anúncio (Gancho de Entrada)
"Você estuda, mas ainda não sabe o que vai cair na sua prova de TRT.
O Protocolo TRT resolve isso.
São 5 materiais prontos, baseados na análise de 46 provas reais de 23 tribunais — o ciclo completo de 2022 a 2025.
✅ Mapa de peso por disciplina
✅ O que FCC, CEBRASPE e FGV cobram em cada matéria
✅ Os 50 artigos da CLT mais cobrados
✅ Súmulas e OJs do TST com maior incidência
✅ Simulado inédito com 60 questões no padrão FCC
Não é opinião. Não é achismo. É o que as provas mostraram.
R$ 27,90 — pagamento único, acesso imediato."

### Títulos do link nos anúncios
- Protocolo TRT — R$ 27,90

### Landing Page: Headline & Promessa Central
"PROTOCOLO trt — Análise estratégica completa das provas de TRT baseada em 46 provas reais de 23 tribunais. A ferramenta plug and play para quem quer estudar o certo, na dose certa, sem desperdiçar tempo."

### Seções da Landing Page (títulos, na ordem)
- R$ 27 ,90
- Tem alguma dúvida?
- Como vou receber esse conteúdo?

### Entregáveis / Formato (termos encontrados na LP)
- PDF
- Simulados


========================================

---
id_oferta: 062
anunciante: "LAP Engenharia"
url_destino: "https://www.facebook.com/61573091783749/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1941243637202247"
dias_ativo: 46
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
primeira_coleta_propria: "2026-10-11"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Mais agilidade e menos custos para seus projetos solares.
🚀 +2.000 projetos aprovados, garantindo processos rápidos e seguros.
📑 Reduza o tempo gasto com burocracia e aumente suas entregas.
✔ Cuidamos de TRT, projeto e homologação na COPEL de forma eficiente.
💰 A partir de R$ 250,00 por projeto.
📞 Converse com nossa equipe e veja como podemos ajudar: (44) 98829-8803
LAP Engenharia Elétrica – Eficiência que gera resultados para integradores solares."

### Títulos do link nos anúncios
- api.whatsapp.com

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 063
anunciante: "Editora Instituto CDT"
url_destino: "https://editora.institutocdt.com.br/produto/libido-masculina-da-fisiologia-a-prescricao"
ad_library_url: "https://www.facebook.com/ads/library/?id=1345385987351355"
dias_ativo: 41
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
dias_distintos_coletado: 5
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
id_oferta: 064
anunciante: "Caderno do Aprovado - Materiais para Concursos"
url_destino: "https://lp.cadernodoaprovado.com/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1607407254411907"
dias_ativo: 33
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
dias_distintos_coletado: 5
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
id_oferta: 065
anunciante: "Pratique Concursos"
url_destino: "https://ti.pratiqueconcursos.com.br/fcti/main.html"
ad_library_url: "https://www.facebook.com/ads/library/?id=2307143873373354"
dias_ativo: 31
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

### Títulos do link nos anúncios
- Super Resumos para Concurso TRT

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
id_oferta: 066
anunciante: "Nação Jurídica com GGS Advogados Associados"
url_destino: "https://guimasilvadvogados.com.br/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1295807189831029"
dias_ativo: 20
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
dias_distintos_coletado: 5
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
id_oferta: 067
anunciante: "Verbo Carreiras Jurídicas"
url_destino: "https://api.whatsapp.com/send"
ad_library_url: "https://www.facebook.com/ads/library/?id=1098210225904481"
dias_ativo: 18
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
dias_distintos_coletado: 5
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
id_oferta: 068
anunciante: "GG Concursos"
url_destino: "https://ggconcursos.com.br/cursos/trt4/?cupom=GG-30"
ad_library_url: "https://www.facebook.com/ads/library/?id=1644945670619014"
dias_ativo: 16
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "tribunal regional do trabalho, trt4"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "imagem (1)"
botoes: "Comprar agora (1)"
precos_exibidos_na_lp: "R$ 9.000,00 | R$ 890,00 | R$ 483,00 | 12x de R$ 40 | R$ 16.000,00 | R$ 490,00 | 12x de R$ 74"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
id_oferta: 069
anunciante: "Escola Até a Aprovação Policiais"
url_destino: "https://www.facebook.com/eaapoliciais/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1837036453960474"
dias_ativo: 11
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
dias_distintos_coletado: 4
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
id_oferta: 070
anunciante: "Vinco Leilões"
url_destino: "https://www.facebook.com/61575191932532/"
ad_library_url: "https://www.facebook.com/ads/library/?id=4069762199991599"
dias_ativo: 11
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
dias_distintos_coletado: 4
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
id_oferta: 071
anunciante: "vamos.falardireito"
url_destino: "http://preceder.com.br/inscreva/"
ad_library_url: "https://www.facebook.com/ads/library/?id=871645662605057"
dias_ativo: 11
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
dias_distintos_coletado: 4
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
id_oferta: 072
anunciante: "oliberal.com"
url_destino: "https://www.facebook.com/oliberal/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1154864303742580"
dias_ativo: 9
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tribunal regional do trabalho, tecnico judiciario"
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

---
id_oferta: 073
anunciante: "Hugo de Freitas"
url_destino: "https://www.facebook.com/hugoconcursos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=966783753153359"
dias_ativo: 9
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tribunal regional do trabalho, trt8"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno, Cronograma / plano de estudos"
formatos_dos_anuncios: "carrossel (1)"
botoes: "sem botão (1)"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"SAIU O EDITAL DO TRT8!
O Tribunal Regional do Trabalho da 8ª Região (Pará e Amapá) publicou hoje o edital para Técnico e Analista Judiciário, com salários de R$ 9.776 a R$ 16.040.
⚠️ Atenção: o concurso é para cadastro de reserva, Técnico agora exige nível superior, e o pedido de isenção da taxa fecha em 09/10.
São pouco mais de 100 dias até a prova. Dá tempo, mas só pra quem começar com plano.
💬 Comenta TRT que eu te mando o link do cronograma de 80 dias feito pra Técnico e Analista do TRT8.
📌 Salva pra não perder os prazos e marca quem vai prestar com você!
#concursoTRT8 #TRT8 #concursospublicos #concurseiros #tecnicojudiciario #analistajudiciario #FCC #concursopara #concursoamapa #justicadotrabalho #editalpublicado #hugoconcursos"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 074
anunciante: "123passei"
url_destino: "https://www.facebook.com/123PasseiOficial/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1806870927394954"
dias_ativo: 9
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, tribunal regional do trabalho, trt8"
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Material em PDF / apostila / caderno"
formatos_dos_anuncios: "carrossel (1)"
botoes: "sem botão (1)"
primeira_coleta_propria: "2026-10-10"
dias_distintos_coletado: 2
heuristica_preliminar_funil: "Misto / Não Determinado"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps: []
---
### Copy do Anúncio (Gancho de Entrada)
"Saiu o edital do TRT-8!
O Tribunal Regional do Trabalho da 8ª Região (Pará e Amapá) publicou o edital para técnico e analista judiciário. A banca é a FCC.
São 107 dias até a prova. Dá tempo de se preparar mesmo trabalhando, desde que você estude o que a FCC realmente cobra.
Quer se preparar uma vez só para o TRT-8 e para os próximos TRTs? Comenta TRT que a gente te manda o link do Do Zero aos TRT's no direct. 👇
#concursoTRT8 #TRT8 #concursospublicos #concurseiro #TRT #tecnicojudiciario #analistajudiciario #FCC #concursoPará #concursoAmapá #123passei"

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 075
anunciante: "Professor José Maria"
url_destino: "https://pergunteaoze.com.br/ebook-fcc-trt8"
ad_library_url: "https://www.facebook.com/ads/library/?id=1770480800743678"
dias_ativo: 8
anuncios_coletados: 1
anuncios_ativos_estimados: 1
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: sim
termos_foco_encontrados: "trt, trt8"
plataforma_checkout: "hotmart"
ticket_principal: "R$ 259,90"
fonte_ticket: "checkout"
tipos_produto: "Material em PDF / apostila / caderno, Questões / simulados, Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (1)"
botoes: "Baixar (1)"
precos_exibidos_na_lp: "R$ 259,90 | 12x de R$ 26,88 | R$ 322,56"
primeira_coleta_propria: "2026-10-11"
dias_distintos_coletado: 1
heuristica_preliminar_funil: "Venda Direta (Checkout)"
heuristica_nicho_estimado: "Tribunais (Poder Judiciário)"
order_bumps:
  - nome: "Questões do Zé - Treine Língua Portuguesa para"
    valor: "R$ 9,90"
  - nome: "Pergunte ao Zé: sua dúvida de Português resolvida"
    valor: "R$ 19,90"
---
### Copy do Anúncio (Gancho de Entrada)
"🚨 EDITAL PUBLICADO! O concurso do TRT 8ª Região (banca FCC) está confirmado, com prova em 17 de janeiro de 2027.
Comece sua preparação agora com o e-book gratuito: 60 questões comentadas de Língua Portuguesa da FCC, com raio-X da banca, dicas de prova e fundamentação teórica.
Baixe grátis 👇"

### Títulos do link nos anúncios
- EDITAL PUBLICADO! E-book grátis: 60 questões FCC – TRT 8ª Região

### Landing Page: Headline & Promessa Central
"Português do ZERO para concursos. — Comece hoje: 12 meses de acesso para construir sua base."

### Entregáveis / Formato (termos encontrados na LP)
- PDF
- Questões comentadas
- Simulados
- Videoaulas


========================================

# Parte 2 — Ofertas adjacentes (76)

Apareceram nas buscas, mas não citam os termos do foco. Servem para comparar formatos e preços de outros nichos de concurso; algumas não são de concurso.

---
id_oferta: 076
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
id_oferta: 077
anunciante: "Sou Concurseiro"
url_destino: "https://www.facebook.com/souconcurseiroevoupassaroficial/"
ad_library_url: "https://www.facebook.com/ads/library/?id=28548012774864327"
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
- Cada vez mais gente com 40, 50 anos está estudando para o TJ-AM: salário acima de R$ 15 mil e jornada das 8h às 14h.
- Salário de nível superior no TJ-AM: R$ 14.240 + R$ 2.660 de auxílio-alimentação = R$ 16.900 por mês.
- Requisitos do concurso do TJ-AM: não tem limite de idade e, para analista, vale qualquer curso superior, inclusive tecnólogo.
- Acabou a faculdade ou vai se formar este ano? O concurso do TJ-AM pode ser o seu próximo passo.
- As disciplinas que você já pode começar a estudar para o concurso do TJ-AM.
- Qualquer curso superior, salário acima de R$ 15 mil e jornada das 8h às 14h: esse é o concurso do TJ-AM.

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 078
anunciante: "EnfConcursos"
url_destino: "https://www.preparaenfermagem.com.br/cursos/curso-de-enfermagem-para-concursos/?utm_source=face_ads&utm_medium=%7B%7Bcampaign.name%7D%7D&utm_campaign=quente&utm_content=%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1600336774097728"
dias_ativo: 895
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
dias_distintos_coletado: 4
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
id_oferta: 079
anunciante: "Caminho da Perícia"
url_destino: "https://lp.vagasjustica.com.br/wpai/diario/engcivil/c?utm_source=meta_%7B%7Bsite_source_name%7D%7D&utm_medium=cpc_%7B%7Bplacement%7D%7D&utm_campaign=%7B%7Bcampaign.id%7D%7D_%7B%7Bcampaign.name%7D%7D&utm_content=%7B%7Badset.id%7D%7D_%7B%7Badset.name%7D%7D&utm_term=%7B%7Bad.id%7D%7D_%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=977290245399124"
dias_ativo: 33
anuncios_coletados: 4
anuncios_ativos_estimados: 16
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "vídeo (1), imagem (3)"
botoes: "Saiba mais (4)"
precos_exibidos_na_lp: "R$ 6.800,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
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
"Engenheiro Civil , seja um perito temporário e ganhe em média R$6.800,00 por mês. — Participe do treinamento gratuito e conquiste sua independência financeira:"

### Seções da Landing Page (títulos, na ordem)
- Informe seu nome e telefone para concluir a inscrição

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 080
anunciante: "Caminho da Perícia"
url_destino: "https://lp.vagasjustica.com.br/wpg/diario/pedagogo/c?utm_source=meta_%7B%7Bsite_source_name%7D%7D&utm_medium=cpc_%7B%7Bplacement%7D%7D&utm_campaign=%7B%7Bcampaign.id%7D%7D_%7B%7Bcampaign.name%7D%7D&utm_content=%7B%7Badset.id%7D%7D_%7B%7Badset.name%7D%7D&utm_term=%7B%7Bad.id%7D%7D_%7B%7Bad.name%7D%7Dl"
ad_library_url: "https://www.facebook.com/ads/library/?id=2116002109306739"
dias_ativo: 33
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
precos_exibidos_na_lp: "R$ 6.800,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
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
"Mais de 3.000 vagas de Perito Temporário para Pedagogos em 2026, receba em média R$6.800,00 por mês. — Reunião AO VIVO, GRATUITA E ON-LINE"

### Seções da Landing Page (títulos, na ordem)
- Informe seu nome e telefone para concluir a inscrição

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 081
anunciante: "Caminho da Perícia"
url_destino: "https://lp.vagasjustica.com.br/wpj/diario/veterinario/c?utm_source=meta_%7B%7Bsite_source_name%7D%7D&utm_medium=cpc_%7B%7Bplacement%7D%7D&utm_campaign=%7B%7Bcampaign.id%7D%7D_%7B%7Bcampaign.name%7D%7D&utm_content=%7B%7Badset.id%7D%7D_%7B%7Badset.name%7D%7D&utm_term=%7B%7Bad.id%7D%7D_%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1093091443660080"
dias_ativo: 33
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
formatos_dos_anuncios: "imagem (3)"
botoes: "Saiba mais (3)"
precos_exibidos_na_lp: "R$ 6.800,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
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
"Mais de 3.000 vagas de Perito Temporário para Veterinários em 2026, receba em média R$6.800,00 por mês. — Participe do treinamento gratuito e conquiste sua independência financeira:"

### Seções da Landing Page (títulos, na ordem)
- Informe seu nome e telefone para concluir a inscrição

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 082
anunciante: "Caminho da Perícia"
url_destino: "https://lp.vagasjustica.com.br/wpj/diario/engagro/c?utm_source=meta_%7B%7Bsite_source_name%7D%7D&utm_medium=cpc_%7B%7Bplacement%7D%7D&utm_campaign=%7B%7Bcampaign.id%7D%7D_%7B%7Bcampaign.name%7D%7D&utm_content=%7B%7Badset.id%7D%7D_%7B%7Badset.name%7D%7D&utm_term=%7B%7Bad.id%7D%7D_%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=1035758079287242"
dias_ativo: 33
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
formatos_dos_anuncios: "vídeo (1), imagem (2)"
botoes: "sem botão (1), Saiba mais (2)"
precos_exibidos_na_lp: "R$ 6.800,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 4
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
"Engenheiro Agrônomo , seja um perito temporário e ganhe em média R$6.800,00 por mês. — Participe do treinamento gratuito e conquiste sua independência financeira:"

### Seções da Landing Page (títulos, na ordem)
- Informe seu nome e telefone para concluir a inscrição

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 083
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
id_oferta: 084
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
dias_distintos_coletado: 5
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
id_oferta: 085
anunciante: "Clube do Perito"
url_destino: "https://lp.vagasjustica.com.br/wpj/diario/fisioterapeuta/c?utm_source=meta_%7B%7Bsite_source_name%7D%7D&utm_medium=cpc_%7B%7Bplacement%7D%7D&utm_campaign=%7B%7Bcampaign.id%7D%7D_%7B%7Bcampaign.name%7D%7D&utm_content=%7B%7Badset.id%7D%7D_%7B%7Badset.name%7D%7D&utm_term=%7B%7Bad.id%7D%7D_%7B%7Bad.name%7D%7D"
ad_library_url: "https://www.facebook.com/ads/library/?id=2113813649227282"
dias_ativo: 18
anuncios_coletados: 2
anuncios_ativos_estimados: 8
anuncios_com_baixo_volume_de_impressoes: 0
sinal_tracao: "médio"
foco_direto: não
termos_foco_encontrados: ""
plataforma_checkout: "Não detectada"
ticket_principal: "Não confirmado"
fonte_ticket: "nenhuma (checkout não lido)"
tipos_produto: "Isca gratuita / grupo VIP"
formatos_dos_anuncios: "imagem (2)"
botoes: "sem botão (2)"
precos_exibidos_na_lp: "R$ 6.350,10"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
id_oferta: 086
anunciante: "Decorando a Lei Seca Cursos Para Concursos E OAB"
url_destino: "https://www.facebook.com/decorandoaleisecaconcursoseoab/"
ad_library_url: "https://www.facebook.com/ads/library/?id=792696320220760"
dias_ativo: 189
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
formatos_dos_anuncios: "carrossel (2), vídeo (1), imagem (3)"
botoes: "Visitar perfil do Instagram (2), sem botão (4)"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
- O art. 319 do Código Penal caiu no concurso para Promotor do MP-GO!
- EDITAL PUBLICADO: TRT-8ª REGIÃO (PA/AP)
- ⚠️ Uma palavra pode mudar completamente o gabarito da questão.
- O Código Penal usa a mesma técnica de redação em dois artigos diferentes, e as bancas cobram a diferença exatamente do mesmo jeito.
- O art. 6º da Lei 14.133/2021 é, hoje, um dos dispositivos mais cobrados em concursos públicos. Só em provas da FGV e do CEBRASPE, já apareceu mais de 40 vezes.

### Landing Page: Headline & Promessa Central
"Destino direto para canal social / WhatsApp"

### Entregáveis / Formato (termos encontrados na LP)
- [nenhum termo conhecido encontrado]


========================================

---
id_oferta: 087
anunciante: "Matheus Santos - Eu concursado"
url_destino: "https://seraprovado.com/mentoria-matheussantos/"
ad_library_url: "https://www.facebook.com/ads/library/?id=1059387566661056"
dias_ativo: 75
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
dias_distintos_coletado: 5
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
id_oferta: 088
anunciante: "Eccos Cursos"
url_destino: "https://eccosedu.com/laser-transdermico/"
ad_library_url: "https://www.facebook.com/ads/library/?id=2426372244512830"
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
tipos_produto: "Curso em videoaulas"
formatos_dos_anuncios: "imagem (1), carrossel (2)"
botoes: "Saiba mais (3)"
precos_exibidos_na_lp: "R$ 9.900,00 | R$ 22.852,00"
primeira_coleta_propria: "2026-10-07"
dias_distintos_coletado: 5
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
id_oferta: 089
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
id_oferta: 090
anunciante: "Milena Correia Advocacia"
url_destino: "https://api.whatsapp.com/send"
ad_library_url: "https://www.facebook.com/ads/library/?id=1625294329172426"
dias_ativo: 26
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
dias_distintos_coletado: 5
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

## Demais adjacentes (resumo)

| id | Anunciante | Dias | Anúncios | Tração | Ticket (checkout) | Destino |
|---|---|---|---|---|---|---|
| 091 | GG Concursos | 11 | 3 | médio | Não confirmado | https://ggconcursos.com.br/cursos/gg-play/gg-play-vitalicio-360 |
| 092 | Sou Concurseiro | 9 | 3 | médio | Não confirmado | https://fabiomsam-cloud.github.io/sou-webinario-52b91323/?w=tjam |
| 093 | Noticiou | 8 | 3 | médio | Não confirmado | https://linkdehoje.online/conteudo-exclusivo/ |
| 094 | Concursos Ceisc | 194 | 2 | médio | Não confirmado | https://ceisc.com.br/cursos/2067-concurso-tj-sp-club-oficial-de-justica?utm_sour |
| 095 | Pódio Tribunais | 174 | 2 | médio | Não confirmado | https://api.whatsapp.com/send |
| 096 | Felipe Sgarbossa Advocacia Criminal | 169 | 2 | médio | Não confirmado | https://www.facebook.com/felipesgarbossa/ |
| 097 | Prof.carlosgoncalves | 124 | 2 | médio | Não confirmado | https://typebot.co/plataformaanalistadetribunais |
| 098 | Tjteiros | 100 | 2 | médio | Não confirmado | https://www.facebook.com/61582438800580/ |
| 099 | Estratégia Concursos | 87 | 2 | médio | Não confirmado | https://www.facebook.com/EstrategiaConcursos/ |
| 100 | Ludy Sena | 86 | 2 | médio | Não confirmado | https://www.facebook.com/ludysena.perita/ |
| 101 | LH no pódio | 80 | 2 | médio | Não confirmado | https://typebot.co/mentoria-zeroaopodio |
| 102 | Venâncio & Delgado - Advogados | 61 | 2 | médio | Não confirmado | https://api.whatsapp.com/send |
| 103 | Venâncio & Delgado - Advogados | 61 | 2 | médio | Não confirmado | https://www.facebook.com/venancioedelgadoadvogados/ |
| 104 | Jus Expert | 48 | 2 | médio | R$ 997,00 | https://pages.jusexpert.com/vsl-grafotecnica-principal |
| 105 | Lucas Viégas | 47 | 2 | médio | Não confirmado | https://foconocontrole.com.br/ |
| 106 | Comunidade de Aprovados com Helena Emerick Abaurre | 46 | 2 | médio | Não confirmado | https://form.respondi.app/9QZkseoW |
| 107 | Academia do Perito | 25 | 2 | médio | R$ 497,00 | https://lp.academiadoperito.com/peju-dor?utm_source=facebook&utm_medium=paid&utm |
| 108 | Estudo e Memorização | 20 | 2 | médio | Não confirmado | https://estudomemorizacao.com.br/pv-video-v2/ |
| 109 | Prof. Ronaldo Santos | 11 | 2 | médio | Não confirmado | https://rslinguaportuguesa.com/aplicacao-fgv/?utm_source=facebook&utm_medium=cpc |
| 110 | IPOG - Pernambuco | 8 | 2 | médio | Não confirmado | https://ipog.edu.br/cursos/pos-graduacao/avaliaces-e-pericias-de-engenharia-pos- |
| 111 | Delta Fabio Silva | 8 | 2 | médio | Não confirmado | https://www.facebook.com/deltafabiosilva/ |
| 112 | Flávio Britto Advocacia | 8 | 2 | médio | Não confirmado | https://www.facebook.com/flaviobrittoadvocacia/ |
| 113 | Projeto Caveira | 328 | 1 | médio | Não confirmado | https://www.facebook.com/projetocaveiraprf/ |
| 114 | Concursos Ceisc | 194 | 1 | médio | Não confirmado | https://ceisc.com.br/cursos/2070-concurso-tj-ba-analista-judiciario-area-judicia |
| 115 | Ceisc Concursos | 181 | 1 | médio | Não confirmado | https://lp.ceisc.com.br/evento-concursos-nivel-medio/ |
| 116 | Gaby no Tribunal | 178 | 1 | médio | Não confirmado | https://www.facebook.com/100090566482087/ |
| 117 | Discursiva na Prática | 129 | 1 | médio | R$ 1.489,00 | https://discursivanapratica.com.br/assinaturacontrole/?utm_source=facebook&utm_m |
| 118 | Douglas Prado - Servidor 30k | 106 | 1 | médio | Não confirmado | https://odouglasprado.com.br/plano-servidor-30k/ |
| 119 | Fauth e Freitas Sociedade de Advogados com Adriane Fauth | 95 | 1 | médio | Não confirmado | https://www.facebook.com/61573224123970/ |
| 120 | mamae_concurseira6 com Decorando a Lei Seca Cursos Para Concursos E OAB | 88 | 1 | médio | Não confirmado | https://www.decorandoaleiseca.com.br/ |
| 121 | Atleta dos Concursos | 86 | 1 | médio | Não confirmado | https://atletadosconcursos.com.br/kit-aprovacao-enam/?sck=facebook%7Cads%7Cconve |
| 122 | Brabo Editora | 86 | 1 | médio | R$ 397,00 | https://braboeditora.com.br/mestre-em-questoes-tjsp-v8/ |
| 123 | Professor Rodrigo Marengo - Consultor Legislativo do Senado Federal aos 24 | 81 | 1 | médio | Não confirmado | https://ataticadaaprovacao.com.br/ |
| 124 | Mege | 69 | 1 | médio | Não confirmado | https://concurcity.mege.com.br/explorar |
| 125 | Themas Cartórios | 67 | 1 | médio | Não confirmado | http://www.themas.com.br/ |
| 126 | cristinedentista | 62 | 1 | médio | Não confirmado | https://www.facebook.com/cristinedentista/ |
| 127 | alineperitasocial | 61 | 1 | médio | Não confirmado | https://www.instagram.com/_u/alineperitasocial |
| 128 | Concurseiro Fora da Caixa | 60 | 1 | médio | Não confirmado | https://concurseiroforadacaixa.com.br/collections/todos-os-materiais |
| 129 | Professora Amanda Aires | 57 | 1 | médio | Não confirmado | https://www.amandaaires.com.br/curso/%5B2026%5D-economia-para-o-tcu/345 |
| 130 | Rô Santtana - OAB | 54 | 1 | médio | Não confirmado | https://rosanttana.com.br/captacao/lp-discursiva-oab.html |
| 131 | Rhema Lab com Rodrigo Noronha | 53 | 1 | médio | Não confirmado | https://rhemalab.com.br/ |
| 132 | Concursos Ceisc | 53 | 1 | médio | Não confirmado | https://www.sympla.com.br/produtor/ceisc |
| 133 | emanuellasouza.adv | 52 | 1 | médio | Não confirmado | https://www.instagram.com/_u/emanuellasouza.adv |
| 134 | Advogado de concurso | 48 | 1 | médio | Não confirmado | https://olivaesouza.com.br/tjsc-objetiva-nivel-superior-conhecimentos-gerais/ |
| 135 | Jus Expert | 46 | 1 | médio | R$ 997,00 | https://pages.jusexpert.com/vsl-papiloscopia-principal |
| 136 | Capriata Educação | 46 | 1 | médio | Não confirmado | https://capriatacursos.com.br/produto/preparatorio-banco-do-brasil/ |
| 137 | Prof. Herbert Almeida | 26 | 1 | médio | Não confirmado | https://herbertalmeida.com.br/mentoria-cgu/ |
| 138 | Memorização Bruno Campos Concursos | 24 | 1 | médio | Não confirmado | https://www.facebook.com/100088833677510/ |
| 139 | Marco Cursos Preparatórios | 16 | 1 | médio | Não confirmado | https://www.facebook.com/marcocursos/ |
| 140 | Pedro Auar Advocacia | 12 | 1 | médio | Não confirmado | https://www.facebook.com/pedroauar/ |
| 141 | Paulo Afonso Advocacia | 12 | 1 | fraco | Não confirmado | https://www.facebook.com/61582851535500/ |
| 142 | Professora Fernanda Barboza | 11 | 1 | médio | Não confirmado | https://hml.fernandabarboza.com.br/2026/09/16/dt-black-friday-antecipada-vsl/ |
| 143 | Bref: Direito Empresarial | 10 | 1 | médio | Não confirmado | https://metodobref.com.br/?utm_source=instagram&utm_medium=paid&utm_campaign=tjp |
| 144 | Êutika Assessoria Empresarial | 10 | 1 | médio | Não confirmado | https://www.facebook.com/61556190747058/ |
| 145 | Marcelomapas | 9 | 1 | médio | R$ 17,00 | https://resumosmapasdireito.com/constitucional/ |
| 146 | Carreiras Educação com Professor Jobson Castelo Branco | 9 | 1 | médio | Não confirmado | https://www.facebook.com/61572024614383/ |
| 147 | Helena Emerick Abaurre com Comunidade de Aprovados | 9 | 1 | médio | Não confirmado | https://pay.plataformatutory.com.br/checkout/af51c9d5-01c3-4988-8e18-2fd62561f10 |
| 148 | Aprovando Concurseiro | 9 | 1 | médio | R$ 57,99 | https://pay.hotmart.com/M107002055F?checkoutMode=10 |
| 149 | Uniforenses Instituto de Pericias Forenses | 8 | 1 | médio | R$ 197,00 | https://nomeacao2.uniforenses.com.br/ |
| 150 | Gran Cursos Online - Concursos Públicos | 8 | 1 | médio | Não confirmado | https://www.grancursosonline.com.br/cursos/por-concurso/sme-itaborai-rj-sme-itab |
| 151 | Giovana reserva | 8 | 1 | médio | Não confirmado | https://www.facebook.com/61572043193487/ |

# Apêndice — Descartadas por não citarem concurso (170)

Vieram nas buscas (ex.: escritórios que citam o TRF como tribunal), mas o texto não tem nenhum termo de concurso. Confira se algo relevante caiu aqui por engano.

| Anunciante | Dias | Destino |
|---|---|---|
| Ato psicologia psicoterapias psicodrama e desenvolvimento humano | 145 | https://api.whatsapp.com/send |
| Reviva | 32 | https://renuva.com.br/pages/drenagem-linfatica |
| SERV FONE | 102 | https://www.facebook.com/servfone.servfone/ |
| EBM Goiás | 99 | http://fb.me/ |
| Godri Domingues Advocacia | 60 | https://www.facebook.com/godridomingues/ |
| Renuva | 11 | https://renuva.com.br/pages/drenagem-linfatica |
| Morrowfen Drama | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Rita Bervig | 181 | https://www.facebook.com/100091834883862/ |
| Danielle Bartoly | 173 | https://www.facebook.com/61577922862090/ |
| Aqui Tem Plano de Saúde | 66 | http://fb.me/ |
| Visão Química do Brasil | 60 | http://fb.me/ |
| Sementes Biomatrix | 59 | https://www.youtube.com/watch?v=CWapR4E8Kdo |
| Precatorial | 57 | http://fb.me/ |
| Dr. Vinicius Valença com Doutor Vinicius Valença | 46 | https://efs3sfec7ia.pro.typeform.com/HPM1125?utm_source=xxxxx&utm_medium=xxxxx&u |
| Carlos Klein - Personal | 23 | https://oficialbarrigazero.protocolocarlos.com.br/quizz |
| Gabriella Ibrahim | 11 | https://www.facebook.com/gabriellathomasibrahim/ |
| Driftmere Chronicles | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Segredos de Um Coração Distante | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Dra. Gabriela Madeira | 13 | https://api.whatsapp.com/send |
| ShopRootvana | 13 | https://tryrootvana.com/pages/listicle-2 |
| Comunidade Milhorin | 9 | https://www.facebook.com/milhorincalculos/ |
| Dravelle | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Northwillow Stories | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| KK drama | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Moonharbor Tales | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Dreamwick Scenes | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Elvoria | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Rastros Deixados por um Mistério | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Dr Bruno Guerra | 129 | https://www.facebook.com/61566645860434/ |
| Hematix - Hematite Bracelet | 128 | https://myhematix.com/products/hematix-strength-band?view=strength-story |
| Agroborges | 90 | https://www.facebook.com/agroborgesjp/ |
| Clinica Osmilto Brandão | 75 | https://www.facebook.com/100093106637344/ |
| Flat & Hotel Executive | 68 | https://www.facebook.com/61584218885791/ |
| Prática e Pós CEISC | 67 | https://ceisc.com.br/categorias/pos-graduacao |
| ShopVantique | 61 | https://shopvantique.com/products/vantique-nad-supplement-for-men |
| Andrew Martin - Health & Performance Advisor | 60 | https://assess.secondprime.io/ |
| TSTemdia | 58 | https://lp.tstemdia.com.br/ |
| Heraclio Cunha | 54 | https://peritoem7dias.com.br/ |
| Bience Agriscience | 53 | https://www.facebook.com/bience.ag/ |
| JB Advocacia | 51 | https://janainabaptista.adv.br/ |
| Rafael Amaral Adv | 32 | https://api.whatsapp.com/send |
| Fernanda Diniz | 32 | https://renuva.com.br/pages/drenagem-linfatica?mlid=lead_20261011_alt1h15ayin&sr |
| ShopRootvana | 28 | https://tryrootvana.com/products/rootvana-l-carnitine-4000mg-liquid-spanish?utm_ |
| Verbo Carreiras Jurídicas | 18 | https://chat.whatsapp.com/Bsvp30MtbOTI4HDJuoMz89?mode=hqrt2 |
| Sport Motors | 13 | https://api.whatsapp.com/send |
| Iridium Labs | 13 | https://www.iridiumlabs.com.br/products/zeus-extreme-pre-hormonal-60-comps |
| Doseprimal Brasil | 11 | https://doseprimal.com/pages/doseprimalt |
| Dr. Rafael Monteiro - Naturopata | 10 | https://renuva.com.br/pages/drenagem-linfatica |
| Hellena Araújo Corretora de Imóveis - CRECI 4048-F | 10 | https://api.whatsapp.com/send |
| Vellora Flicks | 9 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Mentoria Tribunal do Trabalho | 8 | https://black.professoreduardojose.com.br/inscricao |
| Larkstone Tales | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Aurelmere Stories | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Everlune Drama | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Velmique | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Páginas de Um Amor Perdido | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Destinos Marcados por um Segredo | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Boutique dos presentes SP | 368 | https://wa.me/message/V2IWS5YXCDZ4E1 |
| Clínica Ninho | 267 | https://www.facebook.com/clinicaninho/ |
| Juri Digital | 159 | https://www.facebook.com/juridigitalcombr/ |
| CAEPE - Centro Avançado de Estudos Periciais com Erotilde Minharro | 155 | https://caepe.com.br/ |
| Thiago Raso | 153 | https://www.facebook.com/61556940472092/ |
| Alibaba.com | 152 | https://www.alibaba.com/product-detail/haoge_1600937628295.html?src=cpm_fb&sub_c |
| Alibaba.com | 152 | https://www.alibaba.com/product-detail/haoge_10000022888175.html?src=cpm_fb&sub_ |
| Editora Mizuno | 144 | https://www.editoramizuno.com.br/ |
| Bruto Brasil | 131 | https://www.youtube.com/watch?v=S9fODqC2kkw&feature=youtu.be |
| Douglas Prado - Servidor 30k com Servidores High Level | 127 | https://www.facebook.com/professorlucrativo/ |
| Piresvillelaadvocacia | 123 | https://www.facebook.com/100075926929857/ |
| Dental Speed | 121 | https://www.dentalspeed.com/carregador-universal-fotopolimerizador-elipar-deepcu |
| Perville Construtora | 116 | https://www.facebook.com/PervilleConstrutora/ |
| LeClinic Odontologia | 115 | https://www.facebook.com/leclinicodontologia/ |
| Jerônimo E-Lance | 113 | https://www.facebook.com/jeronimodosleiloes/ |
| TSTemdia | 112 | https://www.facebook.com/61581193663516/ |
| Advocacia Miqueias Oliveira | 108 | https://www.facebook.com/61585245201416/ |
| 42pericias | 105 | https://www.42pericias.com.br/ |
| Duarte Advogados Associados | 104 | https://www.facebook.com/61555624388490/ |
| JQM Advocacia Especializada | 103 | https://www.facebook.com/61561436444397/ |
| Mitsubishi Motors Brasil | 100 | https://www.mitsubishimotors.com.br/picapes/nova-triton?utm_source=facebook&utm_ |
| Fibra Pará | 97 | https://www.facebook.com/fibrapara/ |
| Dr. Kegel: For Men’s Health & Wellness | 96 | https://quiz.kegel-plan.me/pt-br/?cmpid=67b757a235e0d329de693d90&sub1=%7B%7Bad.i |
| pilateshiitflow com Riven Fitness for Life | 94 | https://www.instagram.com/_u/pilateshiitflow |
| Carreira de Perito | 91 | https://carreiradeperito.com.br/ |
| OAB Subseção Atibaia | 89 | https://api.whatsapp.com/send |
| IBCCRIM | 86 | https://jcc.ibccrim.org.br/ |
| Madervillas Madeireira . Lauro de Freitas | 79 | https://www.facebook.com/61577737911934/ |
| Start Electric - Instalação e Manutenção Elétrica | 76 | https://www.facebook.com/startelectric31/ |
| VCA Construtora e Incorporadora | 75 | http://fb.me/ |
| Instituto Doutrina Policial 2 | 74 | http://fb.me/ |
| Gestaodeclinica | 74 | https://minhaclinicamilionaria.com.br/?utm_source=facebook&utm_medium=cpc&utm_ca |
| Dr. Jordan Seabra de Oliveira - Advogado Trabalhista | 69 | https://www.facebook.com/61590618007101/ |
| UNDB Imperatriz | 69 | http://fb.me/ |
| Prompt8 AI | 69 | https://jusquant.ai/?utm_source=meta&utm_medium=paid_social&utm_campaign=trab_up |
| Diego Filipe Tulio com Grand Mercure Pinheiros | 68 | https://www.facebook.com/100083362727382/ |
| Caravella's Culinária Regional | 68 | https://www.facebook.com/caravellasculinaria/ |
| Servita Clinic | 68 | https://www.facebook.com/61582841670718/ |
| Gil Fernandes | 67 | https://www.facebook.com/gilfernandes01/ |
| Luiz Guedes | 67 | https://www.facebook.com/100068780851308/ |
| Advocacia com advogada_rosane_castro | 66 | https://www.facebook.com/61586164577697/ |
| prof.eduardowaga | 65 | https://www.facebook.com/prof.eduardowaga/ |
| DramaBox - short drama2 | 63 | https://play.google.com/store/apps/details?id=com.storymatrix.drama |
| DramaBox - short drama1 | 63 | https://play.google.com/store/apps/details?id=com.storymatrix.drama |
| Juanita Restaurante | 62 | https://www.facebook.com/juanitarestaurante/ |
| Fernandez Pollito Advocacia | 61 | https://www.facebook.com/advocaciapollito/ |
| RAIR Silva | 60 | https://www.facebook.com/jornalistarairsilva/ |
| Viégas Filho | 60 | https://www.facebook.com/100094050184913/ |
| Judit | 59 | https://produto.judit.io/miner-precatorios |
| Aurora by Lidiane Kuhn | 59 | https://www.facebook.com/61590179524480/ |
| Sicredi Sementes do Sul | 58 | https://www.linkedin.com/uas/login?session_redirect=https%3A%2F%2Fwww.linkedin.c |
| thainara.assistentesocial | 58 | https://www.instagram.com/_u/thainara.assistentesocial |
| BLL Compras com Licitações Municipais. | 55 | https://www.facebook.com/BLLCOMPRAS/ |
| Gabriela Franco | 55 | https://www.facebook.com/61575028750782/ |
| AnotherVoid | 55 | https://anothervoid.co/products/liquid-l-carnitine-4000mg?variant=49141411283179 |
| Bruno Pesca & Turismo Corumbá | 54 | https://brunopescaturismo.com.br/ |
| Benvindoadv Professor com Benvindoadv Previdenciário | 54 | https://www.facebook.com/100095299025661/ |
| Inovajur Capacitação Jurídica e IA | 54 | https://inovajur.com/nova-pratica-vsl/?utm_source=Facebook_ads&utm_medium=%7B%7B |
| Avante | 54 | https://www.facebook.com/61572155530930/ |
| MB Comunidade | 53 | https://comunidademb.com/lista-de-espera/ |
| Go Kursos | 53 | https://www.gokursos.com/go-oab---direito-penal---2%C2%AA-fase-30553/p |
| Faloppa Advogados Associados | 51 | https://api.whatsapp.com/send |
| Grau Técnico Parnamirim | 51 | https://www.facebook.com/grautecnicoparnamirim/ |
| Dr. Paulo Cruz | 51 | https://www.facebook.com/61588916093349/ |
| Katarinhuk Advogados Associados | 48 | https://www.facebook.com/katarinhuk/ |
| Camila Batista l Advocacia e Consultoria Jurídica | 47 | https://www.facebook.com/61583704602407/ |
| Vidal - Advogados | 46 | https://api.whatsapp.com/send |
| Oliveira Marinho Advocacia com Dra. Marcelia Bruna | 46 | https://oliveiramarinho.com.br/ |
| Keylon Lucarelli - Nutrologia e Emagrecimento Saudável | 30 | https://www.facebook.com/100082746462251/ |
| ShopRootvana | 28 | https://tryrootvana.com/pages/listicle-1 |
| Muniz Auto Center Vitória da Conquista | 25 | https://www.facebook.com/munizvitoriadaconquista/ |
| Cellics Health | 24 | https://cellics.co/pages/appledroppers-2 |
| Experience True Nutra | 20 | https://truenutra.com/products/fb-en-us-mc001 |
| Alfa Viking | 19 | https://alfaviking.com.br/libi/ |
| Hospital Adventista de Belém | 19 | https://www.facebook.com/hospitalbelem/ |
| Morais Amaral Arquitetura | 18 | https://www.moraisamaral.arq.br/ |
| Vanguarda Visual Law | 17 | https://vanguardavisuallaw.com.br/kit-advocacia-trabalhista |
| Hormofy | 17 | https://hormofy.com/reposicao-hormonal/ |
| ANAJUSTRA Federal | 17 | http://fb.me/ |
| Benvindoadv Professor | 16 | https://www.facebook.com/100095299025661/ |
| True Nutra Plus | 15 | https://truenutra.com/products/fb-en-lc001 |
| Leandro Magalhães | 15 | https://www.facebook.com/AnalyticsBR/ |
| Congresso TEA RP com gialbuquerquesp | 13 | https://payfast.greenn.com.br/sdq5zr4 |
| MacPonta Caminhões | 12 | https://macpontacaminhoes.com.br/cada-km-conta/?utm_source=facebook&utm_medium=c |
| UroLages - Urologia Especializada | 11 | https://www.facebook.com/UroLages/ |
| Doctora Karito | 11 | https://trt.colorpack.online/ |
| Gracielle Lima Assessoria e Consultoria Jurídica | 10 | https://www.facebook.com/61585454075287/ |
| Tapai Advogados | 10 | https://www.facebook.com/TapaiAdvogados/ |
| Giselle Tapai | 10 | https://www.facebook.com/61588752251791/ |
| Monica Freitas MTE | 10 | https://www.facebook.com/61583807948841/ |
| brenomarxoficial | 10 | https://www.facebook.com/100081178312118/ |
| Daniel Garcia Leilões | 10 | https://danielgarcialeiloes.com.br/item/80027/detalhes?page=1 |
| Him+ Skin | 10 | https://himpluskin.com/pages/advertorial-lp |
| ResuNinja | 10 | https://www.resuninja.com/bonus |
| Daniella Costa Agro | 9 | https://www.facebook.com/61594331413710/ |
| samwelholandaadv | 9 | https://www.instagram.com/_u/samwelholandaadv |
| BSSP Centro Educacional | 9 | https://bsspce.com.br/pos-graduacao-e-mba/mba-pericia-contabil-economica-e-finan |
| Dr. Elpídio Donizetti | 9 | https://elpidiodonizetti.com.br/ |
| André Luiz Team | 9 | https://www.facebook.com/andreluizteam/ |
| robertalisboa1 | 9 | https://psirh.ditrafego.com/lp02/ |
| Professor Raphael Reis | 9 | https://www.professorraphaelreis.com.br/curso/estudo-de-caso-trt8-ajaj-e-ajoj/ |
| Dilma Nogueira Corretora | 8 | http://fb.me/ |
| Brunno Galvão Advogados Associados | 8 | https://www.facebook.com/61589060739230/ |
| PID Scanner | 8 | http://fb.me/ |
| NS-za-0926a | 8 | https://fb.netshort.com/netshort-h5-landing-page/wT2ZCAKTp2w.html?pid=metaweb_in |
| NS-za-0811B | 8 | https://fb.netshort.com/netshort-h5-landing-page/wT2wbOOXsO9.html?pid=metaweb_in |
| Ecos de um Encontro | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Suspiros da Memória | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Drama Urbano | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Segredos ao Entardecer | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| Histórias da Vida | 8 | https://www.freereelsw2a.com/ads/0/2157/view?c=%7B%7Bcampaign.name%7D%7D&af_adse |
| stevaogandh | 8 | https://www.facebook.com/100063782303724/ |
| JV TÉCNICO PERITO JUDICIAL | 8 | https://www.facebook.com/JV-T%C3%89CNICO-PERITO-JUDICIAL-752648911269348/ |
