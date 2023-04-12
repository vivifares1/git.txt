# git.txt
Introdução ao Git e GitHub
Introdução ao Git e GitHub básico, indicado para quem está dando os primeiros passos em programação.
O que é Git
Criado em 2005 por Linus Torvalds, O Git é um sistema de controle de versionamento distribuído (Version Control System, VCS). Ajuda a gerenciar alterações em código fonte ao longo do tempo pois a ferramenta mantém um registro de todas as versões do código. Podendo voltar para qualquer versão anterior ou compará-las, ajudando a descobrir e corrigir erros.

Instalando e configurando o Git
1 - Instalando a Partir do Fonte: Baixe o arquivo exe do instalador a partir da página e execute-o. Link https://git-scm.com/download
2 - Após a instalação defina o seu nome de usuário e endereço de email.

Comandos:  git config --global user.name "NOME" 
 git config --global user.email EMAIL@EXEMPLO.COM 

Primeiros comandos no Git (Iniciantes)
git help : Ajuda
git init : Cria um repositório
git add *: Adiciona arquivos
git status : Verifica status dos arquivos
git commit : Comitar arquivos
git commit -m "MENSAGEM" : Comitar arquivos com mensagem
git rm : Remove arquivos
git mv : Move arquivos
git log : Visualizar logs
git remote -v : lista o link dos seus repositórios remotos
git remote add origin LINK DO GITHUB : Vincular repositório local com um repositório remoto
git remote show origin : Mostra informações dos repositórios remotos
git push origin master - "empurrar" o código para Github
git pull origin master - "puxar" o código do Github
git clone URL : Clonar um repositório
ls: Listar
ls -a : Listar arquivos ocultos
cd NOME-DA-PASTA : Navegar na pasta
cd .. : Retroceder um nível
mkdir NOME-ARQUIVO : Criar pasta
ctrl + l : Limpar tela do terminal

Iniciando o Git e criando um commit
1 - Abra o Git Bash no local onde deseja criar o repositório
2 - Crie uma pasta mkdir NOME-DA-PASTA, entre nela cd NOME-DA-PASTA e inicie o repositório git init
3 - Crie um arquivo de texto dentro do repositório e salve-o em .md (nomedoarquivo.md)
4 - Use os comandos para comitar: git add * enter e depois git commit -m "MENSAGEM" enter

O que é GitHub
Plataforma de hospedagem de código-fonte e arquivos com controle de versão (VCS) usando o Git.

Criando conta no GitHub
1 - Acesse o site do GitHub https://github.com/
2 - Clique em Sign up
3 - Coloque seus dados nome de usuário, endereço de email e senha
4 - Siga as instruções e verifique sua conta

Subindo primeiro repositório
1 - Acesse o GitHub e clique em novo repositório
2 - Coloque o nome do repositório e descrição
3 - Copie endereço/url gerado na opção “push an existing repository from the command line”
4 - Abra o Git Bash na pasta onde está o seu projeto
5 - Use o comando git remote add origin LINK DO GITHUB
6 - Use o comando git remote -v
7 - Use o comando git push origin master
8 - Será solicitado o usuário e senha para autenticar no GitHub
9 - Repositório local enviado para repositório remoto/Github

Clonando repositório
1 - No GitHub.com, vá até a página principal do repositório
2 - Clique em Código (Code)
3 - Copie a URL do repositório
4 - Abra Git Bash
5 - Escolha o local onde deseja ter o diretório clonado
6 - Digite git clone e cole a URL copiada
Comando: git clone https://github.com/USUARIO/REPOSITORIO
7 - Pressione ENTER para criar seu clone local

Resolvendo Conflitos
Resolvendo conflitos de mesclagem causado por alterações de linha
1 - Abra o arquivo com o conflito
2 - A linha ======= divide suas alterações das alterações na outra ramificação.
3 - Faça as modificações necessárias e exclua os marcadores de conflito <<<<<<<, =======, >>>>>>>
4 - Use o comando git add *
5 - Use o comando git commit -m "Mensagem"
6 - Use o comando git push origin master
