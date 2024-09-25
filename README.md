# O presente repósitorio será o local onde terei a adição dos resumos feitos durante o estágio

## Separando por tópicos abordaremos, em primeiro momento os seguintes assuntos:

- **Metodologias Agéis**
- **Git e GitHub**
- **Conventional Commits**
- **Markdown**
- **Segurança** 

---

# **Metodologias Agéis (MA)**

### Resumo

O manifesto ágil pode ser representado por seus 4 valores e 12 princípios, consistem em:

#### Valores

1. Individuos e interações ** mais ** que processos e ferramentas;
2. Software em funcionamento ** mais ** que documentação;
3. Colaboração com o cliente ** mais ** que negociações de contrato;
4. Responder a mudanças ** mais ** que seguir um plano.

Os Valores sugerem dar mais enfâse na parte de colaboração tanto no time quanto para com o cliente ao invés de se ater aos processos e ferramentas de contução ou as negociações dos contratos, ter documentação se faz necessário, mas nessa questão, algo mais simples documentado com alguma coisa já funcionando é mais importante, seja capaz de responder a mudanças, pois elas estarão sempre acontecendo.

#### Princípios

1. Satisfaça o consumidor;
2. Aceite mudanças;
3. Entregas frequentes;
4. Trabalhe em conjunto;
5. Confie e Apoie;
6. Conversas Face a Face;
7. Softwares Funcionando;
8. Desenvolvimento Sustentável;
9. Atenção continua;
10. Mantenha a simplicidade;
11. Times Auto-organizados;
12. Refletir e ajustar.

Os princípios trazem os conceitos dos valores de forma mais  individualizada e explicita, onde eles levantam a importância da colaboração e do trabalho em equipe para contrução de um ambiente ágil de desenvolvimento.

> " Agilidade é a capacidade de mover e mudar de direção com rapidez e facilidade." 
> 
 Alistair Cockburn

Alistair Cockburn apresentou um modelo chamado de _*Heart of Agile*_

Para seu funcionamento precisa **colaborar** com a equipe para conseguir um bom aprendizado, ter **entregas** frequentes para construir um bom processo, **refletir** e analisar tudo que aprendeu e **melhorar** sobre isso para um bom trabalho. Estes 4 pontos são o coração desse modelo.

Seguindo os pontos apresentados chegamos na estrutura de como um modelo ágil funciona. Ser ágil é composto por, ** mindset **, ** 4 valores **, ** 12 princípios ** e que são manifestadas atráves de diversas ** práticas ** diferentes.

Com essa base em mente, o proximo assunto a ser falado é o framework Scrum, que apresenta uma forma de trabalhar a MA.

### Scrum

Ele é baseado na teoria empírica(Quanto mais eu faço mais eu aprendo), trazendo um modelo de organização e alguns papéis.

| Valores         | Pilares      | Papéis                 |
|---------        |--------------|----------              |
| Coragem         | Transparência|Scrum Master (SM)       |
| Foco            | Inspeção     |Product Owner (PO)      |
| Comprometimento | Adaptação    |Time de desenvolvimento |
| Respeito        |        
| Abertura        | 
----   


O Scrum é:
 - Leve;
 - Simples de aprender;
 - Difícil de aplicar.

Conhecendo seus valores, os pilares trazem os seguintes pontos, precisa ser **transparente** para que todo o processo seja visivel, a **inspeção** vai analisar o desenvolvimento e com base nela, a parte de **adaptação** buscará identificar erros e as formas de solução.

Com relação aos papéis SM, PO e o time de desenvolvedores, cada um possui suas responsabilidades no Scrum, de uma forma geral, o **SM** é reponsável por gerir o time Scrum, ele possui amplo conhecimento Scrum e agirá como um facilitador e instrutor no time, guiando e auxiliando. O **PO** tem a visão de negócio e irá gerir o *backlog* do produto, ele agirá como intermédio entre o cliente e o **Time de desenvolvimento**, esse por sua vez será orientado por objetivos/metas e irá construir aquilo que foi idealizado no backlog do produto.

