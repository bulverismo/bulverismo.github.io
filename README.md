# bulverismo.github.io
créditos da pelo efeito matrix em bulverismo.github.io : https://github.com/emilyxxie/green_rain

Dicas para iniciante que nem eu
que querem fazer um simples commit via linha de comando apartir do linux

digitar os comandos e apertar enter na sequencia


para entrar no modo root digite
su 
e na sequencia digite a senha do user root


Para instalar o git no debian/ubuntu/mint

apt install git

crie uma conta

rode estes comandos com as informações da conta

git config --global user.name “seu Nome” 

git config --global user.email “seu-email@seu-dominio.com”

logue no seu github e va na lateral onde mostra o seu perfil e va em setings e após va em SSH and GPG keys

click em New SSH keys

volte ao linux para gerar a chave que você vai por neste local

execute o comando para gerar a chave
ssh-keygen -t rsa -b 4096 -C "seu email"

siga os passos , pode ir apertando enter direto para criar o arquivo diretamente na pasta padrao com o nome padrão e deixar sem senha

o arquivo gerado é ~/.ssh/id_rsa.pub

execute 
cat ~/.ssh/id_rsa.pub 

copie os dados desse arquivo e cole na pagina que esta aberta do github e confirme
vc compartilhou com eles a sua chave publica e agora pode fazer os comits

va na pagina inicial do git

clique em start a project
de um nome ao repositorio e uma descrição e confirme em create a repository

va ao linux e crie uma pasta com o mesmo nome do repository

mkdir nome-do-repositorio

para entrar no diretorioi faça -> cd nome-do-repositorio

execute estes passos:

este comando somente cria um arquivo para o teste
echo "# repoTeste" >> README.md

este comando inicializa o diretorio
git init

este comando adiciona o arquivo que tu criou para poder entrar no proximo commit
git add README.md

este comando faz o commit dando um nome a ele
git commit -m "first commit"

este comando aponta o repositorio remoto
git remote add origin https://github.com/bulverismo/bulverismo.github.io.git

este comando faz o upload em si para dentro da plataforma
git push -u origin master

Se tudo deu certo você fez o seu primeiro commit

Algumas dicas quentes foram encontradas em https://terminalroot.com.br/git/

bulverizando a galáxia
