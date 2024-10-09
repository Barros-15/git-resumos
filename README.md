
# Configuração Básicas do GIT 
(git n depende do git hub para fazer o versionamento = registra e gerencia oq pe feito no código fonte)

| código | função |
| -------|--------|
|git config| mostra sobre a ferramenta |
|git config –-global user. “”(name ou email) | define o nome ou o email. |
|git config init.defaultBranch| nome da Branch |

•	Colocar “nome” dps altera o nome da Branch |
•	Colocar entre o config e o init (--global) para fazer a alteração globalmente

| código | função |
| -------|--------|
| git confing  -–global  -–list | todas as config globais (sem o global retorna tudo) |
|git clone| clona repositório (joga do github para maquina) |
| git config credential.helper (store ou cash) |  salva as credenciais / store = permanentemente /cash = temporariamente | 
| git config –global –show-origin credential.helper | mostra onde salva os treco |


# Enviar arquivos pro git hub
- git clone URL
- git add . = salva/puxa arquivos
- git commit -n “nome” = salva as alterações
- git push u- origin (nome do Branch) = upa arquivos

# Criando e Clonado Repositorios
 - (armazenamento digital centralizado) – (branch= ramificação do seu projeto)-(oq começa com . fica oculto) 
 | código | função |
| -------|--------|
| mkdir (nome)| cria um repositório (arquivo) |
| cd (nome da pasta) / | entra na pasta |
| cd .. | sai da pasta|
| git init | transforma em um repositório git / inicia|
| cd .git | entra nas config do git ocultas |
| ls | lista oq tem dentro|
|cat | exibir conteúdo / cat config = conteúdo do repositório |
| git clone URL (nome da pasta) | clona o conteúdo |
| origin | nome padrão do servidor|
| git remote add origin URL | vincular o repositório |

# Salvando Alterações no Repositorios Local

| código | função |
| -------|--------|
|git status |  Já diz
| touch README.md | cria um arquivo de txt |
| git add (nome do arquivo)| manda para área de preparação|
| git log | exibe o commit/info |
| echo (nome da pasta / arquivo) / > .gitignore |  ignora os arquivos que adicionar nela |

# Desfazendo Alterações no Repositório 
| código | função |
| -------|--------|
| rm -rf .git | desfaz o git init |
| git restore (nome do arquivo) |  Restaura o arquivo de alguma alteração | 
|git commit –amend -m”nome” | muda o nome do ultimo commit|
|git reset –(1 abaixo) (e dps o código do commit) | desfazer / retornar para um commit anterior |
•	-- soft = tirar os arquivos do commit mencionados
•	-- mixed = 
•	-- hard = ignora os arquivos do ultimo commit e exclui 

# Enviando e Baixando Alterações
(Ao criar um repositório no GitHub ele passa as configs para add) 
| código | função |
| -------|--------|
| git pull |  puxa as info/alterações e mescla no PC|
