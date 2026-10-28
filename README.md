# 🗂️ Cadastro de Equipe

Sistema de terminal em Python para cadastrar, listar, alterar e excluir **clientes** e **produtos**, com os dados salvos em arquivos de texto.

---

## ✨ Funcionalidades

| Módulo | Operações |
|---|---|
| 👤 **Clientes** | Cadastrar, listar, alterar e excluir |
| 📦 **Produtos** | Cadastrar, listar, alterar e excluir |

Os menus usam cores e caixas desenhadas no terminal para facilitar a leitura.

---

## 🧰 Requisitos

- Python 3.8 ou superior
- Biblioteca [colorama](https://pypi.org/project/colorama/)

```bash
pip install colorama
```

---

## 🚀 Como executar

Dentro da pasta do projeto, rode:

```bash
python main.py
```

Use os números do menu para navegar. Escolha `0` para voltar ou sair.

---

## 📁 Estrutura

```
cadastro_equipe-main/
├── main.py               # Menu principal e submenus
├── cadastro_cliente.py   # Operações sobre clientes
└── cadastro_produto.py   # Operações sobre produtos
```

Os arquivos de dados são criados automaticamente na pasta de execução:

| Arquivo | Conteúdo | Formato de cada linha |
|---|---|---|
| `dados_clientes.txt` | Clientes | `nome;email;telefone` |
| `dados_prod.txt` | Produtos | `nome;valor;quantidade` |

---

## ✅ Regras de preenchimento

**Clientes**
- **Nome:** obrigatório, somente letras e espaços.
- **E-mail:** precisa terminar em `@gmail.com`, sem espaços e sem hífen.
- **Telefone:** celular com 9 ou 11 dígitos. O hífen é aceito e removido automaticamente.

**Produtos**
- **Nome:** obrigatório, somente letras e espaços.
- **Valor unitário:** número positivo. Aceita vírgula ou ponto como separador decimal.
- **Quantidade:** número inteiro positivo.

---

## 🔎 Como as buscas funcionam

Alterar e excluir usam o **nome** informado para localizar o registro. A busca não diferencia maiúsculas de minúsculas, porque o nome é formatado com inicial maiúscula antes da comparação.
