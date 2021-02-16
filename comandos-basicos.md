# Comandos básicos

Comando _init_ inicia um repositório no diretório.

```
git init
```

Comando _add_ adiciona um ou mais arquivos a área _staging_.

```
git add [arquivo]
git add *
git add *.txt
```

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
