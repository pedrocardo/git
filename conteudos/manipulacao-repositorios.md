# Manipulação de repositórios

Repositórios podem ser manipulados através de interfaces de linha de comando.

Os comandos são sempre precedidos por _git_.

## _Placeholders_

Em blocos de código nesse arquivo, colchetes são utilizados para demarcar _placeholders_.

```
git comando [placeholder]
```

## Comandos

Os comandos descritos nesse arquivo estão listados a seguir.

- [_add_](#add)
- [_branch_](#branch)
- [_checkout_](#checkout)
- [_clone_](#clone)
- [_commit_](#commit)
- [_config_](#config)
- [_init_](#init)
- [_log_](#log)
- [_merge_](#merge)
- [_pull_](#pull)
- [_push_](#push)
- [_remote_](#remote)
- [_reset_](#reset)
- [_revert_](#revert)
- [_show_](#show)
- [_status_](#status)

### _add_

Comando _add_ adiciona um ou mais arquivos a área _staging_.

```
git add [arquivo]
git add *
git add *.txt
```

### _branch_

Comando _branch_ exibe uma lista de _branches_ do repositório. Nessa lista, a _branch_ com asterisco será a atual.

```
git branch
```

O comando _branch_ com nome cria uma nova _branch_ com o nome especificado.

```
git branch [nome]
```

O comando _branch_ com _-d_ remove a _branch_ especificada se ela não tiver mudanças em relação a _branch_ _master_ ou tiver sido mesclada.

```
git branch -d [branch]
```

O comando _branch_ com _-D_ remove a _branch_ especificada independente de mudanças.

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

### _checkout_

Comando _checkout_ com _commit_ retorna a área _working_ para a versão do _commit_ determinado, criando uma nova _branch_.

```
git checkout [commit]
```

O comando _checkout_ com _branch_ muda para a _branch_ especificada.

```
git checkout [branch]
```

### _clone_

Comando _clone_ baixa um clone de um repositório remoto.

```
git clone [repositório remoto]
```

### _commit_

Comando _commit_ confirma as mudanças que estão na área _staging_ para o repositório.

```
git commit -m "[mensagem]"
```

O comando _commit_ com _-a_ pula a área _staging_ e confirma as mudanças que estão na área _working_ para o repositório.

```
git commit -a -m "[mensagem]"
git commit -am "[mensagem]"
```

O comando _commit_ com _--amend_ confirma as mudanças que estão na área _staging_ para o último _commit_ do repositório.

```
git commit --amend
```

### _config_

Comando _config_ pode modificar ou acessar variáveis locais e globais.

Variáveis globais ficam no arquivo _.gitconfig_.

O comando _config_ com _--global_ _user.name_ modifica a variável global que armazena o nome do usuário.

```
git config --global user.name [nome do usuário]
```

O comando _config_ com _--global_ _user.email_ modifica a variável global que armazena o e-mail do usuário.

```
git config --global user.email [e-mail do usuário]
```

O comando _config_ com _--list_ exibe uma lista de variáveis configuradas.

```
git config --list
```

### _init_

Comando _init_ inicia um repositório no diretório.

```
git init
```

### _log_

Comando _log_ exibe informações sobre os _commits_ realizados.

```
git log
git log --oneline
```

### _merge_

Comando _merge_ mescla a _branch_ atual com a especificada.

```
git merge [branch]
```

### _pull_

Comando _pull_ baixa as modificações de uma _branch_ de um repositório remoto no repositório local.

```
git pull [repositório remoto] [branch]
```

### _push_

Comando _push_ envia as modificações do repositório local para uma _branch_ do repositório remoto.

```
git push [repositório remoto] [branch]
```

### _remote_

Comando _remote_ com _add_ adiciona um nome para referenciar um repositório remoto.

```
git remote add [nome] [URL repositório remoto]
```

O comando _remote_ com _-v_ exibe uma lista dos repositórios remotos salvos.

```
git remote -v
```

### _reset_

Comando _reset_ remove todos ou um arquivo específico da área _staging_.

```
git reset
git reset [arquivo]
```

O comando _reset_ com _--hard_ reseta as áreas _staging_ e _working_ para a versão do _commit_ anterior ou um outro.

Esse comando não deve ser utilizado quando os _commits_ estiverem em um repositório remoto.

```
git reset --hard
git reset --hard [commmit]
```

### _revert_

Comando _revert_ cria um novo _commit_ com base na reversão de outro.

```
git revert [commit]
```

### _show_

Comando _show_ exibe informações sobre o último _commit_ ou outro.

```
git show
git show [commit]
```

### _status_

Comando _status_ exibe informações sobre o estado do repositório no momento do comando.

```
git status
git status -s
```
