# Configurações de projeto (Python)

1) Locais de arquivos e pastas
- Pasta de testes: `tests`
- Arquivos de testes: iniciados com `test_`
- Ambiente virtual: `env`
- Arquivo de Dependências: `requirements.txt`
- Pasta de arquivos Protocol Buffer: `protos`

2) Bibliotecas necessárias
- pre-commit
- pylint
- pytest
- pytest-cov
- black
- flake8
- isort

3) Arquivos extras no projeto
- .coveragerc (cobertura)
- .pylintrc (padronização)
- .gitignore (renomear a extensão)
- .pre-commit-config.yaml (pre-commit)

4) Instalação
4.1) Instalar dependências
4.2) Executar `pre-commit install`

5) Comandos antes de um push

5.1) Executar `pre-commit run --all-files`

5.2) Testes com cobertura e fluxo `pytest --cov`
