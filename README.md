# CD

Notebooks e materiais da disciplina CD.

## Ambiente Python

Na raiz deste diretório, execute o comando abaixo para criar o ambiente virtual,
instalar as dependências e registrar o kernel do Jupyter:

```bash
python3 -m venv .venv && \
  .venv/bin/python -m pip install --upgrade pip && \
  .venv/bin/python -m pip install -r requirements.txt && \
  .venv/bin/python -m ipykernel install --user \
    --name ufes-cd \
    --display-name "Python — UFES CD"
```

No VS Code, abra o notebook e selecione o kernel **Python — UFES CD**.

Para confirmar que o notebook está usando o ambiente correto, execute em uma
célula:

```python
import sys

print(sys.executable)
```

O caminho exibido deve terminar em `CD/.venv/bin/python`. O diretório `.venv`
é local e está ignorado pelo Git; o ambiente pode ser recriado a qualquer
momento com o comando acima.
