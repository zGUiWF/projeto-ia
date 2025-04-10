## Abrir no GitBash
- Clone:
git clone https://github.com/SEU_USUARIO/projeto-ia.git

- Abrir Projeto:
cd projeto-ia

- Criar ambiente conda:
conda env create -f environment.yml

- Ativar ambiente conda:(Ativar sempre que for mexer no Projeto, funciona como uma venv)
conda activate projeto-ia


## Extensões VScode recomendadas
- Jupyter : Para compatibilidade com jupyter notebook
- Python : Pacotes padrão python
- Rainbow CSV : Melhor visualização de arquivos CSV
- Reload : Restart VScode
- GitLens : Mostra histórico de cada linha, comparação de branches, visualizações de merge
- Better Comments : Destaca tipos diferentes de comentários (TODO, !importante, ?pergunta, etc.)
- Path Intellisense : Autocompleta caminhos de arquivos (útil ao lidar com dados, .csv, imagens, etc.)


## Estrutura
- `data/`: Arquivos de dados brutos (.csv),(Não alterar base "dados_projeto_evasão_teste/treino.csv", duplique e coloque seu nome no arquivo para alterações)

- `notebooks/`: Notebooks exploratórios(Coloque seu nome no seu notebook)

- `models/`: Modelos salvos
    - Nescessario para uso : `import joblib`
    - Salvar modelo : `joblib.dump(modelo, 'models/NOME DO MODEL SALVO.joblib')`
    - Carregar modelo : `modelo_carregado = joblib.load('models/NOME DO MODEL SALVO.joblib')`


## Ao rodar um notebook colocar kernel conda
- Play code > Python Environments > projeto-ia (Python 3.10.16)


OBS:esse não é o README final