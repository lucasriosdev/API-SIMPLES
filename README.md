## 🚀 API Simples
Um projeto de API básica desenvolvida para fins educacionais e como ponto de partida para aplicações mais complexas.

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-18.x-green?logo=node.js" alt="Node Version">
  <img src="https://img.shields.io/badge/Express-4.x-blue?logo=express" alt="Express Version">
</p>

## 📌 Pré-requisitos

```bash
# Versões compativeis
Node.js >= 18.0.0
npm >= 9.0.0
```

## 🛠 Instalação Rápida

```bash
# Clone o projeto
git clone https://github.com/lucasriosdev/API-SIMPLES.git && cd API-SIMPLES

# Instale as dependências
npm install

# Inicie em modo desenvolvimento
npm run dev
```

## 🌐 Rotas da API

| Método | Endpoint       | Body Example                  | Descrição           |
|--------|----------------|-------------------------------|---------------------|
| `GET`  | `/api/users`   | -                             | Lista todos usuários|
| `POST` | `/api/users`   | `{"name":"João","email":"joao@ex.com"}` | Cria novo usuário |

## 📦 Estrutura do Projeto

```plaintext
.
├── src/
│   ├── controllers/   # Lógica dos endpoints
│   ├── routes/        # Definição de rotas
│   └── app.js         # Configuração principal
├── .env.example       # Variáveis de ambiente
├── package.json       # Dependências
└── README.md          # Documentação
```

## 🧪 Testando a API

```http
POST http://localhost:3000/api/users
Content-Type: application/json

{
  "name": "Maria Silva",
  "email": "maria@exemplo.com"
}
```

**Resposta esperada:**
```json
{
  "id": 1,
  "name": "Maria Silva",
  "email": "maria@exemplo.com",
  "createdAt": "2023-08-20T12:00:00.000Z"
}
```

## 🚨 Troubleshooting

```bash
# Erro: Porta em uso
lsof -i :3000
kill -9 <PID>

# Erro: Dependências faltando
rm -rf node_modules && npm install
```

## 📜 Licença

```text
MIT License © 2023 - Lucas Rios
```

---

<div align="center">
  <sub>Criado com</sub> 💻 <sub>por</sub> <a href="https://github.com/lucasriosdev">Lucas Rios</a>
</div>
```
