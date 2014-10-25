# SINCRONIZANDO O GIT LOCAL COM O GITHUB VIA PROMPT
===================================================

## FERRAMANTES E SISTEMA OPERACIONAL
- WINDOWS
- SUBLIME TEXT
-------------------------------------

### Vou partir do pré suposto que todos saibam usar a linha de comando.

* DOWNLOAD DO GIT (http://git-scm.com/)
* Atenção: 
###### Fique atento na instalação pois ele irá perguntar se você vai querer que ele rode pelo prompt do windows, marque essa opção.

* Criar conta no Github (https://github.com/)
* Na instalação do GIT vem o GIT BASH. Ele é parecido com o prompt do windows, você precisará criar a chave SSH por ele.

p. Assim você insere a mesma na sua conta do github. Isso autoriza seu computador a enviar arquivor para seu repositório GITHUB online.

* Inicie o GIT BASH e digite ( ssh-keygen -t rsa -C "seu-email@dominio.com" ). ATENÇÃO: Nesse momento ele vai pedir um nome de usuário e senha, eu não quero toda vez que fizer um envio para o github ter que ficar digitando login e senha, por isso nessa hora clique ENTER todas as vezes até ele finalizar a criação da sua KEYGEN.

* A chave SSH fica criada no arquivo ( C:\Users\nome-do-seu-usuario\.ssh\id_rsa.pub )

* Peque o conteúdo desse arquivo e copie.

* No github, vá em configurações - SSH Keys - Add SHH Keys e em título coloque o que quiser e em Key cole seu ssh copiado anteriormente.

* Pronto, você já tem a conexão. Vamos fazer nosso primeiro commit.

* Na home do github você não tem muita coisa para ver, pois ainda não tem nenhum repositório criado.

### Vamos criar nosso repositório:

* Clicamos no botão ( New repository ) e damos um nome para ele.
* Existem 2 tipos de repositórios, públicos (0800) e privados (pagos). Crie um público mesmo.

* Depois de criado ele já aparece na tela do repositório com algumas informações úteis. Copie e cole em um notepad, pois depois do nosso commit essas informações não vão aparecer mais.

## Em nosso computador
---

- Vamos definir uma pasta para nosso projeto. Criaremos um arquivo chamado README.md.
- Podemos abrir esse arquivo no notepad ou no editor de texto que preferir. Adicione no arquivo um texto qualquer.

## Usando o prompt do windows

* Navegue até a pasta que esta nosso projeto pelo prompt (Ex: c:/user/pasta-do-projeto) e vamos fazer nosso commit seguindo os passos abaixo:
#### Atentem em mudar as informações do seu GITHUB!!!

* git init
* git add README.md
* git commit -m "Meu primeiro commit"
* git remote add origin git@github.com:seu-usuario/seu-repositorio.git
* git push -u origin master

#### Feito! Bom galera espero que tenha ajudado a quem precisa e caso tenha outra forma mais  fácil ou melhor por favor deixem comentários.
#### Abs