Sobre seus eventos, a "estrutura do Scrum". Possui um Product Backlog, construido por User stores( desejo do cliente, quebrada em partes menores da ideia geral, elas dever ter título e apresentar pontuação, quanto mais pontos mais relevantes), aqui terá a visão clara e objetiva do produto, para construir o backlog pode fazer uso de:
 - Entrevistas, dinâmicas de grupo e oficinas;
 - Tecnicas de criatividade em grupo;
 - Tecnicas de tomada de decisão em grupo;
 - Questionário, pesquisa, observações e propóstas.

Então para a contrução do backlog temos um conjunto de ações que são: Evolução do Mercado, Feedback, Visão do Produto, Analise de Concorrente e Pesquisa. Ele precisa ser **DEEP**
- **D**etalhado de maneira apropriada
- **E**stimado
- **E**mergente
- **P**rioridade

Com isso todo o processo decorre da analise do backlog, com base nele, inicia a Sprint que funciona de forma ciclica com no maximo 4 semanas, ela inicia com uma *Sprint planning* que define o que pode ser feito, *Daily scrum* que ocorre com o time de desenvolvimento são encontros diários de no máximo 15 minutos regidos por( O que fez? O que vai fazer? Quais impedimentos?), *Sprint review* amostragem do que está feito e análise para aprovação ou não duração máxima de 4 horas( podendo surgir a questão de necessidades de *incrementos do produto*) e *Sprint retrospective* duração máxima de 3 horas e que irá identificar o que manter, melhorar ou retirar.


### Git e GitHub

Neste tópico falaremos brevemente sobre as ferramentas de auxilio no versionamento para seus projetos. O git é um software que ajuda nesse versionamento local, permitindo que você construa aplicações com funcionalidades em diferentes versões, facilitando assim o controle de adições novas. O github funciona com um repósitorio online para seus projetos git, além de mais funcionalidades que existem para o mesmo.

#### Primeiros passos:

1. Baixar o git. [Link Git Download!](https://git-scm.com/downloads "Git")
2. Configure o seu ambiente git.
3. Inicie o seu projeto.

Após feito o download, seguindo passos de que fez isso em uma máquina com windowns, abra o git bash, que vem com a instalação do git, ou o próprio CMD do computador e inicie as configurações para começar no projeto.

Primeiro teste se o git foi instalado passando:

```
git --version

```
Se receber dados da versão está certo, caso receba um erro, tente instalar o git novamente, houve algum problema.

Próximo passo são configurações para padronizar os seus trabalho no git, caso já tenha uma conta no github, será útil agora, pois iremos configurar 3 informações.

- Primeiro user.name
- Segundo user.email
- Terceiro branch

```
git config --global user.name "SEUNOMEUSUARIO"
```
```
git config --global user.email SEUEMAILUSUARIO@.COM
```
```
git config --global init.default branch main
```
Com isso você já conseguirá começar seus projetos usando o git de auxilio.

Irei passar uma lista de comandos que será útil.

```
git init // Faz com que o git reconheça aquele repósitorio

git status // Irá apresentar alguma mudança, caso haja

git add <ARQUIVO> // Prepara o arquivo para o commit

git add . // Prepara todos os arquivos

git rm --cached <ARQUIVO> // Tirá o arquivo que você deu add

git commit // Faz o commit

git commit -m "Mensagem de descrição"

git commit -a // Faz commit dos arquivos ignorando se não fez o add

git diff // Mostra onde foi alterado

git log // Mostra detalhes do histórico de commits

git log --oneline // Resume o histórico

git rm <ARQUIVO> // Apaga o arquivo

git restore <ARQUIVO> // Restaura o arquivo

git mv <ARQUIVO> <NOVONOME> // muda o nome do arquivo sem que o git deixe de identifica-lo

git branch <nomedabranch> // Cria uma nova branch

git switch <nomebranch> // Muda para a branch citada

git push --all origin // Irá mandar todas as branchs locais para o repósitorio do github

git pull // Se atualizou diretamente no github e precisa atualizar o seu local
```