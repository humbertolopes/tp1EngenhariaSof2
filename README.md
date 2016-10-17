UNIVERSIDADE FEDERAL DE MINAS GERAIS

INSTITUTO DE CIÊNCIAS EXATAS

DEPARTAMENTO DE CIÊNCIA DA COMPUTAÇÃO

**CANVAS BY INSTRUCTURE **

**Alunos:**

César Augusto Moura Ferreira

Humberto Lopes

1)  **Descrição do sistema**

Instructure Canvas é um sistema de gerenciamento de aprendizagem que
fornece diversos serviços para acompanhar o progresso de alunos a partir
de uma única interface. Dentre tais serviços, apresenta -se a submissão
e correção de atividades, quizzes online, integração de conteúdo
multimídia, entre outros.

O sistema desenvolvido pela empresa Instructure, foi construído sobre a
crença de que todos na educação devem ter livre acesso à informação de
alta qualidade, conteúdo, dados , recursos e acompanhar o desenvolvido
dos alunos que utilizam essa plataforma.

Canvas é construído sobre uma API aberta, ou seja, os usuários têm
acesso programático para o nosso software. Isto permite integrar
ferramentas personalizadas, extrair os dados de uso e descobrir novas e
excitantes formas de usar Canvas.

Canvas integra com a maioria dos (Sistemas de Informação do estudante)
SISS, nós trabalhamos com mais de 100 parceiros afins para garantir que
a tecnologia, ferramentas e serviços estejam disponíveis para ajudá-los
a construir o seu ecossistema de aprendizagem ideal.

O código dobrado no núcleo da Canvas não é trivial. Em uma segunda
versão, uma forma de melhorar seria implementar como um serviço
separado, usando a API ou LTI. Temos um alto padrão de qualidade em
Instructure e se você não estiver familiarizado com Ruby Rails, ter o
seu código aceito pela Instructure pode ser uma tarefa difícil..

Cada commit para Canvas é revisado por um enge. Cada linha é lida e o
revisor é responsável testá-lo em seu ambiente local e commitar. O que é
validado pelo engenheiro:

-   Confira e tentar o conjunto de alterações.

-   Certifique-se de que a mensagem de commit tem um plano de teste.

-   Certifique-se de que o plano de testes e teste de cobrir todos os
    casos necessários.

-   Certifique-se de que o código segue as convenções de codificação
    da linguagem.

-   Certifique-se de que o código é bem desenhado e arquitetado.

