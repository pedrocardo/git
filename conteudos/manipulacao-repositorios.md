# Manipulação de repositórios

Repositórios podem ser manipulados através de interfaces de linha de comando.

Os comandos são sempre precedidos por _git_.

## _Placeholders_

Em blocos de código, colchetes são utilizados para demarcar _placeholders_.

```
git comando [placeholder]
```

## Comandos

Os comandos descritos nesse arquivo estão listados a seguir.

- [Comando _add_](#comando-add)
- [Comando _branch_](#comando-branch)
- [Comando _checkout_](#comando-checkout)
- [Comando _clone_](#comando-clone)
- [Comando _commit_](#comando-commit)
- [Comando _config_](#comando-config)
- [Comando _init_](#comando-init)
- [Comando _log_](#comando-log)
- [Comando _merge_](#comando-merge)
- [Comando _pull_](#comando-pull)
- [Comando _push_](#comando-push)
- [Comando _remote_](#comando-remote)
- [Comando _reset_](#comando-reset)
- [Comando _revert_](#comando-revert)
- [Comando _show_](#comando-show)
- [Comando _status_](#comando-status)

### Comando _add_

Comando _add_ adiciona um ou mais itens a área _staging_.

```
git add [arquivo]
git add [diretório]
git add *
git add *.txt
```

### Comando _branch_

Comando _branch_ exibe a lista de _branches_ do repositório.

```
git branch
```

O comando _branch_ cria uma _branch_ com o nome especificado.

```
git branch [branch]
```

O comando _branch_ com _-d_ remove a _branch_ especificada se ela não tiver diferenças com a _branch_ _master_.

```
git branch -d [branch]
```

O comando _branch_ com _-D_ remove a _branch_ especificada independentemente de diferenças com a _branch_ _master_.

```
git branch -D [branch]
```

O comando _branch_ com _--merged_ exibe as _branches_ que estão mescladas com a atual.

```
git branch --merged
```

O comando _branch_ com _--no-merged_ exibe as _branches_ que não estão mescladas com a atual.

```
git branch --no-merged
```

### Comando _checkout_

Comando _checkout_ muda o repositório para a _branch_ especificada.

```
git checkout [branch]
```

### Comando _clone_

Comando _clone_ baixa um repositório remoto.

```
git clone [repositório remoto]
```

### Comando _commit_

Comando _commit_ confirma as mudanças que estão na área _staging_ para _repository_.

```
git commit -m "[mensagem]"
```

O comando _commit_ com _-a_ adiciona todos os arquivos para a área _staging_ e confirma as mudanças para _repository_.

```
git commit -a -m "[mensagem]"
git commit -am "[mensagem]"
```

O comando _commit_ com _--amend_ confirma as mudanças que estão na área _staging_ para o último _commit_ do repositório.

```
git commit --amend
```

### Comando _config_

Comando _config_ modifica ou acessa variáveis locais e globais.

Variáveis globais ficam no arquivo _.gitconfig_.

O comando _config_ com _--global_ _user.name_ modifica a variável global que referencia o nome do usuário.

```
git config --global user.name "[nome]"
```

O comando _config_ com _--global_ _user.email_ modifica a variável global que referencia o e-mail do usuário.

```
git config --global user.email "[e-mail]"
```

O comando _config_ com _--list_ exibe uma lista de variáveis configuradas.

```
git config --list
```

### Comando _init_

Comando _init_ inicia um repositório no diretório.

```
git init
```

### Comando _log_

Comando _log_ exibe informações sobre os _commits_ realizados.

```
git log
git log --oneline
```

### Comando _merge_

Comando _merge_ mescla a _branch_ do repositório com a especificada.

```
git merge [branch]
```

### Comando _pull_

Comando _pull_ baixa as modificações de uma _branch_ de um repositório remoto.

```
git pull [nome repositório remoto] [branch]
```

### Comando _push_

Comando _push_ envia as modificações do repositório local para uma _branch_ do repositório remoto.

```
git push [nome repositório remoto] [branch]
```

### Comando _remote_

Comando _remote_ com _add_ adiciona um nome para referenciar um repositório remoto.

```
git remote add [nome repositório remoto] [URL repositório remoto]
```

O comando _remote_ com _-v_ exibe uma lista dos repositórios remotos salvos.

```
git remote -v
```

### Comando _reset_

Comando _reset_ remove todos ou um item específico da área _staging_.

```
git reset
git reset [item]
```

O comando _reset_ com _--hard_ restaura as áreas _staging_ e _working_ para a versão do _commit_ anterior ou um outro.

Esse comando não deve ser utilizado quando os _commits_ estiverem em um repositório remoto.

```
git reset --hard
git reset --hard [commmit]
```

### Comando _revert_

Comando _revert_ retorna o estado do repositório para a versão do _commit_ especificado.

Essa reversão criará um novo _commit_.

```
git revert [commit]
```

### Comando _show_

Comando _show_ exibe informações sobre o último _commit_ ou um outro especificado.

```
git show
git show [commit]
```

### Comando _status_

Comando _status_ exibe o estado do repositório no momento do comando.

```
git status
git status -s
```
