<div>

<span class="c2 c26"></span>

</div>

<span class="c2 c0">Este trabalho é um projeto da disciplina de
Engenharia de Software II da Universidade Federal de Minas Gerais,
Departamento de Ciência da Computação. Feito pelos alunos Cláudio
Manuel, Tauany Santos e Wallace Augusto, em Maio de 2017.</span>

<span class="c2 c0">O objetivo do projeto é fazer uma documentação de um
sistema open source, hospedado no GitHub e que seja popular (com mais de
1000 estrelas).</span>

<span class="c0">Foi escolhido o sistema StackStorm, uma plataforma que
realiza a integração entre serviços de padrões operacionais
comum.</span>

<span class="c4 c11"></span>

1.  <span class="c4 c11">Descrição do Sistema</span>

<!-- -->

1.  <span class="c4 c11">Características e objetivo</span>

<span class="c4 c11"></span>

<span class="c2 c0">O StackStorm é uma plataforma de automação de código
aberto que realiza a integração entre serviços e ferramentas de padrões
operacionais comuns. O foco principal da plataforma é tomar ações em
resposta a eventos que ocorrem. Além disso, tem por objetivo
proporcionar aos seus usuários uma forma organizada de conectar todos os
aplicativos, serviços e fluxos de trabalho que ele utiliza de uma forma
mais simples, tornando mais facilmente esse ambiente automatizado.
</span>

<span class="c2 c0">A plataforma é composta por Sensors, Triggers,
Actions, Rules, Workflows, Packs e Audit Trail, todos estes componentes
em conjunto realizam a conexão dos serviços e fluxos de trabalho.</span>

-   <span class="c2 c0">Os Sensors são plugins que fazem a integração da
    entrada e saída de eventos.</span>
-   <span class="c2 c0">Os Triggers são representações de
    eventos externos. É possível definir um novo disparador, para isso é
    necessários criar um novo plugin de sensor.</span>
-   <span class="c2 c0">As Actions são plugins na linguagem Python ou
    qualquer outro script. Existem ações genéricas, por exemplo “ssh”,
    ou ações personalizadas. Essas ações podem ser chamadas diretamente
    pelo usuário, através de uma API, por exemplo. Além disso, podem ser
    usadas e chamadas como regra e fluxos de trabalho (tópicos que estão
    explicados abaixo). </span>
-   <span class="c2 c0">As Rules desencadeiam ações. Elas aplicam
    critérios de correspond\
    ência e fazem um mapeamento para definir como será a entrada
    de ações.</span>
-   <span class="c2 c0">Os Workflows definem a ordem e as condições de
    transações de dados. Em geral, são necessárias mais de uma ação para
    uma automação, quando ela possui mais de uma etapa. Os fluxos de
    trabalho podem ser chamados manualmente ou por regras.</span>
-   <span class="c2 c0">Os Packs são unidades de implantação de conteúdo
    utilizadas para simplificar o gerenciamento e compartilhamento
    de conteúdos.</span>
-   <span class="c2 c0"> A Audit Trail de execução de ações pode ser
    manual ou automática, o usuário pode definir e a partir disso, é
    gravada e armazenada a ação, especificando o contexto e o resultado
    da execução.</span>

<span class="c2 c0">O conteúdo que é armazenado na plataforma é todo em
código. Além disso, os Packs, que são as unidades de implantação de
conteúdo podem ser criados e compartilhados no GitHub ou enviados para o
repositório da comunidade StackStorm.</span>

<span class="c2 c0">A licença utilizada pelo projeto é a Licença Apache
que pode ser lida no link abaixo:</span>

