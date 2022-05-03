# Lista 2: Introdução à programação orientada a objetos em C++
<sub>Última atualização: 02/05/2022</sub>

## Sumário
- [Visão geral e objetivos](#visão-geral-e-objetivos)  
- [Tarefas](#tarefas)
- [Requisitos](#requisitos)
- [Boas práticas de programação](#boas-práticas-de-programação)
- [Autoria e política de colaboração](#autoria-e-política-de-colaboração)
- [Entrega](#entrega)
- [Avaliação](#avaliação)
- [Dúvidas e informações](#dúvidas-e-informações)

## Visão geral e objetivos
O objetivo desta lista de exercícios é colocar em prática as habilidades de **interpretar especificações de problemas e realizar abstrações** para projetar e implementar uma soluções na forma de programas na linguagem de programação C++, utilizando o paradigma de **programação orientada a objetos**. Para tanto, esta lista explora elementos fundamentais desse paradigma em C++, como classes, objetos, construtores e destrutores, além de outros recursos tradicionais da linguagem, tais como laços, estruturas condicionais simples e compostas, tipos de dados básicos e heterogêneos, expressões lógicas, passagem de parâmetros, leitura de escrita de informações a partir da entrada e saída padrão, dentre outros.

De forma adicional, esta lista de exercícios também aborda elementos da [*Standard Template Library* (STL)](https://en.wikipedia.org/wiki/Standard_Template_Library). A STL integra a biblioteca da linguagem de programação C++ provendo um conjunto de classes referentes a estruturas de dados comuns como vetor, lista, pilha, etc. (*containers*), bem como algoritmos e iteradores para operarem sobre tais estruturas. Todos esses elementos são genéricos, sendo, portanto, capazes de lidar com quaisquer tipos de dados.

## Tarefas
As tarefas centrais a serem realizadas neste trabalho consistem em projetar e implementar, em C++, programas para cada um dos seguintes problemas:

1. [Casa & Rua](https://github.com/bti-ufrn-lp1/lista02/tree/master/casa_rua)

A descrição de cada um desses problemas está em seu respectivo diretório, juntamente com exemplos de entradas e saídas esperados para o programa (se for o caso) e uma relação dos recursos da linguagem de programação C++ necessários à implementação da solução. O código fonte das soluções implementadas deverá constar nos respectivos diretórios.

Cada projeto já está preparado para ser compilado individualmente com o uso de `cmake`. Para que seja possível usufruir da infraestrutura de compilação e teste disponível, **não se deve alterar outros arquivos que não sejam aqueles indicados**. De maneira geral, é importante seguir à risca as instruções sobre a implementação dos exercícios, uma vez que as respostas serão validadas de forma automatizada. Preferencialmente, não se deve realizar qualquer modificação nos testes automatizados, a memos que seja acordado com o docente.

Por fim, caso se deseje criar outros arquivos fonte para melhor modularizar o programa, é necessário alterar o *script* do `cmake` corespondente para incluir o novo arquivo fonte na lista de dependências do alvo `${APP_NAME}` com o comando `target_sources(${APP_NAME} PRIVATE "nome_arquivo.cpp")`.

## Requisitos
Para que seja possível compilar e executar os testes preparados para este trabalho, é necessário que os seguintes elementos estejam instalados no ambiente de desenvolvimento:

- [Git](https://git-scm.com), como sistema de controle de versões
- [*GNU Compiler Collection*](https://gcc.gnu.org) (a qual inclui o compilador `g++`), [`clang`](https://clang.llvm.org/) ou qualquer outro compilador para a linguagem C++
- [`cmake`](https://cmake.org/), para gerar *makefiles* automaticamente e de forma otimizada para o projeto
- [Python 3+](https://www.python.org/), para executar o *script* de teste de comparação de saída gerada/esperada

## Boas práticas de programação
Boas práticas de programação deverão ser constantemente aplicadas no desenvolvimento das soluções aos problemas propostos. Os programas deverão ser codificados de forma legível (com indentação de código fonte, nomes consistentes, etc.) e documentados adequadamente na forma de comentários. O código fonte deverá ainda ser anotado para dar suporte à geração automática de documentação utilizando a ferramenta [Doxygen](https://www.doxygen.nl/). O documento de apoio disponível neste [link](https://drive.google.com/file/d/1YA1KxASCNY3B8APowD2V0sL-kAso9g86/view) contém algumas instruções acerca do padrão de documentação e uso do Doxygen. **Cada projeto deverá ter sua documentação específica**, de forma separada dos demais.

As soluções deverão ser desenvolvidas com qualidade, garantindo que o programa funcione de forma correta e eficiente. Deve-se também pensar nas possíveis entradas que poderão ser utilizadas para testar apropriadamente cada programa, além de serem tratadas adequadamente possíveis entradas consideradas inválidas. A execução dos testes automatizados é útil para identificar esses tipos de casos.

## Autoria e política de colaboração
**Este trabalho deverá necessariamente ser realizado em equipe composta de dois estudantes**, sendo importante, dentro do possível, dividir as tarefas igualmente entre os integrantes da equipe. Após a implementação das soluções para os problemas propostos, o arquivo [`author.md`](https://github.com/bti-ufrn-lp1/lista02/blob/master/author.md) presente no repositório deverá ser editado preenchendo as informações de identificação dos integrantes da equipe, na seção [Informações de Autoria](https://github.com/bti-ufrn-lp1/lista02/blob/master/author.md#identificação-de-autoria) e informando-se quais dos problemas foram solucionados com sucesso, na seção [Soluções Implementadas](https://github.com/bti-ufrn-lp1/lista02/blob/master/author.md#soluções-implementadas). 

O trabalho em cooperação entre estudantes da mesma turma ou de outras turmas é estimulado, sendo admissível a discussão de ideias e estratégias. Contudo, tal interação não deve ser entendida como permissão para utilização de (parte de) código fonte de colegas, o que pode caracterizar situação de plágio. Trabalhos copiados no todo ou em parte de outros colegas ou da Internet serão anulados e receberão nota zero.

## Entrega
O sistema de controle de versões [Git](https://git-scm.com) e o serviço de hospedagem de repositórios [GitHub](https://git-scm.com) serão utilizados para possibilitar a entrega das implementações realizadas. Para possibilitar a associação de repositórios Git para cada equipe e reuni-los sob uma mesma infraestrutura, foi criada uma atividade (*assignment*) no GitHub Classroom. Cada integrante de equipe deverá acessar este [*link*](https://classroom.github.com/a/ZJWRYHNc), aceitar o convite para ingressar no GitHub Classroom e finalmente seguir as instruções em tela para acessar a atividade e ingressar em uma equipe existente ou criar outra. Este [vídeo](https://youtu.be/ObaFRGp_Eko) demonstra como ocorre esse processo.

No momento de criação de uma equipe, o GitHub Classroom cria um repositório Git privado acessível unicamente pelos integrantes da equipe e pelo docente, sob a organização [`bti-ufrn-lp1`](https://github.com/bti-ufrn-lp1). Esse repositório segue a mesma estrutura de diretórios presentes neste repositório, o qual serve de *template*. Todos os arquivos deverão constar no repositório obedecendo **estritamente** a divisão em diretórios, ou seja, os códigos fonte referentes às soluções implementadas deverão estar nos respectivos diretórios de cada problema. A fim de garantir a boa manutenção do repositório, deve-se ainda configurar corretamente o arquivo `.gitignore` para desconsiderar arquivos que não devam ser versionados, a exemplo do diretório `build` e seus arquivos, resultantes do processo de compilação com o `cmake`.

A implementação das soluções para os problemas propostos neste trabalho deverá ser realizada **até as 23h59 do dia 13 de maio de 2022** no respectivo repositório Git da equipe. Para fins de registro, o endereço do repositório também deverá ser enviado através da opção *Tarefas* na Turma Virtual do SIGAA. **Não serão aceitos envios por outros meios ou repositórios que não sejam os descritos nesta especificação.**

## Avaliação
A avaliação de cada uma das soluções para os cinco problemas propostos contabilizará nota de até 10,0 pontos, correspondentes . As soluções implementadas serão avaliadas de acordo com os seguintes critérios: 

- utilização correta dos recursos providos pela linguagem de programação C++;
- modelagem adequada de classes e utilização correta de objetos;
- corretude da execução dos programas implementados, que devem apresentar saída em conformidade com a especificação e as entradas de dados fornecidas;
- aplicação de boas práticas de programação, incluindo legibilidade, organização e documentação de código fonte, e;
- correta utilização do repositório Git, no qual deverá ser registrado todo o histórico da implementação por meio de *commits*. 

O não cumprimento de algum dos critérios de avaliação especificados poderá resultar nos seguintes decréscimos, aplicados sobre a nota obtida até então na avaliação de cada solução:

| Falta | Decréscimo |
| :--- | ---: |
| Falta de comentários no código fonte e/ou de documentação gerada com Doxygen | -10% |
| Uso inadequado de controle de versão com Git | -20% |
| Falta de especificação ou especificação incorreta da autoria do trabalho (arquivo [`author.md`](https://github.com/bti-ufrn-lp1/lista01/blob/master/author.md)) | -20% |
| Implementação na linguagem C ou resultante de mistura entre as linguagens C e C++ | -30% |
| Código fonte com legibilidade prejudicada (por exemplo, com identação ou nomenclatura inadequada) | -40% |
| Programa compila com mensagens de aviso (*warnings*) | -50% |
| Modelagem orientada a objetos inadequada | -50% |
| Programa apresenta erros de compilação, não executa ou apresenta saída incorreta | -70% |
| Plagiarismo | -100% |

## Dúvidas e informações
Caso haja qualquer dúvida, questionamento ou necessidade de informação adicional, é possível:
- enviar *e-mail* para o endereço everton.cavalcante@ufrn.br;
- enviar mensagem privada diretamente ao docente, utilizando o servidor Discord;
- enviar mensagem no canal de texto `#geral-dim0120-t02`, especificamente associado à turma no servidor Discord;
- enviar mensagem no canal de texto `#duvidas` no servidor Discord, comum a todas as turmas da disciplina;
- realizar encontros síncronos presenciais, no horário e local de aula;
- agendar encontros síncronos por videoconferência, ou;
- agendar encontros síncronos pelo canal de áudio `Fale com Prof. Everton` no servidor Discord.
