### Comandos básicos de terminal

| Windows | Linux |
| ----------- | ----------- |
| dir | ls |
| cd | cd |
| cls | clear or ctrl + L |
| mkdir | mkdir |
| echo | echo |
| del(arquivo) / rmdir(diretório) | rm or rf(força e recursivo)|

##### SHA (Secure Hash Algorithm)
- Conjunto de funções hash criptografados projetado pela NASA
- A encriptação gera um conjunto de 40 caracteres
- Forma curta de representar um arquivo

##### Objetos internos do git
- Blobs
- Trees
- Commits

### Comandos do Git
###### Iniciar repositório no git
```
$ git init 
```
###### Clonar repositório 
```
$ git clone linkDoGitHub (ex: chave ssh)
```
###### Verificar status dos arquivos no git
```
$ git status
```
###### Fazer commit
```
$ git add nomeDoArquivo.txt ou $ git add .
$ git commit -m "Sua mensagem aqui"
$ git push origin main
```
###### Puxar arquivos do repositório remoto para o local
```
$ git pull
```

###### Criando e mudando para nova branch
```
$ git checkout -b "nomeDaNovaBranch"
```
###### Trocando de branch
```
$ git checkout nomeDaBranch
```
###### Editar mensagem do último commit
```
$ git commit --amend
```