<span
class="c27 c0">[Http://www.apache.org/licenses/LICENSE-2.0](https://www.google.com/url?q=http://www.apache.org/licenses/LICENSE-2.0&sa=D&ust=1495544847380000&usg=AFQjCNGX8G1gAPVfgqAJlMjsvHgE9hVixQ){.c19}</span>

<span class="c2 c0"></span>

<span class="c4 c11">1.2 Linguagem e Ferramenta</span>

<span class="c2 c0">        </span>

<span class="c2 c0">A linguagem principal utilizada na plataforma é o
Python que é a linguagem utilizada para a criação dos plugins de Sensors
e também para os plugins de Actions. A linguagem Python é uma linguagem
de programação de alto nível, de script, imperativa e orientada a
objetos. Além de Python, outras linguagens são utilizadas nas
contribuições de Packs, como por exemplo a linguagem Shell e o
Javascript.</span>

<span class="c2 c0">Shell é uma linguagem interpretada, de script que é
usada em diversos sistemas operacionais com diversos dialetos. Assim
como o Python, Javascript é uma linguagem de script, orientada a objetos
e é utilizada para conectar os objetos do ambiente.</span>

<span class="c2 c0">Uma ferramenta que é utilizada na plataforma é a
“CloudSlang” que faz o gerenciamento de aplicativos implantados. O
objetivo do uso desta ferramenta é automatizar rapidamente as operações
de TI diárias e definir um workflow estruturado e fácil de entender.
</span>

<span class="c2 c0">A “CloudSlang”, é um DSL que se baseia em uma
linguagem YAML, que é utilizada para realizar consultas complexas no
banco de dados. Os conteúdos da CloudSlang são divididos em dois tipos
principais que são as operações e os fluxos. Estas operações podem ser
escritas em duas linguagens diferentes, que são Java e Python.  </span>

<span class="c2 c0">Um outro mecanismo utilizado é o Jinja2 que é um
modelo completo para a linguagem Python. Ele é utilizado para gerenciar
os workflows da plataforma.</span>

<span class="c2 c0"></span>

------------------------------------------------------------------------

<span class="c2 c0"></span>

<span class="c2 c0"></span>

2.  <span class="c4 c11">Equipe de Desenvolvimento</span>

<span class="c4 c11"></span>

<span class="c2 c0">O projeto StackStorm é uma plataforma de
automatização que possui uma versão open-source com suporte da
comunidade. Seu desenvolvimento e construção se fez através de uma
comunidade no Slack. O Slack funciona como uma rede social, através
dele, qualquer pessoa pode criar uma sala de bate-papo, com múltiplos
canais, dentro de uma empresa, com assuntos distintos e para grupos
diferentes. Dentro de cada um desses canais, a ferramenta permite troca
de mensagens de texto, documentos e compartilhamento de mídias, como
fotos e vídeos.</span>

<span class="c2 c0">Tanto o team principal quanto os diversos usuários e
desenvolvedores utilizam essa ferramenta para desenvolver a plataforma
StackStorm, que, no caso, já são mais de 200 pessoas envolvidas. Abaixo,
a sua equipe de fundação:</span>

<span class="c2 c0"></span>

<span
style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 187.00px; height: 269.00px;">![ph-dmitri1.jpg](images/image10.jpg)</span>

<span class="c2 c0"></span>

<span class="c2 c0">Dmitri Zimine</span>

<span class="c2 c0">Chief Stormer & Co-Fundador</span>

<span class="c2 c0">Ajudou a liderar a primeira onda de automação de
operações enquanto servia como arquiteto-líder e chefe de engenharia na
Opalis.</span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span
style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 187.00px; height: 282.00px;">![ph-winson-2.jpg](images/image1.jpg)</span>

<span class="c2 c26"></span>

<span class="c0 c28">Winson Chan</span>

<span class="c2 c0">Stormer</span>

<span class="c2 c0">Focado no desenvolvimento de produtos. Altamente
qualificado na concepção e desenvolvimento de autoatendimento, soluções
automatizadas e gerenciamento de pilhas VM na nuvem híbrida da
empresa.</span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span
style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 187.00px; height: 283.00px;">![ph-patrick-2.jpg](images/image8.jpg)</span>

<span class="c2 c0"></span>

<span class="c2 c0">Patrick Hooboom</span>

<span class="c2 c0">Stormer</span>

<span class="c2 c0">Stormer focado em DevOps. Tem como objetivos
alavancar as ferramentas de gerenciamento de configuração e criar
scripts personalizados para melhorar os processos em toda a
organização.</span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span
style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 187.00px; height: 271.00px;">![ph-lakshmi-2.jpg](images/image2.jpg)</span>

<span class="c2 c0"></span>

<span class="c2 c0">Lakshmi Kannan </span>

<span class="c2 c0">Stormer</span>

<span class="c2 c0">Responsável por construir uma plataforma previsível,
de melhor performance e utilizável. Anteriormente, trabalhou na Amazon e
Rackspace construindo sistemas altamente distribuídos e de baixa
latência.</span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span
style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 187.00px; height: 269.00px;">![ph-manas.jpg](images/image11.jpg)</span>

<span class="c2 c0"></span>

<span class="c2 c0">Manas Kelshikar </span>

<span class="c2 c0">Stormer</span>

<span class="c0">Desenvolvedor da plataforma. Trabalhos anteriores na
VMware como membro da equipe de clientes vSphere, onde contribuiu para a
arquitetura e implementação do produto de nova geração.</span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span
style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 187.00px; height: 269.00px;">![ph-tomaz-2015-05-14.jpg](images/image5.jpg)</span>

<span class="c2 c0"></span>

<span class="c2 c0">Tomaz Muraus </span>

<span class="c2 c0">Stormer</span>

<span class="c2 c0">Auxilia na construção da plataforma. Trabalhou
anteriormente na Cloudkick, Rackspace e DivyCloud como desenvolvedor e
operando sistemas altamente distribuídos.</span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

<span class="c2 c26"></span>

<span class="c2 c0"></span>

3.  <span class="c4 c11">Evolução do sistema</span>

<span class="c2 c0"></span>

<span class="c2 c0">Nesta seção, serão descritas as principais releases
da plataforma StackStorm, retirados dos log de releases do projeto no
git e do blog de desenvolvedores. Releases de teste, não estáveis, como
beta e alpha, não serão descritas.</span>

<span class="c2 c0"></span>

-   <span class="c4 c0">v0.8.0 - Disponibilizada em 3 de Março de
    2015</span>

<span class="c0">Primeiro release do StackStorm, com 143 </span><span
class="c0 c1">commits</span><span class="c2 c0">, desenvolvido por 2
meses. StackStorm 0.8 possui uma interface web para usuário que facilita
o uso da plataforma. Esta interface possui 3 visões: a página Actions
lista todas as ações registradas na instalação da plataforma; A página
History exibe todas as ações que estão sendo executadas em real-time e
seus status, além de todas as ações anteriormente executadas; A página
Rules indica todas as regras registradas que podem ser executadas pela
interface.</span>

-   <span class="c4 c0">v0.9.1 - Disponibilizada em 13 de Maio de
    2015</span>

<span class="c0">Após várias correções de </span><span
class="c0 c1">bugs</span><span class="c0"> e com 7159 </span><span
class="c0 c1">commits</span><span class="c2 c0">, esta versão foi
apresentada com 2 melhorias: criação da opção de ignorar checagem de
Certificados SSL e retorno de HTTP BAD REQUEST quando requerido token
TTL.</span>

-   <span class="c4 c0">v0.11 - Disponibilizada em 5 de Junho de
    2015</span>

<span class="c0">Com 6689 </span><span class="c0 c1">commits</span><span
class="c0">, esta versão apresentou melhorias na configuração CLI da
plataforma, como a criação de comandos </span><span class="c0 c1">get,
list </span><span class="c0">e </span><span
class="c0 c1">re-emit</span><span class="c2 c0">. Algumas outras
melhorias no funcionamento da API.</span>

-   <span class="c4 c0">v0.13 - Disponibilizada em 24 de Agosto de
    2015</span>

<span class="c0">Após 5542 </span><span
class="c0 c1">commits</span><span class="c0">, esta versão revelou a
construção de uma autenticação no backend da plataforma, além de
aperfeiçoamentos na estrutura da plataforma. Também foram executadas
melhorias na configuração CLI, com a criação de novas </span><span
class="c0 c1">features.</span><span class="c2 c0"> </span>

-   <span class="c4 c0">v1.1.0 - Disponibilizada em 27 de Outubro de
    2015</span>

<span class="c0">Adicionado YAQL v1.0 para suporte do Mistral, já que as
versões anteriores foram descontinuadas. Updates para os comandos da
CLI. Nova autenticação no backend da plataforma para servidores LDAP.
Melhorias na API, tais como chaves que não expiram como tokens de
autenticação. Adicionada opção de verificação de certificado SSL para
requisição HTTPS. Correção de </span><span class="c0 c1">bugs
</span><span class="c0">na execução do Paramiko SSH. Total de 4364
</span><span class="c0 c1">commits</span><span class="c2 c0">. </span>

-   <span class="c0 c4">v1.2.0 - Disponibilizada em 8 de Dezembro de
    2015</span>

<span class="c0">Com 3866 </span><span
class="c0 c1">commits,</span><span class="c0"> esta versão apresenta
correção de </span><span class="c0 c1">bugs</span><span class="c0"> na
execução do Paramiko SSH, tais como conexão com parâmetros ao seu alvo.
Melhorias na API da plataforma, como por exemplo na criação de validação
de parâmetros durante a criação de novas regras. Nova </span><span
class="c0 c1">feature</span><span class="c0"> para o campo de
notificações. Classes mock adicionadas aos </span><span
class="c0 c1">scripts </span><span class="c2 c0">para facilitar
testes.</span>

-   <span class="c4 c0">v1.3.0 - Disponibilizada em 22 de Janeiro de
    2016</span>

<span class="c0">Posteriormente, 3390 </span><span
class="c0 c1">commits</span><span class="c0"> foram feitos a esta
versão, que trouxe a introdução de novos parâmetros para a instalação da
plataforma. Além de novas </span><span
class="c0 c1">features,</span><span class="c0"> como novas ações em
Trace e em uma lista de regras. Suporte para objetos presentes no banco
de dados. Adição de </span><span class="c0 c1">flag</span><span
class="c0">s ao </span><span class="c0 c1">script.</span><span
class="c2 c0"> Melhorias na utilização das classes mock. </span>

-   <span class="c4 c0">v1.4.0 - Disponibilizada em 18 de Abril de
    2016</span>

<span class="c0">Depois de 2717 </span><span class="c0 c1">commits,
</span><span class="c0">várias melhorias foram apresentadas, como
melhorias no suporte da execução SSH da plataforma, através de ações de
autenticação de senha, suporte a porta padrão (22), entre outros.
Aperfeiçoamentos no ChatOps e na API. Acesso ao banco de dados através
da utilização de Python. Novas </span><span class="c0 c1">features,
</span><span class="c0">como operadores </span><span class="c0 c1">regex
</span><span class="c0">e </span><span class="c0 c1">iregex.
</span><span class="c0">Adição de novas </span><span class="c0 c1">flags
</span><span class="c0">no script</span><span class="c22 c0 c1">.</span>

<span class="c0 c1 c22"></span>

<span class="c22 c0 c1"></span>

-   <span class="c4 c0">v2.1.0 - Disponibilizada em 5 de Dezembro de
    2016</span>

<span class="c0">Poucos </span><span class="c0 c1">commits</span><span
class="c0"> realizados, apenas 1016, porém novas </span><span
class="c0 c1">features </span><span class="c2 c0">foram apresentadas
nessa nova versão, tais como a adição de novos comandos CLI e a
adaptação da mesma com JSON. Melhorias no desempenho da API no
tratamento de exceções. Melhorias nos packs, para consistência. </span>

-   <span class="c4 c0">v2.2.0 - Disponibilizada em 25 de Fevereiro de
    2017</span>

<span class="c0">Correção de vários </span><span class="c0 c1">bugs
</span><span class="c2 c0">na API. Validações nas opções de configuração
de criação de regras no sistema. Correções apropriadas nas políticas de
cancelamento de ações.</span>

-   <span class="c4 c0">v2.2.1 - Disponibilizada em 3 de Abril de
    2017</span>

<span class="c0">Versão atual, com apenas 576 </span><span
class="c0 c1">commits,</span><span class="c0"> que apresenta melhorias
em seu </span><span class="c0 c1">script</span><span class="c0">, para
correção de erros padrões. Correção de vários </span><span
class="c0 c1">bugs,</span><span class="c0"> como configurações na API ou
suporte de bibliotecas para testes.</span>

<span class="c4 c11"></span>

4.  <span class="c4 c11">Arquitetura e Componentes do Sistema</span>

<span class="c4 c11"></span>

<span class="c2 c0">O StackStorm é um serviço que possui uma arquitetura
modular. Ele compreende componentes de serviços acoplados que se
comunicam por meio de barramentos de mensagens e escala horizontalmente
para enviar automaticamente em escala. Para isso, o StackStorm utiliza
REST API, que é um meio de providenciar a troca e o uso de informações
entre os sistemas computacionais na Internet. Ele também utiliza CLI
client, que é uma interface para linha de comando, para administradores
e usuários operarem localmente ou remotamente o sistema. Além disso, o
StackStorm utiliza a biblioteca Python client para a conveniência do
desenvolvedor. Ainda não possui uma interface Web mas em breve estará
disponível.</span>

<span class="c2 c0">O diagrama a seguir mostra a arquitetura do sistema,
incluindo seus componentes:</span>

<span
style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 598.99px; height: 454.50px;">![](images/image9.png)</span>

<span class="c2 c0">Diagrama arquitetural do StackStorm</span>

<span class="c2 c0"></span>

1.  <span class="c2 c0">Os eventos são agregados, via Push/Pull, de
    vários serviços por meio de Sensors;</span>
2.  <span class="c2 c0">Events são comparados com Triggers e geram
    Actions;</span>
3.  <span class="c2 c0">As ações processadas dos workflows são colocadas
    na lista de mensagem (RabbitMQ);</span>

<span class="c2 c0">3b.        Mistral workflows são processados pelo
Mistra Service (Opicional);</span>

<span class="c2 c0">3c.        Actions alcançam vários serviços para
executarem ações do workflow;</span>

<span class="c2 c0">4.        O Log e o Audit History são armazenados no
banco de dados (MongoDB);</span>

<span class="c2 c0">5.        Processed Results são enviados de volta
para o mecanismo de regras para processamento adicional.</span>

<span class="c2 c0"></span>

<span class="c2 c0">Os seguintes componentes foram discutidos na
primeira parte desse manual: Sensors, Triggers, Actions, Rules,
Workflows, Packs e Audit trail.</span>

<span class="c2 c0"></span>

<span class="c2 c0">StackStorm implementa o controle Role Based Access
(RBAC) que permite administradores e operadores do sistema a
restringirem o acesso do usuário e limitar as operações que podem ser
realizadas. Além disso, o banco de dados operador pode ter acesso apenas
ao banco de dados relacionado às ações que serão efetuadas.</span>

<span class="c2 c0">Quanto à autenticação do sistema, é incluso um
serviço de autenticação responsável pela autenticação do usuário e gerar
o token de tempo limite de acesso. Quando o modo de autenticação está
ativo (modo default), esse token de acesso é utilizado para autenticar
junto ao StackStorm REST APIs. A imagem a seguir mostra o funcionamento
da autenticação do sistema:</span>

<span
style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 601.70px; height: 348.00px;">![](images/image12.png)</span>

<span class="c2 c0">Serviço de autenticação do StackStorm</span>

<span class="c2 c0"></span>

------------------------------------------------------------------------

<span class="c2 c0"></span>

<span class="c2 c0"></span>

2.  <span class="c4 c11">Padrões de código</span>

<span class="c4 c11"></span>

<span class="c2 c0">A maioria dos repositórios utilizam arquivos de
configuração compartilhados do Flake8 e PyLint. O StackStorm segue
alguns padrões que devem ser utilizados durante o desenvolvimento do
código. São eles:</span>

-   <span class="c2 c0">PEP8 Python Style Guide;</span>
-   <span class="c2 c0">4 espaços para o tab;</span>
-   <span class="c2 c0">No máximo 100 caracteres em uma linha;</span>
-   <span class="c2 c0">Arquivos editados não devem conter espaço em
    branco à esquerda;</span>
-   <span class="c2 c0">Todos os arquivos fonte devem conter o cabeçalho
    da licença do Apache 2.0;</span>
-   <span class="c2 c0">Verificar se as modificações não quebram
    nenhuma regra. Isso pode ser feito rodando o script
    “make flake8”.</span>

<span class="c2 c0"></span>

3.  <span class="c4 c11">Diretriz geral do código</span>

<span class="c4 c11"></span>

-   <span class="c2 c0">Logging</span>

<span class="c2 c0">É importante por aumentar a visibilidade e fazer o
projeto mais fácil de ser entendido e dar suporte. Toda a declaração de
log deve conter o maior número possível de informações adicionais
possível. Essas informações devem ser incluídas no dicionário que é
passado via argumento para o método logger. O formato default do log que
é utilizado inclui esse contexto adicional como parte da mensagem que
ajudará o usuário a encontrar a informação relevante. </span>

<span class="c2 c0">Para obter uma referência à instância logger,
deve-se utilizar a função “st2common.log.getLogger”. Deve-se usar essa
função ao invés da função do módulo logging do stdlib pois é declarado
um nível de log personalizado e faz mais algumas coisas que está
disponível apenas nos loggers que são obtidos através da versão do
getLogger. Na maioria das vezes, isso deve ser feito no início do
módulo, após os imports e esse logger deve ser utilizado no
módulo.</span>

<span
style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 503.50px; height: 109.00px;">![](images/image4.png)</span>

<span class="c2 c0">O dicionário deve conter valores que são relevantes
ao log da mensagem em questão, como por exemplo, criado banco de dados
do objeto, usuário que fez a ação. </span>

<span class="c2 c0">Se estiver passando uma instância de uma classe
personalizada como valor, deve ser implementado o método “to\_dict”
nessa classe. Esse método é responsável por retornar uma representação
do dicionário desse objeto que pode ser serializável como JSON. É
importante lembrar que esse método já está implementado para todos os
banco de dados do StackStorm (ActionDB, RunnerTypeDB, etc).</span>

<span
style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 504.50px; height: 160.00px;">![](images/image3.png)</span>

<span class="c2 c0">Todos os objetos datetime que estão sendo utilizados
no código devem estar na timezone correta e representadas em UTC. O
mesmo vale para datas armazenadas do banco de dados, se não puder
utilizar timestamp, as datas armazenadas devem ser representadas em
UTC.</span>

-   <span class="c2 c0">Instanciando classes modelo</span>

<span class="c2 c0">Quando instanciadas as classes modelo, como
ActionDB, RuleDB, SensorTypeDB, deve-se passar todos os valores como
argumentos ao construtor ao invés de atribuir variáveis à instância da
classe. Passar todos os campos como argumentos ao construtor significa
que a funcionalidade do construtor é preservada. Pode também deixar mais
claro e óbvio para os desenvolvedores quando os valores estão
disponíveis e permite uma análise estática básica no código.</span>

<span class="c2 c0">Como deve ser:</span>

<span
style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 502.50px; height: 52.00px;">![](images/image6.png)</span>

<span class="c2 c0">Como não deve ser:</span>

<span
style="overflow: hidden; display: inline-block; margin: 0.00px 0.00px; border: 0.00px solid #000000; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px); width: 501.50px; height: 107.00px;">![](images/image7.png)</span>

------------------------------------------------------------------------

<span class="c4 c11"></span>

4.  <span class="c4 c11">Estrutura do código</span>

<span class="c2 c0"></span>

-   <span class="c2 c0">StackStorm/st2 Repo</span>

<span class="c2 c0">O StackStorm é feito por serviços individuais viz.
st2auth, st2api, st2rulesengine, st2sensorcontainer, st2actionrunner,
st2notifier.</span>

<span class="c2 c0">StackStorm também possui um CLI e uma biblioteca
client. Os códigos para todos esses serviços e componentes são
apresentados em diferentes pastas no diretório raiz.</span>

-   <span class="c0 c2">st2common</span>

<span class="c2 c0">Código comum que contém o banco de dados e os
modelos dos dados API, funções de utilidades e código de serviço comum
que todo o StackStorm necessita. Cada pacote de serviço (deb/rpm) tem
uma dependência no pacote st2common sendo disponível. Então todo código
comum que deve ser compartilhado entre componentes deve ser adicionado
neste diretório.</span>

-   <span class="c2 c0">st2api</span>

<span class="c2 c0">Esse diretório contém o código para os controladores
API do StackStorm. As APIs e os controladores são versionados.
Controladores experimentais são adicionados ao diretório exp dentro de
st2api e, quando maduros, são movidos para a pasta dos controladores
versionados.</span>

-   <span class="c2 c0">st2auth</span>

<span class="c2 c0">Contém o código para o ponto final do st2auth. Já
que esse ponto final precisa ser implementado separadamente do st2api,
ele está disponível como um aplicativo separado.</span>

-   <span class="c2 c0">st2actions</span>

<span class="c2 c0">Contém o código para as ações que ocorrem no
StackStorm. Uma nova ação para o StackStorm deve ser adicionada em
st2actions/st2actions/runners. Esse diretório também contém o código
para o nó trabalhador que verifica rabbitmq para execuções de
entrada.</span>

<span class="c2 c0">Notifier e results tracker também fazem parte desse
código base. Notifier é o componente que envia disparadores de
notificações e de ações até o final execução da ação. Results tracker é
uma lista assíncrona avançada para certos tipos de corredores, como
mistral, onde a execução do workflow é parada remotamente e é necessário
acionar o mistral API para coletar os resultados.</span>

-   <span class="c2 c0">st2client</span>

<span class="c2 c0">Contém o código tanto para a biblioteca StackStorm
client quanto para StackStorm em apenas um diretório. Isso será
eventualmente separado. </span>

-   <span class="c2 c0">st2debug</span>

<span class="c2 c0">O código apresentado neste diretório vem da
ferramenta st2-submit-debug-info. Essa ferramenta fornece um jeito de
compartilhar logs e outras informações com o engenheiro de solução de
problemas do StackStorm.</span>

-   <span class="c2 c0">st2reactor</span>

<span class="c2 c0">Contém o código para o sensor e para o mecanismo de
regras.</span>

-   <span class="c2 c0">st2tests</span>

<span class="c2 c0">Código compartilhado que contém utilitários de
testes que ajudam a testar individualmente e a integração para todos os
componentes do StackStorm.</span>

<span class="c2 c0"></span>

<span class="c2 c0"></span>

5.  <span class="c11 c29">Referências</span>

<span class="c2 c0"></span>

<span
class="c27 c0">[https://github.com/StackStorm/st2](https://www.google.com/url?q=https://github.com/StackStorm/st2&sa=D&ust=1495544847488000&usg=AFQjCNHiVa1EWfROrzIDDTOFQQX4Q7pP1A){.c19}</span>

<span
class="c0 c27">[https://stackstorm.com/](https://www.google.com/url?q=https://stackstorm.com/&sa=D&ust=1495544847489000&usg=AFQjCNE4O9eAfKha42K3GQBSgj4C3hVF4w){.c19}</span>

<span class="c2 c0"></span>
