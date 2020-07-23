<h1>Desafio - Estágio em Análise de Dados - Inova_MPRJ 2020</h1>
<p>Descrição detalhada dos métodos utilizados para análise de dados</p>
<p><b>Base de Dados Original</b></p>
<p>A base de dados original é composta por um total de 23 planilhas de excel, sendo estas compostas de dados relacionados a pagamentos, prorrogação do prazo, cronogramas de metas e etapas
convenio e historico da situação.</p>
<p><b>Observações:</b></p>
<li>Para esta análise foi utilizada apenas as planilhas: <b>siconv_etapa_crono_fisico</b>, <b>siconv_meta_crono_fisico</b>, <b>siconv_prorroga_oficio</b>, <b>siconv_termo_aditivo</b></li>
<li>As planilhas sofreram modificações em sua composição, foi acrescentado as colunas DURACAO_ETAPA, DURACAO_META e DURACAO_TA. Ambas as colunas foram acrescentadas com o objetivo de apresentar a duração de cada período de etapas, metas, prorrogação e temos aditivos.
Para o cálculo foi utilizada a equação =MONTH()-MONTH do excel. Desta forma, temos agora as planilhas nomeadas Atualizada_siconv_etapa_crono_fisico, Atualizada_siconv_meta_crono_fisico,
Atualizada_siconv_termo_aditivo
