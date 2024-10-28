# Desafios de Código: Formação Quality Assurance (QA) Experience da DIO

Repositório criado para centralizar os desafios de projeto para os estudos de QA.

## Git e GitHub

<details open>
<summary>Commit e Pull Request</summary>

* Criar nova branch
    > git checkout -b fix-18074

* Realizar as alterações desejadas

* Adicionar arquivos no stage
    > git add

* Commitar alterações
    > git commit -m "COF #18074 - Corrige parâmetro Elemento do processo ProcZCEDCriarLinhasPlanilhamento"

* Enviar por push as alterações para a branch criada
    > git push --set-upstream origin fix-18074

* Reverter push por hash do commit
    > git revert 860e984e9fd70fe906ebde0f76ca1e4d403b4f0b -m 1

* Pesquisar por Alterações em Commits Anteriores
    > git log --grep "15898”

</details>
<details open>
<summary>Excluir Branch</summary>

* Realizar checkout para outra branch
    > git checkout development-brerp

* Deletar branch desejada
    > git branch -d fix-17252

</details>
<details open>
<summary>Resolver Conflitos</summary>

* Verificar último commit de cada branch
    > git branch -v

* Mesclar as alterações da branch 'teste' para branch 'main'
    > git checkout main

    > git merge teste

* Baixar alterações do remoto 'origin' na branch 'main'
    > git fetch origin main

* Verificar diferenças entre as duas
    > git diff main origin/main

* Trazer alterações da branch remota
    > git merge origin/main

* Descartar a alteração do último commit mantendo em stage
    > git reset --soft HEAD~1

* Descartar todas alterações da branch atual
    > git reset --hard

</details>

* Clonar apenas uma branch de um repositório
    > git clone {URL} --branch {NOME-BRANCH} --single-branch

<details open>
<summary>Arquivar modificações atuais</summary>

* Arquiva atualizações
    > git stash

* Lista alterações arquivadas
    > git stash list

* Inspecionar arquivados
    > git stash show

* Trás de volta alterações arquivadas e descarta o atual
    > git stash pop

* Trás de volta alterações igual o pop, mas ainda mantém arquivado
    > git stash apply

</details>

## Links Úteis

[Basic Syntax Markdown](https://www.markdownguide.org/basic-syntax/)