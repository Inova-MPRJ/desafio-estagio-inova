# Desafio - Estágio em Análise de Dados - Inova_MPRJ 2020

Se você está visitando este repositório, provavelmente é porque foi selecionado(a) para a segunda fase do processo seletivo para a vaga de estágio em análise de dados no [Laboratório de Inovação do Ministério Público do Rio de Janeiro](http://www.mprj.mp.br/inova) (Inova_MPRJ). **Parabéns!**

A segunda fase consiste em um desafio com dados reais e um caso de uso parecido ao que você poderia encontrar no Laboratório. **Você terá uma semana para desenvolver o desafio**, a contar do disparo dos e-mails confirmando a sua classificação. 

Toda a informação que você precisa para saber por onde começar está descrita abaixo. **Leia com atenção**.


## O desafio

O desafio consiste em realizar uma análise exploratória sobre obras públicas paralisadas, a partir de dados públicos estruturados. Esse desafio é inspirado no projeto [Bússola _ Baía de Guanabara](http://www.mprj.mp.br/inova/baiaguanabara) (B_Guanabara), no qual o Inova_MPRJ trabalhou em parceria com os órgãos da área ambiental do MPRJ para monitorar o andamento das obras de despoluição da Baía de Guanabara.

Na maioria dos projetos que apoiamos, começamos sabendo muito pouco do assunto com o qual vamos trabalhar, e em poucas semanas precisamos aprender o suficiente para apontar o caminho de um protótipo robusto de solução. Neste desafio, queremos saber se você é capaz de fazer esse mergulho em um tema novo e, em poucos dias, propor visões pouco óbvias que orientem uma atuação baseada em dados para resolver problemas públicos.

No B_Guanabara, o desafio tem sido identificar quais das obras previstas tem mais chances de atrasar - e abrir os dados necessários para isso. Aqui, queremos que você faça o mesmo a partir de dados já abertos, relativos às [obras com recursos públicos do Governo Federal](http://plataformamaisbrasil.gov.br/sobre-a-plataforma). Não esperamos que você entregue um modelo preditivo completo, mas sim que seja capaz de manipular os dados, propor cruzamentos e indicadores e documentar o processo de pesquisa e desenvolvimento da solução.


## A entrega

### Conteúdo mínimo do repositório

Ao final de uma semana, você deverá entregar:

- As planilhas em formato *csv* com os resultados da sua análise;
- Um dicionário de variáveis (em formato *csv*, *xlsx* ou *ods*) com a descrição das variáveis nas planilhas que você gerou;
- Um arquivo README.md, em *markdown*, contextualizando o trabalho, apresentando os resultados, justificando as suas escolhas e documentando o processo de análise;
- Todo o código fonte (em qualquer linguagem) que você usou para realizar as análises.
- As visualizações produzidas, embutidas no *markdown* da documentação ou em um subdiretório **/img**, em formato *png*.
- Um arquivo de licença padrão que permita, no mínimo, o compartilhamento e a adaptação do material que você produziu.

Todo o conteúdo deve estar em um repositório público do GitHub, na conta apontada na sua inscrição. O nome e descrição do repositório devem fazer referência ao **Desafio - Estágio em Análise de Dados - Inova_MPRJ 2020**. Caso tenha apontado um portfólio em outra plataforma que não o GitHub, crie uma conta e entre em contato conosco [por e-mail](mailto:inova@mprj.mp.br) informando o seu nome e o endereço da conta criada.


### Conteúdo mínimo da análise

Do ponto de vista do conteúdo das análises, esperamos que você produza:

- Ao menos dois indicadores compostos (cruzamento de variáveis da base de dados original) que joguem luz sobre as perguntas **"Quais obras públicas atrasam? Quais os fatores associados a esse atraso?"**. *A escolha dos indicadores deve estar justificada na documentação da entrega*.
- Ao menos uma operação de filtragem (*subset*) de um subconjunto de interesse. **Dica**: estamos especialmente interessados em obras de saneamento no estado do Rio (em nível estadual e dos municípios), nos últimos cinco anos. Não precisa se fixar só nisso, mas, se não tiver outra ideia, pode usar como referência.
- Ao menos uma operação de agrupamento (*group by*) a partir dos valores em uma ou mais colunas. Você decide os grupos que acha que faz sentido (por período, por tipo de obra, por responsável, etc.), mas *mencione a escolha* na documentação.
- Ao menos uma operação de junção (*join*) entre planilhas ou estruturas de dados diferentes. **Dica**: provavelmente você vai precisar de mais de uma.
- Ao menos uma transformação de forma das planilhas ou estruturas de dados de coluna para linhas (*melt*/*wide to long*) OU de linhas para colunas (*pivot*/*long to wide*).
- Quantas análises você julgar necessárias e possíveis de fazer dos resultados das análises, usando estatísticas descritivas ou inferenciais, com os principais achados e possíveis interpretações.
- Ao menos um gráfico exploratório por indicador proposto. Não estamos interessados em grandes malabarismos de visualização de dados - tem um pessoal de design aqui justamente para ajudar com isso -, mas sim se você consegue propor formas de visualização que permitam enxergar tendências e flutuações para além do que as tabelas e as medidas estatísticas sozinhas possibilitam.


## Os dados

Os dados para a análise vêm da Plataforma +BRASIL, que disponibiliza diariamente *csv*s com informações das transferências voluntárias de recursos da União para os estados e municípíos. Todos os dados estão disponíveis para download [aqui](http://plataformamaisbrasil.gov.br/download-de-dados). No final da página, há os links com o modelo de dados e o dicionário de variáveis.

Opcionalmente, você pode trabalhar também com a [planilha de obras paralisadas do TCE-RJ](https://tcerj365-my.sharepoint.com/:x:/g/personal/rpsvc_tcerj365_onmicrosoft_com/EXVQpfiICt1FqHF1ETwNmJEBqJgv-8u0fRzPDz6MegGMxQ?rtime=bw1uly8o2Eg). Porém, essa planilha é menos rica em informações. Além disso, traz apenas as obras que estão paralisadas ou atrasadas - enquanto uma parte importante do desafio é identificar os fatores que separam as obras que atrasam das que são entregues no prazo (ou quase).


## A avaliação

Cada entrega será avaliada separadamente por duas pessoas do nosso time de dados. Cada um deles dará notas de 1 a 5 (1-muito ruim; 2-ruim; 3-ok; 4-bom; 5-muito bom) para duas dimensões:

- Código fonte e domínio técnico
    - Domínio de todas as [operações mínimas indicadas](https://github.com/Inova-MPRJ/desafio-estagio-inova/blob/master/README.md#conte%C3%BAdo-m%C3%ADnimo-da-an%C3%A1lise);
    - Qualidade do código (legibilidade, economia de código e processamento, melhores práticas do paradigma de programação adotado etc.);
    - Criatividade na seleção de agrupamentos, filtros e cruzamentos, e alinhamento deles com a pergunta central do desafio.

- Documentação e qualidade da análise
    - Qualidade da documentação para comunicar o processo de desenvolvimento de forma clara (inclusive para pessoas que não dominam a linguagem técnica);
    - Criatividade, rigor e alinhamento dos indicadores, das análises estatísticas e das visualizações propostas com a pergunta central do desafio;
    - Domínio de recursos de *markdown* para criar a documentação.

Essas notas serão somadas e divididas para uma média entre os dois revisores. Caso alguma dimensão apresente uma diferença de mais de 2 pontos entre os avaliadores, eles poderão conversar para chegar a um consenso.


## Perguntas (que achamos que serão as mais) frequentes

- Posso usar outros conjuntos de dados também?
**R:** Claro! Inclusive, vamos gostar de ver isso. Mas lembre-se de documentar de onde você tirou tudo. E cuidado para não fugir do tema, nem se perder em análises muito extensas.

- E se eu precisar conhecer mais sobre o tema?
**R:** *Descobre aê*. Tentamos manter um bom equilíbrio com os nossos estagiários entre dar o apoio que eles precisam e estimular a autonomia e a iniciativa de aprender coisas novas por si próprios. Valorizamos as questões (respondidas ou não) e os aprendizados que surgirem ao longo do processo - por isso, não deixe de documentá-las bem na sua entrega.
Em todo caso, se quiser um lugar por onde começar, não deixe de consultar a primeira parte da [seção "Boas práticas"](http://www.mprj.mp.br/documents/20184/1478516/index.html/#secao6), no relatório do B_Guanabara. Ali, resumimos as principais conclusões no nosso próprio processo de aprendizado sobre obras públicas e linkamos alguns documentos nos quais nos baseamos.

- Posso usar qualquer linguagem de programação?
**R:** Sim. Nosso time de dados é fluente em Python e R. Se você usar outra linguagem, apenas redobre os cuidados com a legibilidade do código e a inserção de comentários e *docstrings* no código. Esperamos que não seja difícil ler nenhum código bem escrito, independentemente da linguagem escolhida.

- E Excel (ou outro software de planilhas), vale?
**R:** Vale... Nesse caso, considere como "código fonte" a própria planilha, com qualquer passo intermediário utilizado. Se usar VBA, ele também conta como código fonte.

- Como entrego o resultado?
**R:** Após o final do prazo, vamos visitar as contas de GitHub informadas na inscrição e buscar entre os últimos repositórios com *commits*. Se não conseguirmos identificar o repositório relativo ao desafio, o(a) candidato(a) será desclassificado(a).

- Quanto sai o resultado?
**R:** Esperamos conseguir avaliar tudo em até uma semana após o encerramento do prazo de entrega - mas essa é *só uma previsão*.

- Vocês vão avisar quem não passar para a próxima etapa?
**R:** Com certeza. Mesmo se você não for selecionado(a) para a próxima etapa, vamos mandar um e-mail avisando o resultado.

- Qual é a próxima etapa?
**R:** A próxima etapa são as entrevistas com o time de dados e com o restante da equipe. Dependendo do número de classificados para a última etapa, a primeira dessas duas poderá ser em grupo ou individual. Daremos mais detalhes junto com o resultado.

- Tenho uma dúvida que não está aqui. Onde posso perguntar?
**R:** Você pode [abrir uma issue](https://github.com/Inova-MPRJ/desafio-estagio-inova/issues) neste repositório. Assim, garantimos que uma dúvida que pode ser de mais gente seja respondida apenas uma vez pela nossa equipe.
Se você tiver uma questão exclusivamente pessoal, entre em contato com o nosso e-mail: [inova@mprj.mp.br](mailto:inova@mprj.mp.br). Em ambos os casos, vamos tentar responder o mais breve possível.
