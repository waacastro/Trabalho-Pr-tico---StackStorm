Este trabalho é um projeto da disciplina de Engenharia de Software II da
Universidade Federal de Minas Gerais, Departamento de Ciência da
Computação. Feito pelos alunos Cláudio Manuel, Tauany Santos e Wallace
Augusto, em Maio de 2017.

O objetivo do projeto é fazer uma documentação de um sistema open
source, hospedado no GitHub e que seja popular (com mais de 1000
estrelas).

Foi escolhido o sistema StackStorm, uma plataforma que realiza a
integração entre serviços de padrões operacionais comum.

1.  **Descrição do Sistema**

    1.  **Características e objetivo**

O StackStorm é uma plataforma de automação de código aberto que realiza
a integração entre serviços e ferramentas de padrões operacionais
comuns. O foco principal da plataforma é tomar ações em resposta a
eventos que ocorrem. Além disso, tem por objetivo proporcionar aos seus
usuários uma forma organizada de conectar todos os aplicativos, serviços
e fluxos de trabalho que ele utiliza de uma forma mais simples, tornando
mais facilmente esse ambiente automatizado.

A plataforma é composta por Sensors, Triggers, Actions, Rules,
Workflows, Packs e Audit Trail, todos estes componentes em conjunto
realizam a conexão dos serviços e fluxos de trabalho.

-   Os Sensors são plugins que fazem a integração da entrada e saída
    de eventos.
-   Os Triggers são representações de eventos externos. É possível
    definir um novo disparador, para isso é necessários criar um novo
    plugin de sensor.
-   As Actions são plugins na linguagem Python ou qualquer outro script.
    Existem ações genéricas, por exemplo “ssh”, ou ações personalizadas.
    Essas ações podem ser chamadas diretamente pelo usuário, através de
    uma API, por exemplo. Além disso, podem ser usadas e chamadas como
    regra e fluxos de trabalho (tópicos que estão explicados abaixo).
-   As Rules desencadeiam ações. Elas aplicam critérios de correspond\
    ência e fazem um mapeamento para definir como será a entrada
    de ações.
-   Os Workflows definem a ordem e as condições de transações de dados.
    Em geral, são necessárias mais de uma ação para uma automação,
    quando ela possui mais de uma etapa. Os fluxos de trabalho podem ser
    chamados manualmente ou por regras.
-   Os Packs são unidades de implantação de conteúdo utilizadas para
    simplificar o gerenciamento e compartilhamento de conteúdos.
-    A Audit Trail de execução de ações pode ser manual ou automática, o
    usuário pode definir e a partir disso, é gravada e armazenada a
    ação, especificando o contexto e o resultado da execução.

O conteúdo que é armazenado na plataforma é todo em código. Além disso,
os Packs, que são as unidades de implantação de conteúdo podem ser
criados e compartilhados no GitHub ou enviados para o repositório da
comunidade StackStorm.

A licença utilizada pelo projeto é a Licença Apache que pode ser lida no
link abaixo:

[*Http://www.apache.org/licenses/LICENSE-2.0*](http://www.apache.org/licenses/LICENSE-2.0)

**1.2 Linguagem e Ferramenta**

A linguagem principal utilizada na plataforma é o Python que é a
linguagem utilizada para a criação dos plugins de Sensors e também para
os plugins de Actions. A linguagem Python é uma linguagem de programação
de alto nível, de script, imperativa e orientada a objetos. Além de
Python, outras linguagens são utilizadas nas contribuições de Packs,
como por exemplo a linguagem Shell e o Javascript.

Shell é uma linguagem interpretada, de script que é usada em diversos
sistemas operacionais com diversos dialetos. Assim como o Python,
Javascript é uma linguagem de script, orientada a objetos e é utilizada
para conectar os objetos do ambiente.

Uma ferramenta que é utilizada na plataforma é a “CloudSlang” que faz o
gerenciamento de aplicativos implantados. O objetivo do uso desta
ferramenta é automatizar rapidamente as operações de TI diárias e
definir um workflow estruturado e fácil de entender.

A “CloudSlang”, é um DSL que se baseia em uma linguagem YAML, que é
utilizada para realizar consultas complexas no banco de dados. Os
conteúdos da CloudSlang são divididos em dois tipos principais que são
as operações e os fluxos. Estas operações podem ser escritas em duas
linguagens diferentes, que são Java e Python.

Um outro mecanismo utilizado é o Jinja2 que é um modelo completo para a
linguagem Python. Ele é utilizado para gerenciar os workflows da
plataforma.

1.  **Equipe de Desenvolvimento**

O projeto StackStorm é uma plataforma de automatização que possui uma
versão open-source com suporte da comunidade. Seu desenvolvimento e
construção se fez através de uma comunidade no Slack. O Slack funciona
como uma rede social, através dele, qualquer pessoa pode criar uma sala
de bate-papo, com múltiplos canais, dentro de uma empresa, com assuntos
distintos e para grupos diferentes. Dentro de cada um desses canais, a
ferramenta permite troca de mensagens de texto, documentos e
compartilhamento de mídias, como fotos e vídeos.

Tanto o team principal quanto os diversos usuários e desenvolvedores
utilizam essa ferramenta para desenvolver a plataforma StackStorm, que,
no caso, já são mais de 200 pessoas envolvidas. Abaixo, a sua equipe de
fundação:

Dmitri Zimine

Chief Stormer & Co-Fundador

Ajudou a liderar a primeira onda de automação de operações enquanto
servia como arquiteto-líder e chefe de engenharia na Opalis.

Winson Chan

Stormer

Focado no desenvolvimento de produtos. Altamente qualificado na
concepção e desenvolvimento de autoatendimento, soluções automatizadas e
gerenciamento de pilhas VM na nuvem híbrida da empresa.

Patrick Hooboom

Stormer

Stormer focado em DevOps. Tem como objetivos alavancar as ferramentas de
gerenciamento de configuração e criar scripts personalizados para
melhorar os processos em toda a organização.

> Lakshmi Kannan

Stormer

Responsável por construir uma plataforma previsível, de melhor
performance e utilizável. Anteriormente, trabalhou na Amazon e Rackspace
construindo sistemas altamente distribuídos e de baixa latência.

Manas Kelshikar

Stormer

Desenvolvedor da plataforma. Trabalhos anteriores na VMware como membro
da equipe de clientes vSphere, onde contribuiu para a arquitetura e
implementação do produto de nova geração.

Tomaz Muraus

Stormer

Auxilia na construção da plataforma. Trabalhou anteriormente na
Cloudkick, Rackspace e DivyCloud como desenvolvedor e operando sistemas
altamente distribuídos.
