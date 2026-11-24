# aula-ml

Classificador de chamados (comum ou urgente) com versionamento de dados e modelos via DVC.

## Pré-requisitos

- Git
- Python 3.10 ou superior
- DVC 3 (`pip install dvc`)

## Armazenamento DVC

O remote padrão é `storage`, apontando para `../dvc-storage`. Confira com `dvc remote list`.

## Restauração de uma versão

    git clone https://github.com/Kadson-Sousa/aula-ml.git aula-ml-restauracao
    cd aula-ml-restauracao
    git switch --detach modelo-r1
    dvc pull

## Treinamento

    python src/train.py <model_id>

Versões disponíveis: `dados-v1`, `dados-v2`, `modelo-r1` e `modelo-r2`.
