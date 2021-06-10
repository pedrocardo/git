# Comandos para exibir informações

Comando _status_ exibe informações sobre o estado do repositório no momento do comando.

```
git status
git status -s
```

Comando _log_ exibe informações sobre os _commits_ realizados.

```
git log
git log --oneline
```

Comando _show_ exibe informações sobre o último _commit_ ou outro.

```
git show
git show [commit]
```

Comando _diff_ exibe as diferenças entre os arquivos que estão nas área _working_ e _repository_.

```
git diff
git diff [arquivo]
```

O comando _diff_ com _--staged_ exibe as diferenças entre os arquivos que estão nas área _staging_ e _repository_.

```
git diff --staged
git diff --staged [arquivo]
```
