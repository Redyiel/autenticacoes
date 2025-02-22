# 📚 Estudos sobre autenticações  
Repositório de teste criado a fim de estudos sobre o GitHub através da Formação GitHub Certification da Dio.me  

## 📝 Testes  feitos:  
- Criação desse repositório *(Meu primeiro repositório)*
- Autenticação via nome de usuário e senha.  
- Autenticação via Token de acesso pessoal. https://github.com/settings/tokens  
- Autenticação via SSH. https://github.com/settings/keys  

## 📟 Comandos utilizados no Git:  

### 🛠️ Configurando o Git  

`git config --global user.name "nome"`  
Comando para configurar meu nome de usuário, tal nome de usuário que tem que ser idêntico ao do GitHub para funcionamento.  
Exemplo: `git config --global user.name "Redyiel"`  

`git config --global user.name "e-mail"`  
Comando para configurar meu e-mail, tal e-mail que tem que ser idêntico ao do GitHub para funcionamento.  

`git config --list`  
Comando para retornar a lista de configurações.  

### 🔄 Adicionando ou atualizando o repositório  

`git clone <url>`  
Comando para clonar um repositório do GitHub 
Exemplo: `git clone https://github.com/Redyiel/autenticacoes`  

`git add .`  
Comando para adicionar as alterações feitas no repositório na máquina local depois que ele foi clonado.  

`git commit -m "mensagem"`  
Comando para especificar uma mensagem sobre a alteração feita no repositório, com o objetivo de salvar o histórico da linha do tempo do repositório.  
Exemplo: `git commit -m "README.md atualizado com mais informações"`  

*Ao meu entender `commit` é um registro informativo feito por você da sua alteração na linha do tempo do repositório.*  
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

### 🔐 Configurando autenticação SSH  

**🤔 O que é e para que serve o SSH no contexto do GitHub?**  
Com as chaves SSH, é possível se conectar ao GitHub sem fornecer o nome de usuário e o personal access token em cada visita. Você também pode usar uma chave SSH para assinar commits.  
Fonte: https://docs.github.com/pt/authentication/connecting-to-github-with-ssh  

`ssh-keygen`  
Comando para gerar uma chave SSH.  
Após gerar a pasta, irá solicitar uma senha (passphrase) não obrigatória.  

**📁 Onde estará a chave SSH?**  
No diretório citado pelo resultado do comando.  

**🔑 Sobre as chaves:**  
A chave que vamos utilizar é a pública, ou seja a .pub  
A chave privada não se compartilha com ninguém por segurança.  

`cat <nome-da-chave>`  
*Ao meu entendimento é o comando para descriptografar a chave, para copiar e colar no GitHub https://github.com/settings/keys, para liberar o acesso sem ter as credenciais do usuário.*  

*O link para trabalhar em um repositório com acesso concedido através do SSH é o "link SSH"*  
![Link SSH](https://github.com/Redyiel/autenticacoes/blob/main/Link%20SSH.png)  

`git remote set-url origin git@github.com:<link-ssh>`  
Exemplo: `git remote set-url origin git@github.com:Redyiel/autenticacoes.git`  
*Comando que ao meu entender é para trocar o módulo HTTPS do Git para um módulo de link SSH tornando possível trabalhar com o repositório remotamente através do SSH*  

Ao fazer o comando de `git push` em um repositório acessado através de SSH poderá ocorrer uma pergunta do terminal questionando se é uma conexão segura.  

## 🗑️ Gerenciador de Credenciais do Windows  

Foi utilizado o Gerenciador de Credenciais do Windows para remover o armazenamento do login salvo do GitHub para efetuar os testes de autenticações.  