-   Certifique-se de que todas as cadeias / datas / horários / números
    voltados para o usuário são
    internacionalizada
    (https://github.com/instructure/canvas-lms/wiki/I18n).

Outros fatores que devem ser considerados:

-   Deve permanecer alto desempenho sob carga pesada.

-   Deve trabalhar em um ambiente multi-tenant. Mais sobre isso em um
    minuto, mas basicamente melhorias deve ser construído usando a
    arquitetura de plug-in de Canvas.

-   Deve ser acessível aos leitores de tela e outros dispositivos de
    tecnologia assistiva

-   Deve seguir o [estilo de
     codificação](https://github.com/instructure/canvas-lms/wiki/code-styleguides)[](https://github.com/instructure/canvas-lms/wiki/code-styleguides)

Melhorias e extensões
---------------------

Porque Canvas nuvem é executado como um ambiente *multi-tenant*,
quaisquer alterações no código base irá afectar todas as instituições de
uma só vez. Se você estiver olhando para adicionar grandes pedaços de
funcionalidade para Canvas, você precisa manter isso em mente, já que
provavelmente apenas algumas instituições vão querer que a
funcionalidade adicionada.

Para ajudar com isso nós construímos a noção de Plugins em Canvas.
Plugins podem ser registrados em tempo de execução, mas só aparecem na
interface para contas de raiz ativados. Há alguns lugares no código que
já foram instrumentados para plugins (como conferências web e
colaborações), mas se você estiver olhando para estender a
funcionalidade em outro lugar, em seguida, o primeiro passo vai ser
*pluginifying* que parte do código, em seguida, a construção de um
plug-in para sua implementação específica.

![](media/imagem1.png)

**2) Informações da equipe de desenvolvimento**

![](media/img4.png)

![](media/img5.png)

Canvas é um novo e open-source desenvolvido em 2011 pela equipe da
Instructure Inc. A Instructure, adota um modelo simples. Ela possui a
tecnologia mas em termos de código aberto. Ela é responsável pela
manutenção e desenvolvimento da árvore da código fonte , mas oferece um
modelo de dual licenciamento . Este modelo dual-licenciamento permite um
sério compromisso com a abertura do código, mas ao mesmo tempo ter um
estábulo e negócio rentável para apoiar uma mudança real na indústria.

Qualquer 1 pode contribuir com o projeto. Para contribuir com o
desenvolvimento do Canvas é necessário assinar [o acordo de
contribuição](https://github.com/instructure/canvas-lms/wiki/ica.pdf) e
antes de aceitar uma solicitação de desenvolvimento é necessário ler as
informações de [Diretrizes para
Codificação](https://github.com/instructure/canvas-lms/wiki/Coding-Guidelines).

![](media/img2.png)


**3) Breve descrição da evolução do sistema: principais releases**

Uma nova versão do Canvas é lançado a cada três semanas. Muitas vezes,
os novos lançamentos incluem novas características impressionantes, e
estes são quase sempre fácil de usar. Menos frequentemente, Canvas
modifica características existentes em maneiras que você pode não
gostar. Infelizmente, os usuários são mais propensos a notar mudanças
que os afetam negativamente.

Instructure trabalha duro para manter a interface do usuário em tela
semelhante o suficiente de uma versão para a próxima que as mudanças não
vai ser incapacitante, de fato, a maioria das vezes as pessoas nem
sequer notar as mudanças. Isso pode ser bom e ruim. Bom, porque os seus
fluxos de trabalho antigo continuará a trabalhar. Ruim, porque a
familiaridade da interface disfarça o fato de que as grandes novas
opções têm aparecido.

**Principais Releases nos últimos meses**

-   **Atribuições diferenciadas** -
  missões do Canvas pode agora ser alvo não só do curso seções e grupos de curso, mas os estudantes individuais.

-   **Eventos recorrentes** -
    Ao criar um novo evento no calendário, os usuários podem optar por
    criar várias cópias do evento a cada dia, semana ou mês.

-   **Atribuições
     dispensado** -
    Um indivíduo pode agora ser dispensado de qualquer atribuição.
    Basta atribuir uma «classe» de EX.

-   **Marcar como feita** -
    Os professores podem atribuir marca como feito como um requisito
    do módulo para as atribuições e as páginas do curso. Essa mudança
    ajuda os alunos a manter o controle de seu progresso em módulos.
    Por exemplo, um instrutor pode querer um aluno para rever uma
    página várias vezes antes de avançar para o próximo item do
    módulo, ou a exigência também pode ser usado em tarefas que são
    puramente para a auto estudando.

-   **Encomenda do calendário
     Colors** -
    Canvas permite aos usuários definir suas próprias cores para cada
    calendário na sua conta. Canvas irá atribuir uma cor arbitrária
    para cada calendário, a menos que uma cor personalizada
    é escolhida. Cada calendário contém 15 cores padrão, mas os
    usuários podem inserir um código Hex para criar qualquer cor de
    sua escolha.

-   **Colunas Boletim
     persistentes**-
    Canvas salva preferências Boletim costume de um usuário e
    associa-los com o perfil do usuário. Essa alteração permite que os
    utilizadores de reorganizar uma coluna no Boletim, incluindo o
    tamanho da coluna, e que as alterações persistem em qualquer
    computador ou navegador. Este recurso diz respeito apenas às
    colunas de atribuição no Boletim.

-   **Como
     ícone**-
     Os professores podem criar discussões e permitir que os estudantes
    para indicar "gostava" respostas de discussão.

-   **Anonymous Peer
    Review** -
    Os professores podem optar por criar avaliações pelos pares com
    respostas anônimas. Localizado nas opções de avaliação pelos pares
    e trabalhos e discussões classificados, a opção de anonimato
    permite que os instrutores para ocultar o nome do revisor
    estudante do aluno com a apresentação.

**4) Principais frameworks, ferramentas e linguagens usadas no
desenvolvimento.**

Instructure Inc. foi criada a fim de apoiar o desenvolvimento contínuo
de um novo sistema de gestão de aprendizagem
([*LMS*](https://en.wikipedia.org/wiki/Learning_management_system))
originalmente chamado Instructure. Uma vez incorporados, os fundadores
mudou o nome do software a Canvas. A companhia sediada em Utah testaram
os *LMS* em várias escolas locais, incluindo [*Utah State
University*](https://en.wikipedia.org/wiki/Utah_State_University) *e*
[*da Universidade Brigham
Young*](https://en.wikipedia.org/wiki/Brigham_Young_University) antes de
lançar oficialmente Canvas.

Canvas foi construído usando [*Ruby on
Rails*](https://en.wikipedia.org/wiki/Ruby_on_Rails) como o framework de
aplicações web apoiado por uma
[*PostgreSQL*](https://en.wikipedia.org/wiki/PostgreSQL) banco de dados.
Ele incorpora [*JQuery*](https://en.wikipedia.org/wiki/JQuery) ,
[*HTML5*](https://en.wikipedia.org/wiki/HTML5) e
[*CSS3*](https://en.wikipedia.org/wiki/CSS3) para fornecer uma interface
de usuário moderna. [OAuth](https://en.wikipedia.org/wiki/OAuth) é usado
para fornecer acesso limitado às informações de um usuário em
determinados sites de mídia social como
[Facebook](https://en.wikipedia.org/wiki/Facebook) e
[Twitter](https://en.wikipedia.org/wiki/Twitter) para permitir a
colaboração entre sites. Canvas funciona como um [software como um
serviço](https://en.wikipedia.org/wiki/Software_as_a_service) usando [o
Amazon Web Services](https://en.wikipedia.org/wiki/Amazon_Web_Services)
na "nuvem".

[*Ruby on Rails*](https://en.wikipedia.org/wiki/Ruby_on_Rails) é um
[framework](https://pt.wikipedia.org/wiki/Framework)
[livre](https://pt.wikipedia.org/wiki/Software_livre) que promete
aumentar velocidade e facilidade no desenvolvimento de sites orientados
a banco de dados (*database-driven web sites*), uma vez que é possível
criar aplicações com base em estruturas pré-definidas. Frequentemente
referenciado como **Rails** ou **RoR**, o Ruby on Rails é um projeto de
código aberto escrito na linguagem de programação
[Ruby](https://pt.wikipedia.org/wiki/Ruby_(linguagem_de_programa%C3%A7%C3%A3o)).
As aplicações criadas utilizando o framework Rails são desenvolvidas com
base no padrão de arquitetura [MVC](https://pt.wikipedia.org/wiki/MVC)
(*Model*-*View*-*Controller*).

*HTML5* ([Hypertext Markup
Language](https://pt.wikipedia.org/wiki/Hypertext_Markup_Language),
versão 5) é uma linguagem para estruturação e apresentação de conteúdo
para a [World Wide Web](https://pt.wikipedia.org/wiki/World_Wide_Web) e
é uma tecnologia chave da Internet originalmente proposto por [Opera
Software](https://pt.wikipedia.org/wiki/Opera_Software).[^\[1\]^](https://pt.wikipedia.org/wiki/HTML5#cite_note-1)
É a quinta versão da linguagem
[HTML](https://pt.wikipedia.org/wiki/HTML). Esta nova versão traz
consigo importantes mudanças quanto ao papel do HTML no mundo da Web,
através de novas funcionalidades como semântica e acessibilidade.
Possibilita o uso de novos recursos antes possíveis apenas com a
aplicação de outras tecnologias. Sua essência tem sido melhorar a
linguagem com o suporte para as mais recentes multimídias, enquanto a
mantém facilmente legível por seres humanos e consistentemente
compreendida por computadores e outros dispositivos
([navegadores](https://pt.wikipedia.org/wiki/Navegadores), parsers etc).
O HTML5 será o novo padrão para
[HTML](https://pt.wikipedia.org/wiki/HTML),
[XHTML](https://pt.wikipedia.org/wiki/XHTML), e HTML DOM. Atualmente,
está em fase de esboço, porém diversos navegadores já implementam
algumas de suas funcionalidades.

Após seus predecessores imediatos HTML 4.01 e XHTML 1.1, HTML5 é uma
resposta à observação de que o HTML e o XHTML, de uso comum na [World
Wide Web](https://pt.wikipedia.org/wiki/World_Wide_Web), é uma mistura
de características introduzidas por várias especificações, juntamente
com aquelas introduzidas por software, tais como os navegadores, aqueles
estabelecidos pela prática comum, e os muitos erros de sintaxe em
documentos existentes na web. É, também, uma tentativa de definir uma
única linguagem simples de marcação que possa ser escrita em HTML ou em
sintaxe XHTML. Isso inclui modelos de processamento detalhados para
incentivar implementações mais interoperáveis; isso estende, melhora e
racionaliza a marcação disponível para documentos, e introduz marcações
e [interfaces de programação de
aplicativos](https://pt.wikipedia.org/wiki/API) (APIs) para aplicações
web complexas. Pelas mesmas razões, HTML5 também é um candidato em
potencial aplicações multi-plataforma móveis. Muitos recursos do HTML5
tem sido construídos com a consideração de ser capaz de executar em
dispositivos de baixa potência como
[smartphones](https://pt.wikipedia.org/wiki/Smartphone) e
tablets.[^\[2\]^](https://pt.wikipedia.org/wiki/HTML5#cite_note-diff-2)

Em particular, HTML5 adiciona várias novas funções sintáticas. Elas
incluem as tags de&lt;video&gt;,&lt;audio&gt;,&lt;header&gt; e
elementos&lt;[canvas](https://pt.wikipedia.org/wiki/Canvas_(HTML5))&gt;,
assim como a integração de conteúdos
[SVG](https://pt.wikipedia.org/wiki/SVG) que substituem o uso de
tags&lt;object&gt; genéricas. Estas funções são projetadas para tornar
mais fácil a inclusão e a manipulação de conteúdo gráfico e multimídia
na web sem ter de recorrer a
[plugins](https://pt.wikipedia.org/wiki/Plugins)[proprietários](https://pt.wikipedia.org/wiki/Software_propriet%C3%A1rio)
e APIs. Outros novos elementos, como
&lt;section&gt;,&lt;article&gt;,&lt;header&gt; e&lt;nav&gt;, são
projetados para enriquecer o conteúdo semântico dos documentos. Novos
atributos têm sido introduzidos com o mesmo propósito, enquanto alguns
elementos e atributos têm sido removidos. Alguns elementos,
como&lt;a&gt;, e&lt;menu&gt; têm sido mudados, redefinidos ou
padronizados. As APIs e os modelos de objetos de documentos
([DOM](https://pt.wikipedia.org/wiki/Modelo_de_Objeto_de_Documentos))
não são mais pensamentos retrógrados, mas são partes fundamentais da
especificação do HTML5. HTML5 também define com algum detalhe o
processamento necessário para que erros de sintaxe de documentos
inválidos sejam tratados uniformemente por todos os browsers e outros
agentes de usuários em conformidade com o HTML5.

jQuery é uma
[biblioteca](https://pt.wikipedia.org/wiki/Biblioteca_(computa%C3%A7%C3%A3o))
[JavaScript](https://pt.wikipedia.org/wiki/JavaScript)
[cross-browser](https://pt.wikipedia.org/wiki/Cross-browser)
desenvolvida para simplificar os
[scripts](https://pt.wikipedia.org/wiki/Linguagem_de_script) [client
side](https://pt.wikipedia.org/wiki/Client_side) que interagem com o
[HTML](https://pt.wikipedia.org/wiki/HTML).[^\[^](https://pt.wikipedia.org/wiki/JQuery#cite_note-1)
Ela foi lançada em dezembro de
[2006](https://pt.wikipedia.org/wiki/2006) no
[BarCamp](https://pt.wikipedia.org/wiki/BarCamp) de [Nova
York](https://pt.wikipedia.org/wiki/Nova_York) por John Resig. Usada por
cerca de 77% dos 10 mil sites mais visitados do mundo, jQuery é a mais
popular das bibliotecas
JavaScript.[](https://pt.wikipedia.org/wiki/JQuery#cite_note-3)

jQuery é uma biblioteca de [código
aberto](https://pt.wikipedia.org/wiki/C%C3%B3digo_aberto) e possui
[licença dual](https://pt.wikipedia.org/wiki/Licen%C3%A7a_dual), fazendo
uso da [Licença MIT](https://pt.wikipedia.org/wiki/Licen%C3%A7a_MIT) ou
da [GNU General Public
License](https://pt.wikipedia.org/wiki/GNU_General_Public_License)
versão 2. A sintaxe do jQuery foi desenvolvida para tornar mais simples
a navegação do documento HTML, a seleção de elementos
[DOM](https://pt.wikipedia.org/wiki/Document_Object_Model), criar
animações, manipular eventos e desenvolver [aplicações
AJAX](https://pt.wikipedia.org/wiki/AJAX_(programa%C3%A7%C3%A3o)). A
biblioteca também oferece a possibilidade de criação de
[plugins](https://pt.wikipedia.org/wiki/Plugin)sobre ela. Fazendo uso de
tais facilidades, os desenvolvedores podem criar camadas de
[abstração](https://pt.wikipedia.org/wiki/Abstra%C3%A7%C3%A3o_(programa%C3%A7%C3%A3o))
para interações de mais baixo nível, simplificando o desenvolvimento de
aplicações web dinâmicas de grande complexidade.

A [Microsoft](https://pt.wikipedia.org/wiki/Microsoft) e a
[Nokia](https://pt.wikipedia.org/wiki/Nokia) anunciaram planos de
incluir o jQuery em suas plataformas, a Microsoft adotando-a
inicialmente no [Visual
Studio](https://pt.wikipedia.org/wiki/Visual_Studio) para uso com o
framework AJAX do [ASP.NET](https://pt.wikipedia.org/wiki/ASP.NET), e a
Nokia na sua plataforma Web Run-Time de widgets. A biblioteca jQuery
também tem sido usada no
[MediaWiki](https://pt.wikipedia.org/wiki/MediaWiki) desde a versão
1.16.[](https://pt.wikipedia.org/wiki/JQuery#cite_note-8)

**5) Documentação da arquitetura**

A nuvem de Canvas arquitetura construída no Amazon Web Services
infra-estrutura fornece inigualável disponibilidade, escalabilidade e
confiabilidade. A arquitetura Canvas e a AWS infra-estrutura são
totalmente escalável horizontalmente fornecendo capacidade praticamente
ilimitada através do provisionamento de recursos adicionais. Canvas
fornece:

-   Redundância de recursos de computação com a vigilância activa para a
    detecção de falhas e automatizados de failover

-   Ajuste de desempenho em tempo real via Automated provisionamento de
    recursos para responder às picos e momentos de pico de uso para
    minimizar a degradação do desempenho

-   A proteção de dados através da replicação de dados, backup /
    restauração e recuperação de desastres procedimentos

-   Carga equilibrada servidores de aplicativos e dados em cache
   agressivo para web superiores desempenho

-   Rolar cronograma de lançamento de atualizações e upgrades, raramente
    incorrer em tempo de inatividade do sistema.

Canvas foi projetado especificamente para jogar bem com outras
tecnologias baseadas em padrões tais como Ferramentas IMS Global de
Aprendizagem para Interoperabilidade (LTI), permitindo Canvas para se
integrar perfeitamente com ferramentas best-of-breed. Com esta abordagem
e arquitetura, Canvas será sempre beneficiar da sua posição na vanguarda
da LMS inovações por prontamente incorporando novas e melhores
ferramentas, enquanto supressão progressiva e substituir tecnologias
obsoletas.

**Características de Canvas e Funções**

**Accessibility:** Adere a Seção 508 padrões de acessibilidade dos EUA,
e está comprometida com a Web. Iniciativa de Acessibilidade (WAI) para
conteúdo (WCAG) e aplicações ricas para internet (ARIA), conforme
documentado no nosso Voluntary Product Accessibility Template (VPAT)

**Analytics**: Monitoramento dos alunos, prediz o sucesso, e acompanha
os resultados de aprendizagem dos alunos e progresso por metas
pedagógicas e resultados desejados.

**Announcements**: Emitido automaticamente para o fluxo de todos os
usuários e outros canais de comunicação de atividades do curso, com base
nas preferências de notificação individuais dos usuários.

**Assignments**: Trabalhos Enviados pode incluir páginas web, documentos
do Word, vídeo, áudio, apresentações de slides,links, e mais

**Browser-enabled**: Compatível com as últimas duas versões do Apple
Safari, Google Chrome, Internet Microsoft, Explorer e Mozilla Firefox.

**Calendar**: Arrastar e soltar funcionalidade para agendar e remarcar
eventos no calendário.

**Chat**: Síncrona de textos para dentro de uma comunidade de
aprendizagem

**Collaborations**: Permitir que os usuários colaborem em projetos que
usam espaços de trabalho compartilhados Canvas.

**Conferences**: Webinars síncronas /videoconferência, e chat ao vivo
integrada

**Discussions**: Fornece assíncronos com fóruns de discussão graduáveis
de mídia rica para cursos e grupos

**ePortfolios:** Os alunos podem criar ePortfolios públicos ou privados
para exibir e refletir sobre cursos notável.

**FERPA and COPPA compliant:** Em conformidade com a lei federal dos EUA
sobre Direitos Familiares Educação Lei de Privacidade (FERPA) e Online
Privacy Protection Act de Crianças (COPPA) e dá às escolas as
ferramentas que precisam para manter a conformidade

**Files repository:** Hierárquica criação de pasta de arquivo e
organização, importação de arquivos zip e exportação, o bloqueio de
arquivos, dragand-drop reorganização de arquivos, renomear arquivos,
exclusão de arquivo, e outras de gerenciamento de arquivos padrão
funcionalidade

**Gradebook:** geradas automaticamente e atualizadas com base em tarefas
e avaliações do curso, ligada ao livro de notas de pontuação e integrado
com características de feedback e de notificação inteligentes
