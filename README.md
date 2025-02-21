# Autenticações
Repositório de teste criado a fim de estudos sobre o GitHub através da Formação GitHub Certification da Dio.me

## Teste feitos:
- Autenticação via nome de usuário e senha.
- Autenticação via Token de acesso pessoal. https://github.com/settings/tokens

## Comandos utilizados no Git:

`git config --global user.name "nome"`
Comando para configurar meu nome de usuário, tal nome de usuário que tem que ser idêntico ao do GitHub para funcionamento.
Exemplo: `git config --global user.name "Redyiel"`

`git config --global user.name "e-mail"`
Comando para configurar meu e-mail, tal e-mail que tem que ser idêntico ao do GitHub para funcionamento.

`git config --list`
Comando para retornar a lista de configurações.

`git clone <url>`
Comando para clonar o repositório que criei no GitHub para esse estudo de autenticações.
Exemplo: `git clone https://github.com/Redyiel/autenticacoes`

`git add .`
Comando para adicionar as alterações feitas no repositório em minha máquina depois que ele foi clonado.

`git commit -m "mensagem"`
Comando para especificar uma mensagem sobre a alteração feita no repositório, com o objetivo de salvar o histórico da linha do tempo do repositório.
Exemplo: `git commit -m "README.md atualizado com mais informações"`

*Ao meu entender `commit` é um registro informativo feito por você da sua alteração na linha do tempo do seu repositório.*
*Gosto de o interpretar como um comentário feito para dizer sobre o que aconteceu naquele momento no repositório.*

`git status`
Comando para checar o status atual do repositório.

`cd <diretório>`
Comando para navegar entre os diretórios

*Admito que comecei tendo problemas, pois não estava na pasta do diretório em si, e sim em na pasta onde estava a pasta dele.*

`ls`
Comando para visualizar o que se encontra naquele diretório.

`git push origin main`
Comando que utilizei para enviar as atualizações que fiz em minha máquina localmente o repositório que estava em nuvem, ou seja passando do Git para o GitHub.

*Entendo que ao utilizar o comando `origin` em `git push` significa que estou atualizando a origem dele, ou seja da onde eu o clonei, da nuvem do GitHub.*

*Ao meu entender, esse comando serve para atualizar a branch `main` para o GitHub.*
*E o que é branch? Novamente usando o comando "ao meu entender" ele é o código que pode ser ramificado, ou seja um código que pode ser modificado e ter novas versões, todavia o código original estará seguro se caso precisar do backup dele.*

*Então compreendo que branch `main` é o código principal, que estou ramificando mas sem perder a versão original do mesmo.*