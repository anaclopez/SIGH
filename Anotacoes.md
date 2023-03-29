# Antotações

### Git

#### Comandos basicos:

###### Inicializar repositorio:
```git init```

###### Adicionar itens ao versionamento:
```git add [arquivos ou "." para todos os arquivos]```

###### Verifica status do vercionamento:
```git status ```

###### Criar commit:
```git commit [Arquivo especifico ou -a para todos os arquivos] -m "messagem sobre as alterações feitas"```

###### Criar uma nova Branch:
```git branch -m [nome da nova branch]```

###### Adicionar repositorio remoto:
```git remoto add [apelido para o repo, convencinalmento usado "origin"] [link de repositorio remoto]```

###### Enviar alterações paraa o repositorio remoto:
```git push origin [repositorio remoto] [branch destino]```

###### Atualizar repositorio local baseado no remoto:
```git pull```

###### Clonar um repositorio remoto localmente:
```git clone [link do repositorio remoto]```

###### Remover arquivo:
```git rm [nome do arquivo]```

###### Exibir log de commits:
```git log (Para sair use Ctrl+c ou Ctrl+q ou q)```

###### Mover arquivo:
```git mv [arquivo inical] [caminho destino] (ao mover é possivel alterar o nome do arquivo no precesso)```

###### Desfazer todas as alterações e volta os arquivos para o estado original do repo remoto:
```git checkout```

###### Usando .gitignore:
```Dentro do projeto crie um aquivo chamado .gitignore, dentro dele indique os arqui e diretoris que o git deve ignorar```

###### Resetar uma branch se baseando em outra branch:
```git reset --hard (força o reset) [branch a base para o reset]```


#### Branch's:

###### Listar branch's:
```git branch```

###### Criar uma nova branch:
```git branch [nome da nova branch] (A copia sera baseada na branch que vôce está)```

###### Deletar branch:
```git brach -d ou --delete [nome da branch que deseja deletar]```

###### Trocar de bransh:
```git checkout -b [nome da branch que deseja acesar] (alterações não "comitadas" serão selavados para a nova branch)``` 

###### Mesclar branch's:
```git merge [branch da qual dejesa puxar as alterações para mesclar]```

##### Stash:

###### Criar stash:
```git stash [cria salva as alterações feitas um stash e apaga todas as alterações feitas]```

###### Listar as stash's:
```git stash```

######  Recuperar stash:
```git stash apply [id da stash]```

###### Mostar as alterações feitas salvas na stash: 
```git stash show -p [id da stash]```

###### Deletar uma stash:
```git stash drop [id da stash]```

###### Deletar todas as stash's:
```git stash clear```

##### Tag:

###### Criar Tag "Checkpoint":
```git tag -a [nome da tag] -m "mensagem descrevendo a tag"```

###### Lista tag:
```git tag```

###### Mostra alterações feitas na tag:
```git show [nome da tag]```

###### Trocar de tag:
```git checkout [nome da tag]```

###### Enviar tag para o repo remoto:
```git push origin [nome da tag ou --tags para todas as tags]```

###### Deletar tag:
```git tag -d ou --delete [nome da tag]```

#### Integração com repositorio remoto:

###### Encontrar novos branch's no repositorio remoto:
```git fetch -a```

###### Adicionar subemodulo:
```git submodule add [link do submodulo]```

###### Atualizar submodulo:
``` cd [caminho do submodulo]``` <br>
```git pull```

###### Commit no submodulo:
``` cd [caminho do submodulo]``` <br>
```git commit -m "menssagem"```

###### Enviar atualizações para o repositorio remoto do submodulo:
```git push --recurse-submodules=on-demand```

#### Analize e inspeção:

###### Exibr alterações feitas:
```git show```

###### Comparar diferenças entre 2 arquivos ou branch's:
```git diff [nome da branch]```
```git diff [branch_a:arquivo_a] [branch_b:arquivo_b]```

###### Exibir log resumido de commit's:
```git shortlog```

##### Administração de repositorio:

###### Excluir todos os arquivos untracked:
```git clean -f```

###### Otimizar repositorio:
```git gc```

###### Checar integridade dos arquivos:
```git fsck```

###### Listar **todas** as alterações feitas nos repositorio (por padrão apenas dos ultimos 30 dias):
```git reflog```

###### Restaurar para um commit anterior:
```git reset --hard [hash]```

###### Transformar uma branch em um arquivo .zip:
```git archive --format zip --output [nome_do_arquivo.zip] [branch de referencia]```

#### Melhorando commits

###### Remover commit's desnecessários
```git rebase [branch que ira receber apenas os commits necessarios] [branch de desenvolvimento] -i```

###### Dicas para mensagens de commit
```Separar o assunto do corpo do mensagem aperte {Enter} antes de fechar as aspas para quebrar linha```<br>
```Assunto com no maáximo 50 caracteres, iniciando com letra maiúscula```<br>
```Corpo explicando alterações no mámixo 72 caracteres```

#### MarkDown

# Titulos
## Titulos
### Titulos
#### Titulos
##### Titulos
###### Titulos

*Italico* _Italico_

**Negrito** __Negrito__

_**Italico em Negrito**_

1. Lista ordenada
    1. item
2. topico

> box

###### Imagem
![Logo da Compassa Uol](https://logospng.org/wp-content/uploads/compasso-uol.png)

[Meu linkedin](https://www.linkedin.com/in/leonardoteixeira23/)

[![Logo Linkedin](https://cdn-icons-png.flaticon.com/512/174/174857.png)](https://www.linkedin.com/in/leonardoteixeira23/)


```javascript
let codigo = "Codigo aqui"
```

- [x] tarefa 1
- [ ] tarefa 2
 
