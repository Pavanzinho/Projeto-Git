# Caminho para adicionar arquivos/alterar no github.

# //git init : criar repositório vazio para a pasta.
# //add : enviar arquivo para área de staging(comandos ' na fila' para serem executados).
       Estes arquivos estão salvos na memória do computador, mais para frente, iremos usar push para ' empurrar' 
        esse commit que vamos criar(que estao no repositorio local), assim, eles irão para o repositorio do github.
# commit : como se fosse uma versão do codigo.
# branch: git branch -M'"nome que deseja que o branch principal tenha(main está sendo bem utilizado pelas empresas)"
# https://github.com/p4van772000/git-e-github.git : PADRÃO 
# git remote add origin https://github.com/p4van772000/git-e-github.git:
    "remote": conexao entre repositorio local com repositorio do github4
    "add" para adicionar
    "origin": nome que estou dando para essa conexao.
# git push -u origin main

# Criando novo branch
 git checkout -b "nome da nova branch"
 Lembrando que, se caso já exista alguma outra branch além da principal(neste caso a main), é só fazer o comando : git checkout "nome da outra branch"
 -Após criar, deletar, alterar os arquivos, seguir o caminho que ja está demonstrado anteriormente:
    *mandar alterações para o staging(git add . = esse ponto significa que estou mandando todas as alterações/arquivos alterados que estão no diretório, caso queira adicionar um arquivo especifico, basta colocar o nome dele entre aspas duplas)
    *criar o novo commit (versao)= git commit -m " nome da nova versão/commit que está sendo salvo no repositório da minha maquina""
    *empurrar essa nova versão para dentro da branch que está automaticamente conectada com o repositório do github
        = git push origem "nome da nova branch"


 # Juntando duas branchs
- git checkout main (Retornando para a brach principal)
-git merge +nome da branch que quer misturar com a main
-git push origem main: jogando as informaçoes da nova branch que foi criado para a main.
- Agora, podemos ver a commit que foi criada dentro da nova branch, na branch main .

# Clone github
 -Pegar o link do repositório que deseja clonar e :
    git clone +link

# como atualizar o repositório que não está na sua maquina. Assim, caso eu faça um clone de um arquivo alheio que não está na minha máquina e o dono atualizar, basta : :
- Entrar na pasta do repositório, onde está o projeto que quer atualizar:
    cd +nome da pasta
-git pull

# FORK : 
    É uma forma de colocar repositórios alheios no meu repositório no github
    -Basta entrar no repositório da pessoa e clickar no botao " fork" na parte superior direita.

# Pull request:
    após faze o fork do repositório alheio, posso enviar um pull request para solicitar uma possível alteracao no codigo dessa pessoa, caso ela concorde e aceite, o codigo dela será atualizado automáticamente.
    - Basta entrar no código presente no repositório, alterar e depois mandar um commit(por meio do próprio git hub).
