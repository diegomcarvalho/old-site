---
title: Pandemia COVID-19
subtitle: Alguns resultados da pesquisa feita pelo grupo de biomatemática

# Summary for listings and search engines
summary: Nessa página, o de grupo de modelagem e inteligência computacional do Centro Federal de Educação Tecnologica Celso Suckow da Fonseca, composto pela Profa. Dayse Pastori, D.Sc, Prof. Rafael Barbastefano, D.Sc, Prof. Diego Carvalho, D.Sc., e Profa. Maria Clara Lippi, M.Sc., apresenta um súmário dos resultados da pesquisa que vem sendo feita sobre a Pandemia da COVID-19. Esses resultados não são definitivos e devem ser considerados com cuidado, pois são fruto de pesquisa ainda em desenvolvimento. O principal objetivo dessa divulgação é compartilhar rapidamente com os nossos pares para validação, sugestões e comentários. Um painel completo com todos os resultados intermediários pode ser encontrado no seguinte link.

# Link this post with a project
projects: []

# Date published
date: '2020-05-20T00:00:00Z'

# Date updated
lastmod: '2022-09-05T00:00:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: true

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: [**SENAI-CETIQI**](https://senaicetiqt.com/wp-content/uploads/2022/03/IC-1.jpg)'
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - admin

tags:
  - Academic

categories:
  - Research
  - Pesquisa
  - COVID
---
## Nas seções abaixo são apresentadas tópicos sobre o diário de pesquisa.

### Dia 17 de julho de 2020

De posse dos dados do Ministério da Saúde com diversos atributos dos pacientes testados com suspeita de COVID-19, fizemos uma verificação de alguns casos conhecidos para entender como os casos se apresentavam na base.

A verificação foi feita com a comparação de casos conhecidos. Por exemplo, procuramos a data de nascimento do presidente da república na base e tentamos encontrar algum paciente com diagnóstico positivo através do PCR em alguma data em torno da data real do exame. Nos três primeiros casos que procuramos, nós não encontramos correspondentes.

Como a base também apresenta pacientes com teste negativo, fizemos o mesmo procedimento com alguns exames negativos e também não encontramos nenhum deles na base.

Mesmo não tendo a expectativa de se encontrar um exame negativo na base, ficamos preocupados com a inexistência dos testes positivos que deveriam pertencer a base de dados do Ministério da Saúde, pois a notificação é obrigatória.

Com esse pano de fundo, fizemos a seguinte pergunta: qual seria a curva de notificação (casos diagnosticados) se levássemos em consideração a curva de óbitos. Ou seja, qual seria a curva de casos acumulados compatível com a curva de óbitos que temos. Essa pergunta se baseia na premissa que por causa da burocracia própria que existe na ocorrência do óbito, a notificação compulsória do óbito teria maior chance de acontecer.

Na figura abaixo, nós apresentamos dados do Ministério da Saúde, onde os óbitos acumulados no Rio de Janeiro estão marcados em em preto no gráfico e os casos diagnosticados acumulados em azul. Já a curva laranja mostra a estimativa do casos acumulados diagnosticados que teríamos no RJ quando utilizamos o nosso modelo da COVID-19. Nessa curva temos um indicativo que chegamos na quantidade de casos que temos hoje (2020/07/17) há 49 dias e que a escalada de casos foi muito mais íngrime do que mostrariam os dados.


![Figura1](Gnuplot.svg)
**Figura1**: Casos acumulados no Basil (fonte: Ministério da Saúde) e resultado do modelo SARS-Cov-2-EDO-BR com previsão de 7 dias.

Além disso, ficamos consternados com a decisão da Prefeitura Municipal do Rio de Janeiro em mudar a forma de contagem de óbitos na cidade. Felizmente, na manhã de hoje (28 de maio de 2020), recebemos a notícial que a Defensoria Pública conseguiu que a prefeitura revesse a sua posição. Essa decisão era preocupante, pois como podemos observar no gráfico abaixo, o Estado do Rio de Janeiro apresenta a maior taxa de conversão em óibtos induzida pela COVID-19 e o município do Rio tem grande peso nos óbtitos contabilizados.

![Figura2](EDO-PARAM.png)
**Figura2**: Gráfico com o dD taxa de conversão em óbitos induzida pela COVID-19 nos diagnosticados. Resultado do ajuste do modelo SARS-Cov-2-EDO-BR em 2020-05-27 nos dados dos estados brasileiros.

A taxa de conversão em óbitos induzida pela COVID-19 nos diagnosticados indica a velocidade que o grupo de diagnosticados vão a óbito e serve para avaliar os efeitos de políticas desenvolvidas por agentes públicos, principalmente no Brasil onde se testa menos que 0,5% da população. Por causa disso, os modelos matemáticos podem ser uma das únicas ferramentas disponíveis para se avaliar o resultado das ações governamentais.