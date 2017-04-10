#Comandos git
git config --global user.name "$nome"
git config --global user.email "$email"
git config --global core.editor $editor
git config --list
mkdir $repositorio
cd $repositorio
git init
git status
git add $arquivo
git status
git diff
	--name-only
git commit -m "$mensagem"
	-am (adiciona todos os arquivos modified)
git log
	--decorate
	--author"$nome"
	--graph
git shortlog
	-sn
git show $hashdaversao
git reset (--option) $hashdaversao
	--soft (staged)
	--mixed (modified)
	--hard (unmodified)(!!!) 
git remote add $remotename $remotolink
git push -u $remotedestino $branchorigem
git clone $repositoriolink $pastalocal