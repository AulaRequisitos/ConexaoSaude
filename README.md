# ConexaoSaude

# Projeto Disciplina: Requisitos de Software

Olá! Este repositório faz parte do projeto da disciplina de Requisitos de Software da UTFPR - Campus Cornélio Procópio. 

Link do Padlet:
https://padlet.com/neto0309/requisitos-de-software-glri12evthgxkqlf

## 1. Introdução
  
  ***1.1.  Grupo 6***

helder659
rafinhagvianna
FernandesHigor
GustavGomes36

  ***1.2.  Nome do Sistema***

Conexão Saúde

  ***1.3.  Propósito do Sistema***

  Objetivo: O objetivo do software é ajudar grupos vulneráveis da sociedade, informando e localizando postos de saúde, hospitais e outras instituições de saúde pública que possam suprir suas necessidades específicas. Além disso, busca priorizar, de modo eficiente, a redução do processo consultivo e auxiliar no transporte desses grupos vulneráveis até as instituições.

  ***1.2.  Público Alvo***

  Público-alvo: Pais com filhos pequenos e necessidades médicas, idosos, pessoas com doenças degenerativas, gestantes, entre outros.

  ***1.3. Descrição dos usuários***

  Pais com filhos pequenos e necessidades médicas: Geralmente buscam produtos e serviços que ofereçam segurança, conforto e praticidade. Estão preocupados com saúde, alimentação, bem-estar e desenvolvimento infantil.

  Idosos: Podem ter demandas voltadas à acessibilidade, conforto, saúde, entretenimento e qualidade de vida. Muitos valorizam a autonomia, mas também podem precisar de suporte para mobilidade e assistência médica.

  Pessoas com doenças degenerativas: Necessitam de acompanhamento contínuo e soluções que melhorem sua qualidade de vida. Terapias alternativas, equipamentos médicos e assistência personalizada são essenciais para o dia a dia.

  Gestantes: Buscam informação, produtos e serviços que garantam uma gravidez tranquila e saudável. Itens como roupas adaptadas, alimentação balanceada, suporte emocional e médico são prioritários.

  ***Personas:***

