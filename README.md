# avaliacao-jp
Avaliação

Comandos do git:
- git init --> Tem a função de inicializar um repositorio em um diretório já existente.

- git pull --> Tem a função de pegar todas as informações de um repositorio local e jogar para a sua branch atual.

- git status --> Ele vai mostrar o estado atual do seu repositorio ou seja vai mostrar todos os arquivos, arquivos alterados e arquivos que estejam prontos para serem comitados.

- git fetch --> Tem como função de baixar tudo de um repositorio remoto e sem fazer a mesclagem.

- git add <filename ou .> --> Sua função consiste em adicionar arquivos ao índice e prepara todos os arquivos para o proximo commit

- git branch -D <branchname> --> Ele vai remover a branch selecionada 

- git rm --cached <file> --> Tem a função oposta do git add, ao invés de adicionar arquivos ao indice ele vai remove-los

- git push --> Tem como função enviar os commits realizados no repositorio local para o repositorio remoto

- git branch --> Tem a função de mostrar todas as branches que existem. Existem algumas variações de git branch como git branch -r que vai listar as branches remotas e git branch -a que vai listar tanto as remotas como as locais

- git merge <branch> --> Team a função de fazer o merge da sua branch atual para a branch selecionada

- git checkout <branchname> --> Irá te levar para a branch descrita e para voltar para sua branch antiga use git checkout <previous-branchname>

- git commit -m "<description>" --> Tem como função comitar as mudanças realizadas no indice com uma mensagem descritiva

- git checkout -b <branchname> --> Tem a função de criar uma branch nova e direciona-lo diretamente para ela
Chave SSH:

- Primeiramente precisamos saber se nosso dispositivo possui uma chave SSH que servira para acessar remotamente aos nossos servidores, para isso usamos este comando --> "ls -al~/.ssh"

- Verificando e estando ciente da chave existindo podemos iniciar um agente para ela com o seguinte comando --> "eval "$(ssh-agent -s)""

- Caso nao exista um chave SSH precisamos realizar o seguinte comando para cria-lá --> "ssh-keygen -t ed25519 -C"seu email""

- Após criar a chave e criar o agente devemos adicionar a chave ssh ao agente com o seguinte comando --> "ssh-add ~/.ssh/id_25519"

- Para copiar-mos alguma chave ssh devemos realizar o seguinte comando -->"clip <~/.ssh/id_ed25519.pub"

- E para sabermos se a chave ssh esta conectada com o github usamos o seguinte comando --> "ssh -T git@github.com" e em seguida "yes" 