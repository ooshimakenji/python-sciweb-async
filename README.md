# Robô SEMASA Assíncrono

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white) ![asyncio](https://img.shields.io/badge/asyncio-paralelo-blue) ![Playwright](https://img.shields.io/badge/Playwright-async-2EAD33?logo=playwright&logoColor=white) ![Licença](https://img.shields.io/badge/licença-MIT-green)

Versão assíncrona do robô SEMASA. Utiliza `asyncio` com Playwright para processar múltiplos registros em paralelo, reduzindo significativamente o tempo total de automação em lotes grandes.

## Diferenças em relação ao python-sciweb

| Característica | python-sciweb | python-sciweb-async |
|---|---|---|
| Execução | Sequencial | Paralela |
| Motor | Playwright síncrono | Playwright async |
| Ideal para | Lotes pequenos | Lotes grandes |

## Stack

- **Python 3.x** + `playwright` (async)
- **asyncio** para execução paralela
- **Pandas** para leitura e escrita de planilhas Excel
- **python-dotenv** para gestão de credenciais

## Instalação

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
playwright install chromium
```

## Configuração

Copie `.env.example` para `.env`:

```dotenv
SEMASA_USUARIO=SEU_USUARIO
SEMASA_SENHA=SUA_SENHA
```

## Execução

```powershell
python main.py --excel dados.xlsx
```

## Licença

MIT


## Contribuindo / Contributing

Contribuições são bem-vindas! Abra uma issue ou envie um pull request.  
Contributions are welcome! Feel free to open an issue or submit a pull request.
