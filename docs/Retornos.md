# Retornos

A resposta da API é sempre no formato do JSON,

|resultCode|Significado|
|----------|-----------|
|000|Sucesso (genérico)|
|001|Sucesso com numeração automática gerada|
|100|Parâmetros inválidos (genérico)|
|101|Parâmetros inválidos para preparação de ambiente|
|102|Parâmetros inválidos para numeração automática|
|103|Parâmetros inválidos para posicionamento de cursor|
|104|Parâmetros inválidos para MsExecAuto|
|200|Falha de preparação de ambiente (genérica)|
|300|Falha de posicionamento de cursor (genérica)|
|301|Falha de posicionamento de cursor (valor não encontrado no índice)|
|400|Falha durante o processo de preparação e invocação do MsExecAuto (genérica)|
|500|MsExecAuto executou e retornou com falha (genérico)|
|700|Falha tratada na camada de API REST (genérica)|
|701|Falha tratada na camada de API REST: corpo da requisição chegou vazio|
|800|Falha tratada na camada de interface JSON (genérica)|
|801|Falha tratada na camada de interface JSON: o texto recebido não é um JSON|
|802|Falha tratada na camada de interface JSON: o JSON recebido não atende ao schema esperado|
|900|Exceção não tratada (genérica)|
|901|Exceção não tratada na camada do AtechExecAuto|
|902|Exceção não tratada na camada da interface JSON|