![image](https://github.com/user-attachments/assets/087783fe-9b34-4af6-9c62-84232df6bd01)
![image](https://github.com/user-attachments/assets/84a7c439-c949-42d3-b940-e17e96b2fa3e)
link para o acesso completo ao mapa da persona: https://www.canva.com/design/DAGm_WIvfpI/dtyuo0LkB_7ElQNZDLkcvA/edit?ui=eyJBIjp7fX0

  ***Análise da situação atual: antes da introdução de sua solução***

*`1. O que as pessoas fazem?`*

  Pessoas em situação de vulnerabilidade normalmente buscam atendimento de saúde de forma manual, ligando para unidades ou indo presencialmente até postos e hospitais, muitas vezes sem saber se há atendimento disponível, resultando em longas filas, deslocamentos desnecessários e falta de informação adequada.

*`2. Quais os artefatos envolvidos?`*

  Celulares para ligações, documentos físicos, transporte público ou privado, informações orais obtidas em comunidades, anotações em papel, além de recursos informais como redes sociais ou recomendações de conhecidos.

*`3. O que elas precisam saber?`*

  Precisam saber onde há atendimento próximo, se há especialidades compatíveis com suas necessidades, se o local está funcionando, qual o tempo de espera e como chegar até lá de forma acessível.

  ***Análise das tarefas depois: como serão executadas as suas tarefas com sua solução:***

*`1. O que as pessoas fazem?`*
   
   Utilizam o aplicativo Conexão Saúde para localizar rapidamente unidades próximas, filtrar por especialidades, verificar disponibilidade e agendar atendimentos prioritários, além de consultar rotas e solicitar transporte quando necessário.

*`2. Quais os artefatos envolvidos?`*

  Smartphone com o aplicativo Conexão Saúde, conexão com a internet, sistema de geolocalização, integração com bases como o CNES, aplicativos de transporte e notificações em tempo real.

*`3. O que elas precisam saber?`*

  Precisam apenas saber utilizar o aplicativo, pois a ferramenta irá fornecer informações completas e acessíveis sobre as unidades de saúde, tempos de espera, especialidades, localização e meios de transporte disponíveis.

  ***Cenário: Antes***

  Joana, mãe de uma criança asmática, precisa levá-la ao médico com urgência. Sem saber onde encontrar um pediatra disponível, ela tenta ligar para várias unidades de saúde, sem sucesso. Decide ir até o hospital da cidade, onde enfrenta uma fila de espera de horas, apenas para ser informada de que não há pediatras de plantão. Sem informações, ela volta para casa frustrada e preocupada com a saúde do filho.


  ***Cenário: Depois***

  Joana, ao perceber que seu filho apresenta sintomas, abre o aplicativo Conexão Saúde. Em segundos, ela localiza uma unidade próxima com atendimento pediátrico disponível, visualiza o tempo estimado de espera e solicita um carro de transporte parceiro pelo próprio app. Chega ao local em segurança e com prioridade de atendimento, garantindo o cuidado necessário com agilidade.


## 2. Documentos gerais no repositório

  ***2.1. Requisitos Funcionais***

| Identificador | Descrição    | Prioridade  | Depende de                                                                |
|:------:|:----------------------------------------------------:|:------------:|:------------------------:|
| RS01   | O software deve notificar um alerta para os usuários médicos em caso de superlotação em postos de atendimentos da região | Alta | R1 |
| RS02   | O software deve salvar o cadastro dos usuários e médicos em um banco de dados | Alta | R1 |
| RS03   | O software deve localizar o usuário para saber sua trajetória a um melhor destino, isso deve ocorrer após o usuário permitir a que o app acesse a sua localização | Alta | R1 |
| RS04   | O software deve todo mês mostrar ao usuário um evento e nesses evento enviar tasks para o usuário | Alta | R1 |
| RS05   | O software deve priorizar certos pacientes, dependendo da sua situação de risco/saude ou seja hierarquia na fila/ criar uma fila para casos graves | Alta | R1 |
| RU04   | O usuário deve informar se está sozinho ou não, se consegue chegar ao posto mais acessível ou não, para assim o software entender se requisitar ajuda de transporte para o usuário | Alta | R1 |
| RU08   | O usuário poderá avaliar o atendimento (nota + comentário). E o software deve conectar/alocar esse comentário a comentários do posto e do médico que usuário refere-se | Alta | R1 |
| RS09   | O software deve filtrar quais tipos de medicamentos devem ser indicados para o usuário (devido a alguma alergia, ou restrição que ele informou ) | Alta | R1 |
| RS12   | O Sistema deve possibilitar a busca de informações sobre postos de saúde,hospitais entre outras intituições de saúde publica: exibição de uma caixa de texto que servira de entrada do usuario para o sistema; exibe resultados com base em entradas parciais do usuario, em caixas em fileira; exibe informações simplificadas da instituição nas caixas infileiradas | Alta | R1 |
| RU05   | O usuário deve informar/selecionar qual tipo de atendimento procura (Pediatrico; Pronto-Atendimento; Hospital geral;) | Alta | R1 |



  ***2.2. Requisitos Não Funcionais***

| Requisito | Tipo     | Descrição                                                                 |
|:------:|:-------:|---------------------------------------------------------------------------|
| RU01 | Estático | O Sistema deve garantir a Conformidade com as regulações LGPD Brasileiras. |
| RU02 | Estático | O Sistema deve garantir um tempo de resposta rápido, dado o objetivo do projeto |
| RU03 | Volátil | O Sistema deve ser compátivel e integrado com API gratuitas e sistemas governamentais(por enquanto simulação com um banco de dados e servidores) para auxiliar em questões como geolocalização,
exibição e armazenamento de informações | 
| RU04 | Estático | O Sistema deve ter uma interface simples e intuitiva para ser acessivel ao público não familizarizado com a tecnologia | 
| RS01 | Volátil | O Sistema deve utilizar um mecanismo de auditoria para verificar logs, o banco de dados e documentações, afim criar um relatorio apontando possiveis
irregularidades com a LGPD |
| RS02.1 | Estático | O Sistema deve cachear consultas frequentes utilizando Redis para reduzir o tempo de acesso ao banco de dados | 
| RS02.2 | Estático | O Banco de dados deve suportar indexação para otimizar a pesquisa de dados | 
| RS02.3 | Volátil | O Sistema deve registrar e analisar métricas de desempenho (tempo de resposta médio, quantidade de requisições, taxa de erro) |
| RS02.3 | Estático | O Sistema deve garantir um processamento assincrono por meio async e await em python |
| RS03.1 | Estático|  O Sistema deve integrar a API Fused Location Provider do Android para a geolocalização|
| RS03.2 | Estático|  O Sistema deve utilizar o [banco de dados] para armazenar informações |
| RS03.3 | Estático|  O Sistema deve utilizar uma [Interface Gráfica] para exibir informações |

  ***2.3. Perguntas***

*<Arquivo com as perguntas realizadas na entrevista .>*

  ***2.4. Entrevista***

*<Arquivo com as respostas do indivíduo entrevistado e link do drive com upload da gravação.>*

  ***2.5. Histórias do Usuário***

*<Imagem, arquivo (PDF), link com as Histórias de Usuário.>*

  ***2.6. Diagramas de Caso de Uso e Especificações***

*<Imagem, arquivo (PDF), link com Diagrama de Caso de Uso.>*

  ***2.7. Diagramas de Atividades***

*<Imagem, arquivo (PDF), link com Diagrama de Atividades.>*

  ***2.8. Matrizes de Rastreabilidade***

*<Imagem, arquivo (PDF), link com Matriz de Rastreabilidade.>*

  ***2.9. Protótipos***

*<Imagem, arquivo (PDF), link com Protótipo.>*

## Referências

*<Esta seção é destinada à descrição das referências utilizadas pelo documento, como por exemplo, URLs e livros. Ver exemplo a seguir:>*

[1] “Glossário da _USina_”, <_id_doc glossário_>, Versão <_versão_>. Localização: <_localização_>.
