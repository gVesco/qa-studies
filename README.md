# Desafios de Código: Formação Quality Assurance (QA) Experience da DIO

Repositório criado para centralizar os desafios de projeto para os estudos de QA.

## Git e GitHub

<details close>
<summary>Commit e Pull Request</summary>

* Criar nova branch
    ```bash
    git checkout -b fix-18074
    ```

* Realizar as alterações desejadas

* Adicionar arquivos no stage
    ```bash
    git add
    ```

* Commitar alterações
    ```bash
    git commit -m "COF #18074 - Corrige parâmetro Elemento do processo ProcZCEDCriarLinhasPlanilhamento"
    ```

* Enviar por push as alterações para a branch criada
    ```bash
    git push --set-upstream origin fix-18074
    ```

* Reverter push por hash do commit
    ```bash
    git revert 860e984e9fd70fe906ebde0f76ca1e4d403b4f0b -m 1
    ```

* Pesquisar por Alterações em Commits Anteriores
    ```bash
    git log --grep "15898”
    ```

</details>
<details close>
<summary>Excluir Branch</summary>

* Realizar checkout para outra branch
    ```bash
    git checkout development-brerp
    ```

* Deletar branch desejada
    ```bash
    git branch -d fix-17252
    ```

</details>
<details close>
<summary>Resolver Conflitos</summary>

* Verificar último commit de cada branch
    ```bash
    git branch -v
    ```

* Mesclar as alterações da branch 'teste' para branch 'main'
    ```bash
    git checkout main
    ```

    ```bash
    git merge teste
    ```

* Baixar alterações do remoto 'origin' na branch 'main'
    ```bash
    git fetch origin main
    ```

* Verificar diferenças entre as duas
    ```bash
    git diff main origin/main
    ```

* Trazer alterações da branch remota
    ```bash
    git merge origin/main
    ```

* Descartar a alteração do último commit mantendo em stage
    ```bash
    git reset --soft HEAD~1
    ```

* Descartar todas alterações da branch atual
    ```bash
    git reset --hard
    ```

* Clonar apenas uma branch de um repositório
    ```bash
    git clone {URL} --branch {NOME-BRANCH} --single-branch
    ```

</details>
<details close>
<summary>Arquivar modificações atuais</summary>

* Arquiva atualizações
    ```bash
    git stash
    ```

* Lista alterações arquivadas
    ```bash
    git stash list
    ```

* Inspecionar arquivados
    ```bash
    git stash show
    ```

* Trás de volta alterações arquivadas e descarta o atual
    ```bash
    git stash pop
    ```

* Trás de volta alterações igual o pop, mas ainda mantém arquivado
    ```bash
    git stash apply
    ```

</details>

## Links Úteis

[Basic Syntax Markdown](https://www.markdownguide.org/basic-syntax/)