# Configurações de projeto (Python)

1) Locais de arquivos e pastas
- Pasta de testes: `tests`
- Arquivos de testes: iniciados com `test_`
- Ambiente virtual: `env`
- Arquivo de Dependências: `requirements.txt`
- Pasta de arquivos Protocol Buffer: `protos`

2) Bibliotecas necessárias
- pylint
- pytest
- pytest-cov
- black

3) Arquivos extras no projeto
- .coveragerc (cobertura)
- .pylintrc (padronização)
- .gitignore (renomear a extensão)

3) Comandos antes de um push

3.1) Reestruturação do projeto 
`python -m black . --line-length 80`

3.2) Checagem de padronização de código
- (Windows) `forfiles /s /m *.py /c "cmd /c echo @relpath" | findstr /v "env migrations _pb2.py _pb2_grpc.py" | xargs pylint`
- (Linux) `find . -name "*.py" -and -not -name "0*.py" | xargs pylint`

3.3) Testes com cobertura e fluxo
`pytest --cov`
