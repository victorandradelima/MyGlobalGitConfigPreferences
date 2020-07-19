# MyGlobalGitConfigPreferences

PS: para usar o VSCode como editor do arquivo, rode o seguinte comando no terminal:
git config --global core.editor code

Use o comando:
git config --global --edit

Insira os seguintes comandos:

```
[user]
	email = victorandradelima@gmail.com
	name = Victor Lima
[core]
	longpaths = true
	editor = code --wait
[push]
	followTags = true
[alias]
	c = !git add --all && git commit -m
	s = !git status -s
	l = !git log --pretty=format:'%C(blue)%h%C(red)%d %C(white)%s - %C(cyan)%cn, %C(green)%cr'
	amend = !git add --all && git commit --amend --no-edit
	count = !git shortlog -s --grep
```

PS2: Caso trabalhe com várioas repositórios remotos diferentes, voce vai precisar configurar o USER direto no projeto, neste caso devemos usar a tag --local ex:
git config --local --edit