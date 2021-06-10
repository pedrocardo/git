# Comandos para reversão

Comando _revert_ cria um novo _commit_ com base na reversão de outro.

```
git revert [commit]
```

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
