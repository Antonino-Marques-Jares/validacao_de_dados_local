# Validação de dados local com python

## Correções a serem feitas

* Dados Faltantes (Cidade)
* Dados Duplicados (ID)
* Dados Inválidos (CNPJ)
* Dados Conflitantes

## Características principais de DADOS DE REFEÊNCIA:
*  **Estabilidade** - Mudam raramente.
* **Compartilhamento** - São usados por múltiplas áreas, sistemas e processos.
* **Padronização** - Seguem normas externas ou internas.
* **Volume pequeno** - São conjuntos pequenos de dados.
* **Baixa complexidade estrutural** -
Geralmente tabelas simples
* **Alta criticidade** -
Não pode ter erros em dados de referência porque propagam-se por todo o ecossistema.
* **Governança forte** -
Devem ter dono (owner), curador e processo formal de mudança.
* **Origem geralmente externa**

## Definindo Plano de Ação

### 1. Criação das regras de qualidade de dados
1. Consistência - Os mesmos dados devem ter os mesmos valores em diferentes tabelas, sistemas ou momentos, sem contradições.
2. Conformidade - Os dados seguem um formato, padrão ou regra de negócio definido (máscaras, domínios, unidades, padrões do setor).
3. Disponibilidade - O dado está acessível quando e onde é necessário — sem indisponibilidade, latência excessiva ou falta de permissão.
4. Integridade - Os dados mantêm relacionamentos e restrições corretos (chaves primárias, estrangeiras, unicidade, não-nulos)
5. Precisão - O dado representa corretamente a realidade que ele descreve.
6. Completude - Todos os dados necessários estão presentes — sem campos faltantes, nulos indevidos ou registros ausentes.

### Suposições a serem verificadas
Será que o estado do registro é válido ? -> testar se o estado é um dos estados brasileiros
Será que existe a cidade informada realmente pertence aquele estado ? -> testar se aquela cidade pertence aquele estado.
Será que este registro está completo ? -> testar se existe algum dado nulo.
Será que o CNPJ atende à conformidade ? -> Testar se o CNPJ tem 14 digitos
Será que existe mais de um registro para o mesmo ID ?
Será que existe mais de um registro para um determinado cliente ?

### 2. Retificar os Dados que não passam na qualidade de dados
### 3. Identificar a responsabilidade sobre os dados

