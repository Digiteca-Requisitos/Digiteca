# Projeto Disciplina: Requisitos de Software

[](https://github.com/PedroBiklho/requisitos-software#projeto-disciplina-requisitos-de-software)

Olá! Este repositório faz parte do projeto da disciplina de Requisitos de Software da UTFPR - Campus Cornélio Procópio.

Link do Padlet: https://padlet.com/joaomarcosalcala123/kanban-8ij5jcvmiyhbrknr

## 1. Introdução

[](https://github.com/PedroBiklho/requisitos-software#1-introdu%C3%A7%C3%A3o)

_**1.1. Nome do Grupo**_

MATEUS CASTRO DA CUNHA  - https://github.com/Mateuscastroc  
PEDRO HENRIQUE DE OLIVEIRA BICALHO - https://github.com/PedroBiklho  
MURILO HOLZLE DE MORAES - https://github.com/murilo-holzle  
JOAO MARCOS ARAUJO ALCALA - https://github.com/joaomarcosaa  

_**1.2. Nome do Sistema**_

Digiteca

_**1.3. Propósito do Sistema**_

O objetivo do sistema é criar uma plataforma digital para cadastro e empréstimo de livros, com foco em automatizar e facilitar o processo, especialmente em instituições educacionais onde, atualmente, esse processo ainda é feito de forma analógica.

_**1.2. Público Alvo**_

Alunos, Educadores, bibliotecas e instituições educacionais.

_**1.3. Descrição dos usuários**_

O sistema será utilizado por diferentes perfis de usuários finais, todos vinculados ao ambiente educacional. Cada grupo de usuários terá permissões e funcionalidades específicas, de acordo com suas necessidades e responsabilidades no processo de empréstimo e gestão de livros.

_**Personas:**_

_<Imagem, arquivo (PDF), link com as Personas.>_

_**Análise da situação atual: antes da introdução de sua solução**_

_`1. O que as pessoas fazem?`_  _`2. Quais os artefatos envolvidos?`_  _`3. O que elas precisam saber?`_

_**Análise das tarefas depois: como serão executadas as suas tarefas com sua solução:**_

_`1. O que as pessoas fazem?`_  _`2. Quais os artefatos envolvidos?`_  _`3. O que elas precisam saber?`_

_**Cenário: Antes**_

_<Preencher com o cenário idealizado antes da aplicação do seu sistema.>_

_**Cenário: Depois**_

_<Preencher com o cenário idealizado depois da aplicação do seu sistema.>_

## 2. Documentos gerais no repositório

[](https://github.com/PedroBiklho/requisitos-software#2-documentos-gerais-no-reposit%C3%B3rio)

_**2.1. Requisitos Funcionais**_

|Identificador   | Descrição                             |Prioridade    |Depende       |
|----------------|---------------------------------------|--------------|--------------|
| RF01           | O sistema deve permitir o cadastro de novos usuários com dados obrigatórios (nome, e-mail, senha).|Alta | Nenhuma     |
| RF02           | O sistema deve autenticar usuários através de login com e-mail e senha.|Alta | RF01 |
| RF03           | O sistema deve somente realizar emprestimos de livros para usuários cadastrados.|Alta | RF01, RF02 |
| RF04 | O sistema deve permitir o cadastro de livros (título, autor, ano, categoria, código único).|Alta | Nenhuma |
| RF05 | O sistema deve permitir a consulta de livros cadastrados e mostrar status (disponível, emprestado, reservado). | Alta | RF03|
| RF06 | O sistema deve registrar o empréstimo de um livro, vinculando usuário, livro e data de devolução. | Alta | RF03, RF04| 
| RF07 | O sistema deve registrar a devolução de um livro, atualizando o status para disponível. | Alta | RF05 |
| RF08 | O sistema deve manter um histórico de todos os empréstimos realizados por cada usuário. | Média | RF05, RF06 |
| RF09 | O sistema deve enviar notificações sobre a proximidade da data de devolução dos livros. | Média | RF05 |
| RF010 | O sistema deve permitir a reserva de livros que estejam emprestados. | Média | RF04, RF05|



_**2.2. Requisitos Não Funcionais**_

|Identificador   | Descrição                             |Prioridade    |
|----------------|---------------------------------------|--------------|
| RN01 |O aplicativo deve estar em conformidade integral com a Lei Geral de Proteção de Dados (Lei nº 13.709/2018) e regulamentos correlatos, assegurando tratamento, armazenamento, segurança e compartilhamento de dados pessoais conforme princípios e bases legais vigentes.| Alta |
| RN02 |O usuário deve conseguir concluir a locação e a devolução de um livro em, no máximo, 10 interações (cliques ou toques) a partir da tela inicial, em condições usuais de uso.| Média |
| RN03 | As listagens do sistema devem ser exibidas em até 10 segundos a partir da solicitação, sob condições normais de operação. | Média |
| RN04 | O sistema deve operar corretamente nos principais navegadores suportados (Chrome, Firefox, Safari e Edge), nas versões atualmente mantidas pelos respectivos fabricantes. | Alta |
| RN05 | As falhas críticas do sistema devem ser registradas automaticamente em logs centralizados, com tempo de resposta para análise em até 24 horas. | Média |
| RN06 | O sistema deve criptografar todas as comunicações entre cliente e servidor utilizando protocolo HTTPS (TLS 1.2 ou superior). | Alta |
| RN07 | O aplicativo deve estar disponível para uso em pelo menos 99,5% do tempo em cada mês, excluindo janelas programadas de manutenção. | Alta |
| RN08 | A interface do usuário deve seguir as diretrizes de acessibilidade, garantindo uso adequado por pessoas com deficiência. | Alta |
| RN09 | O sistema deve suportar, simultaneamente, pelo menos 500 usuários ativos em bibliotecas de médio porte, sem degradação perceptível de desempenho. | Alta |
| RN10 | O aplicativo deve ser compatível com dispositivos móveis Android (versão 10 ou superior) e iOS (versão 14 ou superior), bem como oferecer versão web responsiva | Média |

_<Link, imagem, arquivo com os requisitos não funcionais.>_

_**2.3. Perguntas**_

_<Arquivo com as perguntas realizadas na entrevista .>_

_**2.4. Entrevista**_

_<Arquivo com as respostas do indivíduo entrevistado e link do drive com upload da gravação.>_

_**2.5. Histórias do Usuário**_

_<Imagem, arquivo (PDF), link com as Histórias de Usuário.>_

_**2.6. Diagramas de Caso de Uso e Especificações**_

_<Imagem, arquivo (PDF), link com Diagrama de Caso de Uso.>_

_**2.7. Diagramas de Atividades**_

_<Imagem, arquivo (PDF), link com Diagrama de Atividades.>_

_**2.8. Protótipos**_

_<Imagem, arquivo (PDF), link com Protótipo.>_

## Referências

[](https://github.com/PedroBiklho/requisitos-software#refer%C3%AAncias)

_<Esta seção é destinada à descrição das referências utilizadas pelo documento, como por exemplo, URLs e livros. Ver exemplo a seguir:>_

[1] “Glossário da  _USina_”, <_id_doc glossário_>, Versão <_versão_>. Localização: <_localização_>.
