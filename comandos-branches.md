# Comandos para manipular _branches_

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

Comando _merge_ mescla a _branch_ atual com a especificada.

```
git merge [branch]
```

O comando _branch_ com _--merged_ exibe as _branches_ que estão mescladas com a atual.

```
git branch --merged
```

O comando _branch_ com _--no-merged_ exibe as _branches_ que não estão mescladas com a atual.

```
git branch --no-merged
```
