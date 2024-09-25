# Guia-de-Git-Github
Esse repositório tem como finalidade facilitar o uso do git/github e explicar conceitos para o uso dessas ferramentas...Aproveitem!!👍
## Tópicos Abordados
- [O que é Git?](#ancora1)
- [O que é Github?](#ancora2)
- [Como instalar o Git?](#ancora3)
- [Primeiras configurações no Git Bash](#ancora4)
- [Principais comandos do Git](#ancora5)
- [Como Usar o Github](#ancora6)
- [Padrões de Commit](#ancora7)
- [Curiosidades e Dicas sobre Git/GitHub](#ancora8)
- [Conclusão](#ancora9)
- [Extras](#ancora10)
- [Referências Bibliográficas](#ancora11)
<a name="ancora1"></a>
## O que é Git?
[Git](https://git-scm.com/downloads), é um sistema usado para rastrear mudanças no código-fonte durante o desenvolvimento de software. Ele permite que vários desenvolvedores trabalhem em um projeto simultaneamente, mantendo o histórico de todas as alterações.

*obs.* Caso ainda não o tenha instalado, basta a acessar o link e fazer o download para o seu sistema operacional.
### Principais características:
- Controle de versão: Ele mantém o histórico de alterações no código.
- Cada cópia de um repositório é completa, ou seja, o histórico é copiado para cada máquina que o clona.
- Branches: Permite que se trabalhe em diferentes funcionalidades ou correções de forma isolada, sem interferir no código principal.
<a name="ancora2"></a>
## O que é Github?
[GitHub](https://github.com/) é uma plataforma de hospedagem de repositórios Git na nuvem, que facilita a colaboração, o compartilhamento de código e oferece recursos para gerenciamento de projetos, revisão de código e documentação.
#### Principais características:
- Repositórios públicos e privados.
- Integração contínua do código. 
- Pull requests: Solicitações para incorporar mudanças em um projeto.
- Issues: Para gerenciamento de tarefas e bugs.
<a name="ancora3"></a>
## Como instalar o Git?
### Para Windows:
Baixe a versão mais recente do Git nesse [link](https://git-scm.com/downloads).
Siga as instruções de instalação, deixando as opções padrão. 
Isso também instalará o Git Bash, um terminal que emula o Linux no Windows.
### Para Linux:
No terminal, execute:
~~~ bash
sudo apt-get update
sudo apt-get install git
~~~
### Para macOS:
No terminal, execute:
~~~ bash
brew install git
~~~ 
<a name="ancora4"></a>
## Primeiras configurações no Git Bash
Depois de instalar o Git, é necessário configurar suas informações de usuário. Abra o Git Bash e siga as etapas:

1. Configure seu nome:
~~~bash
git config --global user.name "Seu Nome"
~~~

2. Configure seu email:

~~~bash
git config --global user.email "seuemail@example.com"
~~~

3. Verifique suas configurações:

~~~bash
git config --list
~~~

4. Configure o editor padrão (opcional): Caso queira usar um editor diferente (como o Vim ou o VSCode):

~~~bash
git config --global core.editor "code --wait"  # Exemplo usando VSCode
~~~

Agora, o Git está configurado e pronto para uso.

<a name="ancora5"></a>
## Principais comandos do Git
Aqui estão os comandos básicos e mais utilizados no Git:

Crie um repositório Git na pasta atual:
~~~bash
git init
~~~

Copie um repositório de um servidor para seu computador:
~~~bash
git clone https://github.com/usuario/repo.git
~~~

Veja quais arquivos foram modificados, quais estão prontos para serem commitados, etc.:
~~~bash
git status
~~~

Adicione um ou mais arquivos ao stage para serem commitados:

~~~bash
git add arquivo.txt
~~~

Adicione todos os arquivos alterados:

~~~bash
git add .
~~~

Grava as alterações no histórico do repositório:
~~~bash
git commit -m "Mensagem do commit"
~~~

Veja os commits feitos até agora:
~~~bash
git log
~~~

Crie um novo branch para trabalhar em uma funcionalidade específica:
~~~bash
git branch nome-do-branch
~~~

Mude para um branch existente:
~~~bash
git checkout nome-do-branch
~~~

Una as alterações de um branch ao branch principal (geralmente o master ou main):
~~~bash
git merge nome-do-branch
~~~

Envie seus commits para um repositório remoto:
~~~bash
git push origin nome-do-branch
~~~

Baixe e aplique mudanças do repositório remoto para o local:
~~~bash
git pull origin nome-do-branch
~~~
<a name="ancora6"></a>
## Como usar o GitHub
Agora que você sabe como usar o Git localmente, vamos entender como usar o GitHub:

### Criar um repositório no GitHub:
Acesse GitHub.com.
Faça login (ou crie uma conta).
Clique em New repository.
Dê um nome ao seu repositório e escolha se será público ou privado.
Após criar, você verá as instruções para clonar o repositório.
### Conectar seu repositório local ao GitHub:
Assumindo que você já tem um repositório local, conecte-o ao GitHub:
~~~bash
git remote add origin https://github.com/usuario/repo.git
~~~
### Subir um repositório local para o GitHub:
Envie suas alterações para o repositório remoto:
~~~bash
git push -u origin master  # Ou main, dependendo da configuração
~~~
### Colaborando no GitHub:
Para colaborar em um projeto, você pode criar issues (para discutir problemas ou melhorias) ou criar pull requests (para propor mudanças no código).
<a name="ancora7"></a>

### Importância do README.md
O README.md é um arquivo essencial em qualquer repositório do GitHub. Ele fornece informações sobre o projeto, como o que ele faz, como usá-lo e como contribuir. É a primeira coisa que as pessoas veem ao acessar o repositório, então é importante que seja claro e informativo.
### Importância de um bom perfil no GitHub
O GitHub é uma plataforma de colaboração e compartilhamento de código, e um perfil bem organizado e completo pode ser um diferencial para recrutadores e empresas. Aqui estão algumas dicas para melhorar seu perfil no GitHub:
### Github Desktop
O GitHub Desktop é uma interface gráfica para o Git que facilita o uso do Git e do GitHub. Ele permite clonar repositórios, fazer commits, criar branches e muito mais, tudo de forma visual e intuitiva. É uma ótima opção para quem prefere uma interface gráfica em vez do terminal.

Glossário 📖
fork - Cópia de um repositório para a sua própria conta no GitHub. Isso cria um novo repositório em sua conta que é independente do original, permitindo que você faça alterações sem afetar o repositório original.

issues - Ferramenta usada para gerenciar tarefas, pedidos de novos recursos e correções de bugs em projetos de código aberto. As issues devem ser descritas e listadas, permitindo aos colaboradores discutirem e rastrearem o progresso das mesmas.

pull request - Mecanismo usado para submeter alterações propostas ao repositório original. Um pull request é uma solicitação para que os mantenedores do projeto revisem e potencialmente incorporem as alterações. O pull request passará por um processo de avaliação e pode ser aceito ou rejeitado.

gist - Ferramenta que permite o compartilhamento de trechos de código sem a necessidade de criar um repositório completo. Gists podem ser compartilhados publicamente ou de forma privada.

<a name="ancora7"></a>
## Padrões de Commit
Para um melhor desempenho coletivo se utilizam padrões de commit, afinal você há de entender o que o seu amiguinho fez no código. Isso não é necessário para iniciantes, porém são boas práticas e muito recomendado para o trabalho em equipe. As regras no geral são as seguintes: a mensagem do commit deve conter um emoji (opcional), o tipo do commit (obrigatório), um escopo (opcional) e uma breve mensagem descrevendo as alterações feitas (obrigatório).
~~~
git commit -m " emoji? tipo(escopo?): assunto"   # Modelo
git commit -m ":sparkles: feat(main.c): win module"  # Exemplo
~~~~
### Emoji 
O emoji serve apenas para facilitar a vida do dev, onde só de bater o olho o mesmo já teria uma ideia do que se trata o commit.

Tipo de commit	| Emojis
----------------|--------
Commit inicial	|🎉 `:tada:`
Tag de versão	|🔖 `:bookmark:`
Novo recurso	|✨ `:sparkles:`
Lista de ideias (tasks)|	🔜 `:soon:`
Bugfix	|🐛 `:bug:`
Documentação	|📚 `:books:`
Testes	|🧪 `:test_tube:`
Adicionando um teste|	✅ `:white_check_mark:`
Teste de aprovação	|✔️ `:heavy_check_mark:`
Acessibilidade	|♿ `:wheelchair:`
Texto	|📝 `:pencil:`
Package.json em JS	|📦 `:package:`
Em progresso	|🚧 `:construction:`
Arquivos de configuração	|🔧 `:wrench:`
Removendo uma dependência	|➖ `:heavy_minus_sign:`
Adicionando uma dependência	|➕ `:heavy_plus_sign:`
Revertendo mudanças|	💥 `:boom:`
Alterações de revisão de código	|👌 `:ok_hand:`
Refatoração	|♻️ `:recycle:`
Mover/Renomear	|🚚 `:truck:`

Para mais referências de emojis olhe esse [repositório](https://github.com/iuricode/padroes-de-commits).
### Tipo
O tipo é responsável por nos dizer qual o tipo de alteração ou iteração está sendo feita, das regras da convenção, temos os seguintes tipos:

> - `test`: indica qualquer tipo de criação ou alteração de códigos de teste. 
*Ex.* Criação de testes unitários.
> - `feat`: indica o desenvolvimento de uma nova feature ao projeto. 
*Ex.* Acréscimo de um serviço, funcionalidade, endpoint, etc.
> - `refactor`: usado quando houver uma refatoração de código que não tenha qualquer tipo de impacto na lógica/regras de negócio do sistema. 
*Ex.* Mudanças de código após um code review.
> - `style`: empregado quando há mudanças de formatação e estilo do código que não alteram o sistema de nenhuma forma.
>*Ex.* Mudar o style-guide, mudar de convenção lint, arrumar indentações, remover espaços em brancos, remover comentários, etc.
> - `fix`: utilizado quando há correção de erros que estão gerando bugs no sistema.
>*Ex.* Aplicar tratativa para uma função que não está tendo o comportamento esperado e retornando erro.
> - `chore`: indica mudanças no projeto que não afetem o sistema ou arquivos de testes. São mudanças de desenvolvimento.
>*Ex.* Mudar regras do eslint, adicionar prettier, adicionar mais extensões de arquivos ao .gitignore
> - `docs`: usado quando há mudanças na documentação do projeto.
>*Ex.* adicionar informações na documentação da API, mudar o README, etc.
> - `build`: utilizada para indicar mudanças que afetam o processo de build do projeto ou dependências externas.
>*Ex.* Gulp, adicionar/remover dependências do npm, etc.
> - `perf`: indica uma alteração que melhorou a performance do sistema.
>*Ex.* alterar ForEach por while, melhorar a query ao banco, etc.
> - `ci`: utilizada para mudanças nos arquivos de configuração de CI.
>*Ex.* Circle, Travis, BrowserStack, etc.
> - `revert`: indica a reverção de um commit anterior.


Dessa maneira, conseguimos de forma simples e direta ver qual tipo de mudança está ocorrendo, melhorando bastante a visibilidade e alinhamento com a equipe.

*obs.* Só um tipo por commit. Caso esteja indeciso sobre qual tipo usar, provavelmente trata-se de uma grande mudança e é possível separar esse commit em dois ou mais commits. A diferença entre `build` e `chore` pode ser um tanto quanto sutil e pode gerar confusão, por isso devemos ficar atentos quanto ao tipo correto. No caso do Node.js por exemplo, podemos pensar que quando há uma adição/alteração de certa dependência de desenvolvimento presente em devDependencies, utilizamos o `chore`. Já para alterações/adições de dependências comuns aos projeto, e que haja impacto direto e real sobre o sistema, utilizamos o `build`.

### Escopo
Esse campo serve para detalhar um pouco mais a área do código que foi mudada. 
*Ex.* (UserModule), (Auth), (Database), etc.

### Assunto
Resumo em até 4 palavras do que foi feito no commit.
*Ex.* módulo de pagamento, implementação do hash de senhas, etc.

### Recomendações 
- Adicione um tipo consistente com o título do conteúdo.
- Recomenda-se que na primeira linha deve ter no máximo 4 palavras.
- Para descrever com detalhes, usar a descrição do commit.
- Usar um emoji no início da mensagem de commit representando sobre o commit.
- Os links precisam ser adicionados em sua forma mais autêntica, ou seja: sem encurtadores de link e links afiliados.

Por fim, podemos dizer que o Conventional Commit pode adquirir propriedades daquele projeto, equipe ou empresa, desde que não fuja do conjunto de regras definidos pela convenção, esteja bem alinhados entre os interessados/participantes do projeto e seja bem documentado.


<a name="ancora8"></a>
## Curiosidades e Dicas sobre Git/GitHub
- História do Git: O Git foi criado em 2005 por Linus Torvalds, o criador do Linux, como uma solução para gerenciar o código do kernel do Linux.

- Github Actions: É uma ferramenta de integração contínua que permite automatizar testes e implantar código.
- Branches nomeados: É comum usar nomes descritivos para branches, como feature/novo-recurso ou bugfix/corrigir-bug.
- Forks: No GitHub, você pode "forkar" (copiar) repositórios públicos, permitindo fazer suas próprias modificações sem afetar o projeto original.
- Commits claros: Sempre escreva mensagens de commit claras e concisas. Isso ajuda a entender o que foi mudado no futuro.
<a name="ancora9"></a>
## Conclusão
O Git e o GitHub são ferramentas essenciais para qualquer desenvolvedor de software. Eles permitem que você rastreie e compartilhe código, colabore com outros desenvolvedores e gerencie projetos de forma eficiente. Com este guia, você deve ter uma compreensão básica de como usar o Git e o GitHub, e estar pronto para começar a colaborar em projetos de código aberto ou privados. Lembre-se de praticar e explorar mais recursos para se tornar um mestre no Git e no GitHub. Boa sorte e bons commits!🚀
<a name="ancora10"></a>
## Extras
Como personalizar seu perfil:
https://www.youtube.com/watch?v=TsaLQAetPLU&t=2s
https://www.youtube.com/watch?v=cRoBt6AZgjc&ab_channel=Sujeitoprogramador
Como montar readme
https://www.youtube.com/watch?v=7fEjG4VSXJc
https://www.youtube.com/watch?v=k4Rsy8GbKE0
[pra quem gosta do bash](https://www.youtube.com/shorts/XzFuVIbXF1M)
<a name="ancora11"></a>

## Referências Bibliográficas
padrões de commits: 
https://medium.com/linkapi-solutions/conventional-commits-pattern-3778d1a1e657
https://dev.to/renatoadorno/padroes-de-commits-commit-patterns-41co 
Git e Github:
https://www.youtube.com/watch?v=UBAX-13g8OM&list=PLhkO7OMKgT_rqwGYldqcFxyN4yjFgmDh8 - explica os dois
https://www.youtube.com/watch?v=s54N3QuLdKc&t=369s&ab_channel=EvertonDev - criar repo
https://www.youtube.com/shorts/2s-7aleij-Q - criar repo
