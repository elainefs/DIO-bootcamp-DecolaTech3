Uma mensagem de Git commit bem elaboradora é a melhor maneira de comunicar o contexto sobre as mudanças feitas em um projeto para outros contribuidores.

Um bom commit do Git deve conter um **assunto** e um **corpo**. Ele deve ser estruturado assim:
```
(Assunto) Curto (50 caracteres ou menos) resume as mudanças

(Corpo) Mais detalhes sobre as mudanças. Pode ter várias linhas.
Cada linhas do corpo do commit não devem ter mais do que 72 caracteres.
Sempre adicionar uma linha em branco para
separar o assunto do corpo do commit.
Se 50 caracteres não forem suficientes
para o assunto, não ultrapasse 72 caracteres.

Novos parágrafos vem depois de linhas em branco.

- Pode usar tópicos
```

#### As sete regras para um boa mensagem de commit do Git

[Cbeas](https://cbea.ms/git-commit/#seven-rules)

1. Assunto e corpo do commit devem ser separados por uma linha em branco
2. Limite a linha de assunto a 50 caracteres
3. O assunto deve começar com letra maiúscula
4. Não termine a linha do assunto com um ponto
5. Use o modo imperativo na linha do assunto
6. Limite as linhas do corpo em até 72 caracteres
7. Use o corpo para explicar _o que_ e _por que_ 

###### Nota
Nem todo commit requer um assunto e um corpo. Às vezes, uma única linha é suficiente para explicar as alterações, não necessitando de nenhuma informação adicional.
Nesse casso pode usar o comando `$ git commit -m "Seu commit de uma linha"`

Para commits com assunto e corpo use `$ git commit`

O editor de texto irá abrir para você escrever.
Você pode configurar um editor para usar com o Git na linha de comando se você ainda não tiver um configurado.

###### Dica 01
Se você está tendo dificuldades em resumir o assunto do seu commit, pode ser que você esteja fazendo muitas alterações de uma só vez. A melhor forma de resolver isso é fazendo _commits atômicos._

#### Commits Atômicos
[Fresh](https://www.freshconsulting.com/insights/blog/atomic-commits/)
Os commits atômicos giram em torno de uma tarefa ou correção por vez.

**- Como funciona**
- Commit cada correção ou tarefa como uma alteração separada
- Commit apenas quando um bloco de trabalho estiver concluído

**- Benefícios**
- Fácil de reverter sem afetar outras alterações
- Fácil de fazer outras alterações em tempo real
- Fácil de mesclar recursos com outras ramificações

###### Dica 02
Use o modo imperativo no assunto do commit.
Por exemplo, tente encaixar a mensagem do commit na seguinte frase: "Quando aplicado, o que esse commit faz?"
_Ex.: Quando aplicado, o que esse commit faz? Corrige erro no servidor_

###### Dica 03
Caso você queira aprender um padrão mais elaborado de como fazer commit, existe o [_Conventional Commits_](https://www.conventionalcommits.org/en/v1.0.0/).

Sua estrutura segue o seguinte modelo:
```
<tipo>[escopo opcional]: <descrição>
<corpo opcional>
<rodapé opcional>
```
**Tipos**
O Tipo de um commit tem a finalidade de comunicar a intenção que o utilizador teve ao modificar o código.

Você pode criar seus próprios tipos, mas os principais são: 
- **build:** Alterações que afetam o sistema de compilação ou dependências externas (escopos de exemplo: gulp, broccoli, npm)
- **ci:** Alterações em nossos arquivos e scripts de configuração de CI (escopos de exemplo: Travis, Circle, BrowserStack, SauceLabs)
- **docs:** Somente a documentação muda
- **feat:** Um novo recurso
- **fix:** Uma correção de bug
- **perf:** Uma alteração de código que melhora o desempenho
- **refactor:** Uma alteração de código que não corrige um bug nem adiciona um recurso
- **style:** Alterações que não afetam o significado do código (espaço em branco, formatação, ponto e vírgula ausente etc.)
- **test:** Adicionando testes ausentes ou corrigindo testes existentes

**Escopo**
É um parâmetro opcional, fornece informações contextuais adicionais e está contido entre parênteses.

**Descrições**
É um parâmetro obrigatório, seria o mesmo que o assunto do commit, que foi falando anteriormente.
No entanto, há algumas mudanças na sintaxe, como por exemplo deve ser escrito em letras minúsculas.


Para saber mais, acesse esse artigo em português sobre [Conventional Commits](https://blog.geekhunter.com.br/o-que-e-commit-e-como-usar-commits-semanticos/)