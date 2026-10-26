# TechBairro

A TechBairro é um sistema de cadastro de clientes desenvolvido em Python para a associação de moradores. Ele permite cadastrar, consultar, alterar e excluir informações dos clientes.

**Versão atual:** 3.3.1 · Histórico de mudanças no [CHANGELOG](CHANGELOG.md)

## Funcionalidades

- Cadastro de clientes com nome, telefone, e-mail e endereço.
- Consulta, alteração e exclusão de clientes cadastrados.

## Requisitos para execução

| Item | Requisito |
|---|---|
| Sistema operacional | Windows, Linux ou macOS |
| Python | Python 3 instalado (versão testada: confirmar no computador) |
| Tkinter | Necessário para a interface gráfica |
| Bibliotecas externas | Nenhuma |
| Internet | Necessária para baixar o projeto; não é necessária para utilizar o programa depois de instalado |

## Instalação

### Opção 1: Baixar com Git

1. Instale o Python e o Git no computador.
2. Abra o terminal e execute:

```bash
git clone https://github.com/baracho061/techbairro.git
```

3. Entre na pasta do projeto:

```bash
cd techbairro
```

4. Confira a versão do Python:

```bash
python --version
```

5. Verifique se o Tkinter está funcionando:

```bash
python -m tkinter
```

6. Instale as dependências, se necessário:

```bash
pip install -r requirements.txt
```

7. Execute o programa:

```bash
python techbairro.py
```

### Opção 2: Baixar pelo GitHub

1. Acesse o repositório: https://github.com/baracho061/techbairro
2. Clique em **Code** e depois em **Download ZIP**.
3. Extraia o arquivo ZIP.
4. Abra a pasta extraída no terminal.
5. Execute:

```bash
python techbairro.py
```

Ao abrir, deverá aparecer a janela de cadastro da TechBairro. No terminal, confira a mensagem `Banco em uso` para identificar o arquivo de banco de dados utilizado.

## Configuração do banco de dados

A TechBairro utiliza o SQLite para armazenar os dados dos clientes. O arquivo `techbairro.db` é criado quando o programa inicializa o banco de dados, caso ele ainda não exista.

A mensagem `Banco em uso`, exibida no terminal, informa o caminho do banco de dados utilizado pelo programa.

O banco de dados não deve ser enviado ao GitHub, pois pode conter informações pessoais dos clientes, como nomes, telefones e e-mails.

Para fazer uma cópia de segurança, feche o programa e copie o arquivo `techbairro.db` para uma pasta segura. Guarde essa cópia em um local protegido.

## Como usar

O passo a passo está no [Manual de uso](docs/manual_de_uso.md).

## Estrutura do projeto

- `techbairro.py`: arquivo principal que inicia a aplicação e apresenta a interface.
- `cliente.py`: contém a classe que representa os dados de um cliente.
- `banco.py`: gerencia as operações relacionadas ao banco de dados.
- `validacao.py`: contém as regras de validação dos dados.
- `testar_validacao.py`: executa os testes das regras de validação.
- `scripts/`: pasta destinada a scripts auxiliares.
- `CHANGELOG.md`: registra as mudanças realizadas nas versões.
- `requirements.txt`: informa as dependências do projeto.
- `docs/manual_de_uso.md`: contém o manual para quem utiliza o sistema.

## Autor

Gabriel da Silva Baracho
Curso Técnico em Desenvolvimento de Sistemas  
Senac DF
