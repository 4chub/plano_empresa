## Endpoint de Login

### **POST** `/api/Login`

**Descrição:** Efetua login na API para obter o token necessário para autenticação.

### Parâmetros

- **Sem parâmetros de URL**

### Corpo da Requisição

Formato `application/json`:

```json
{
  "username": "string",
  "password": "string"
}
```

### Respostas

- **200 OK**: Retorna o token e a validade.
- **400 Bad Request**: Falha na autenticação.

---

# Endpoint: GET /api/PlanoEmpresa/Pagina/{page}

Obtém a lista de planos, quantidade de clientes e quantidade contratado de cada empresa de forma paginada.

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
