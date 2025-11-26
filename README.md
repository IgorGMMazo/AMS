# AMS

INFORMAÇÕES IMPORTANTES:
- Nunca subam as alterações direto na branch MAIN, subam apenas para a branch HOM, nossa branch hom é nosso teste de validção, após validado iremos colocar na branch MAIN.
- Não editem nada no próprio git, isso gera conflito se alguém depois esquecer de dar o pull e tentar dar o push, se quiserem mudar algo ou editar, editem no VSCode e deem push.

COMANDOS QUE PROVAVELMENTE VOCÊS USARÃO:

- ### git init =
	
	-Cria uma pasta git para a pasta
	
- ### git add . =
	
	-adiciona todos os arquivos para a área de preparação ( adicionar um único arquivo seria git 
	add NOME )
	
- ### git commit -m "MENSAGEM" =
	
	-Salva um comentário junto com a mudança
	
- ### git remote add origin URL =
	
	-Faz a conexão
	
- ### git branch -M main =
	
	-Renomeia o ramo principal para main
	
- ### git push -u origin main = 
	
	-Leva as informações para o main e define ele como padrão para as outras vezes( deixando claro que nas próximas vezes será apenas necessário git push (caso queria para para a main))
	
- ### git status =
	
	-Mostra o status da sua pasta: quais arquivos foram modificados, quais estão na área de preparação e quais não estão sendo rastreados.
	
- ### git pull =
	
	-Puxa as atualizações mais recentes do repositório no GitHub para o seu computador local.
	
- ### git clone URL =
	
	-Usado para baixar um repositório que já existe no GitHub
	
- ### git branch =
	
	-Lista todos os branches locais.
	
- ### git branch nome-do-novo-branch=
	
	-Cria um novo branch.
	
- ### git checkout nome-do-branch =
	
	-Troca você para o branch especificado.
	
- ### git merge nome-do-branch-para-juntar =
	
	-"Mescla" (junta) as alterações de outro branch no branch em que você está atualmente.
	
- ### git fetch =
	
	-Ele **"baixa" (busca) todas as atualizações** do repositório remoto (como o GitHub), mas **não as aplica** (não faz o "merge") automaticamente no seu branch de trabalho local. Ele simplesmente atualiza as suas "cópias" locais dos branches remotos (ex: `origin/main`).
