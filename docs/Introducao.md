# Introdução

AtechExecAuto é uma API REST, com único método POST, com propósito de executar uma rotina automática no Protheus (MsExecAuto).

* Recebe JSON e devolve JSON;
* É capaz de executar qualquer programa exposto no Protheus para chamada via MsExecAuto para qualquer empresa/filial;
* É capaz de obter uma numeração automática para os casos de inclusão de registro (como novo pedido de venda, nova ordem de produção, ...);
* É capaz de executar "posicionamento de cursor" antes da chamada ao MsExecAuto, como é exigido para algumas operações. Por exemplo: exclusão de OP;
* Posicionamento de cursor consiste em percorrer um índice de uma tabela do Protheus em busca de um valor pré-determinado. Exemplo: localizar a OP a ser excluída.
* A sequência das operações é a seguinte:
1. preparação do ambiente (seleção de empresa e filial);
2. obtenção da numeração automática;
3. posicionamento de cursor;
4. MsExecAuto.

> Mais informações detalhadas na [página Wiki do AtechExecAuto](http://portal.automatech.com.br/projects/analise-desenvolvimento/wiki/API_REST_universal_para_MsExecAuto).