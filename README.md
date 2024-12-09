# Endpoint: GET /api/PlanoEmpresa/Pagina/{page}

Obtém a lista de planos de empresas de forma paginada.

---

## **Parâmetros**

### **Path Parameters**
| Nome | Tipo        | Descrição                   | Obrigatório |
|------|-------------|-----------------------------|-------------|
| page | integer(int32) | Número da página desejada   | Sim         |

### **Query Parameters**
| Nome              | Tipo            | Descrição                                    | Obrigatório |
|-------------------|-----------------|--------------------------------------------|-------------|
| pageSize          | integer(int32) | Número de itens por página                  | Não         |
| empresaId         | integer(int32) | ID da empresa para filtrar os planos        | Não         |
| nomePlaneo        | string         | Nome do plano para filtrar                  | Não         |
| dtContratacao     | string         | Data inicial de contratação (YYYY-MM-DD)    | Não         |
| dtContratacaoFim  | string         | Data final de contratação (YYYY-MM-DD)      | Não         |

---

## **Respostas**

### **200 - Sucesso**
- Descrição: Solicitação bem-sucedida.
- Media type: `application/json`
- Exemplo de resposta:
  ```json
  {
    "type": "string",
    "title": "string",
    "status": 0,
    "detail": "string",
    "instance": "string",
    "additionalProp1": "string",
    "additionalProp2": "string",
    "additionalProp3": "string"
  }
