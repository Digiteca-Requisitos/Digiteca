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


## Análise da Situação Atual (Antes da Digiteca)

### O que as pessoas fazem?
- *Alunos:* Vão presencialmente à biblioteca, consultam catálogos físicos ou perguntam aos bibliotecários sobre livros disponíveis, preenchem fichas de empréstimo manualmente
- *Professoras:* Visitam a biblioteca para verificar acervo, anotam informações em cadernos, fazem solicitações verbais ou por bilhetes aos bibliotecários

### Quais os artefatos envolvidos?
- Fichas de empréstimo em papel
- Catálogos físicos ou cadernos de registro
- Carimbos e carimbeiras para datas
- Cadernos de controle manual
- Bilhetes e anotações avulsas

### O que elas precisam saber?
- Localização física da biblioteca e horários de funcionamento
- Como usar o sistema de catalogação (CDD, por exemplo)
- Regras de empréstimo (prazos, quantidades, renovações)
- Como preencher fichas corretamente
- A quem se dirigir para diferentes solicitações

---

## Análise das Tarefas Depois (Com a Digiteca)

### O que as pessoas fazem?
- *Alunos:* Acessam o sistema via celular ou computador, buscam livros digitalmente, verificam disponibilidade em tempo real, fazem empréstimos/reservas online, recebem notificações automáticas
- *Professoras:* Consultam o acervo remotamente, criam listas de leitura, acompanham uso da biblioteca pelos alunos através de relatórios, comunicam-se com a biblioteca via sistema

### Quais os artefatos envolvidos?
- Smartphones, tablets ou computadores
- Aplicativo/site do Digiteca
- Notificações push ou por e-mail
- Dashboard com histórico e estatísticas
- QR codes para identificação rápida de livros

### O que elas precisam saber?
- Como acessar e fazer login no sistema
- Como pesquisar livros (palavras-chave, filtros)
- Como interpretar status dos livros (disponível, emprestado, reservado)
- Como gerenciar seus empréstimos e reservas
- Como configurar preferências de notificação

_**Cenário: Antes**_

_<Preencher com o cenário idealizado antes da aplicação do seu sistema.>_

_**Cenário: Depois**_

_<Preencher com o cenário idealizado depois da aplicação do seu sistema.>_

## 2. Documentos gerais no repositório

[](https://github.com/PedroBiklho/requisitos-software#2-documentos-gerais-no-reposit%C3%B3rio)

_**2.1. Requisitos Funcionais**_

|Identificador   | Descrição                             |Prioridade    |Dependência       | MoSCoW    |
|----------------|---------------------------------------|--------------|--------------|------------------|
| RF01           | O sistema deve permitir o cadastro de novos usuários com dados obrigatórios (nome, e-mail, senha).|Alta | Nenhuma     | M
| RF02           | O sistema deve autenticar usuários através de login com e-mail e senha.|Alta | RF01 | M
| RF03           | O sistema deve somente realizar emprestimos de livros para usuários cadastrados. Caso contrário, deverá aparecer a mensagem "Usuário não cadastrado."|Alta | RF01, RF02 | M
| RF04 | O sistema deve permitir o cadastro de livros (título 100 cacteres, autor 20 cacteres, ano, filtro por categoria, código único de até 5 digitos).|Alta | Nenhuma | M
| RF05 | O sistema deve permitir a consulta de livros cadastrados e mostrar status por filtro de disponível, emprestado e reservado. | Alta | RF03| M
| RF06 | O sistema deve registrar o empréstimo de um livro, vinculando usuário, livro e data de devolução. | Alta | RF03, RF04| M
| RF07 | O sistema deve registrar a devolução de um livro, atualizando o status para disponível. | Alta | RF05 | M
| RF08 | O sistema deve manter um histórico de todos os empréstimos realizados por cada usuário. | Média | RF05, RF06 | S
| RF09 | O sistema deve enviar notificações sobre a proximidade da data de devolução dos livros. | Média | RF05 | S
| RF10 | O sistema deve permitir a reserva de livros que estejam emprestados. | Média | RF04, RF05| C



_**2.2. Requisitos Não Funcionais**_

|Identificador   | Descrição                             |Prioridade    |Dependência       | MoSCoW    |
|----------------|---------------------------------------|--------------|------------------|-----------|
| RNF01 |O aplicativo deve estar em conformidade integral com a Lei Geral de Proteção de Dados (Lei nº 13.709/2018) e regulamentos correlatos, assegurando tratamento, armazenamento, segurança e compartilhamento de dados pessoais conforme princípios e bases legais vigentes.| Alta | Nenhuma | M
| RNF02 |O usuário deve conseguir concluir a locação e a devolução de um livro em, no máximo, 10 interações (cliques ou toques) a partir da tela inicial, em condições usuais de uso.| Média | RF05 | S
| RNF03 | As listagens do sistema devem ser exibidas em até 10 segundos a partir da solicitação, sob condições normais de operação. | Média | RF05 | S
| RNF04 | O sistema deve operar corretamente nos principais navegadores suportados (Chrome, Firefox, Safari e Edge), nas versões atualmente mantidas pelos respectivos fabricantes. | Alta | Nenhuma | M
| RNF05 | As falhas críticas do sistema devem ser registradas automaticamente em logs centralizados, com tempo de resposta para análise em até 24 horas. | Baixa | RF02 | C
| RNF06 | O sistema deve criptografar todas as comunicações entre cliente e servidor utilizando protocolo HTTPS (TLS 1.2 ou superior). | Alta | Nenhuma | M
| RNF07 | O aplicativo deve estar disponível para uso em pelo menos 99,5% do tempo em cada mês, excluindo janelas programadas de manutenção. | Alta | Nenhuma | M
| RNF08 | A interface do usuário deve seguir as diretrizes de acessibilidade, garantindo uso adequado por pessoas com deficiência. | Alta | Nenhuma | M
| RNF09 | O sistema deve suportar, simultaneamente, pelo menos 500 usuários ativos em bibliotecas de médio porte, sem degradação perceptível de desempenho. | Alta | RF02, RF05 | M
| RNF10 | O aplicativo deve ser compatível com dispositivos móveis Android (versão 10 ou superior) e iOS (versão 14 ou superior), bem como oferecer versão web responsiva | Média | RF01 a RF10 | M

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
