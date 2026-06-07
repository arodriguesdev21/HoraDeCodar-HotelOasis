# Sistema de Gestão Hoteleira - Hotel Oasis

## 📖 Descrição

O Sistema de Gestão Hoteleira Hotel Oasis foi desenvolvido em HTML e JavaScript com o objetivo de simular a operação básica de um hotel, permitindo o gerenciamento de reservas, controle de ocupação dos quartos e cadastro de hóspedes.

O projeto é dividido em dois módulos principais:

* **Módulo Principal do Hotel**
* **Módulo de Cadastro de Hóspedes**

A navegação entre os módulos é realizada por meio de páginas HTML independentes.

---

# 🚀 Funcionalidades

## 1. Autenticação de Usuário

Ao iniciar o sistema:

* Exibe mensagem de boas-vindas.
* Solicita o nome do usuário.
* Solicita senha de acesso.
* Permite até 3 tentativas.
* Bloqueia o acesso após exceder o número de tentativas.

---

## 2. Menu Principal

Após autenticação, o usuário pode acessar:

```text
1. Reservas de Quartos
2. Cadastro de Hóspedes
3. Eventos
4. Ar-Condicionado
5. Abastecimento
6. Relatórios Operacionais
7. Sair
```

---

# 🏨 Módulo de Reservas

Permite realizar reservas de quartos do hotel.

## Fluxo

1. Informar valor da diária.
2. Informar quantidade de diárias.
3. Informar nome do hóspede.
4. Selecionar tipo de quarto.
5. Escolher quarto disponível.
6. Confirmar reserva.

---


## Regras de Negócio

### Diárias

* Mínimo: 1 diária
* Máximo: 30 diárias

### Quartos

O hotel possui:

```text
20 quartos
```

Cada quarto pode estar:

* Livre
* Ocupado

Não é permitido reservar quartos já ocupados.

---

## Cálculo da Reserva

O sistema calcula:

```text
Subtotal = Diária × Quantidade de Dias × Fator do Quarto

Taxa de Serviço = 10%

Total = Subtotal + Taxa
```

---

## Mapa de Ocupação

Após uma reserva confirmada, o sistema exibe:

```text
[L] = Livre
[O] = Ocupado
```

Exemplo:

```text
[O] [L] [L] [O] [L]
[L] [O] [L] [L] [L]
[L] [L] [O] [L] [L]
[L] [L] [L] [L] [O]
```

---

# 👥 Módulo de Cadastro de Hóspedes

Responsável pelo gerenciamento dos hóspedes cadastrados.

---

## Menu de Cadastro

```text
1. Cadastrar
2. Pesquisar Exato
3. Pesquisar Prefixo
4. Listar
5. Atualizar
6. Remover
7. Voltar
```

---

## Cadastro de Hóspedes

Permite cadastrar hóspedes contendo:

* Nome
* Data/Hora do cadastro

---

### Limites

Máximo permitido:

---

### Validações

Não é permitido:

* Cadastrar hóspedes duplicados.
* Ultrapassar o limite de registros.

---

## Pesquisa Exata

Localiza hóspedes pelo nome completo.

---

## Pesquisa por Prefixo

Permite pesquisar hóspedes utilizando o início do nome.

---

## Listagem de Hóspedes

Exibe todos os hóspedes cadastrados:

* Ordenados alfabeticamente (A-Z)
* Com data e hora de cadastro

---

## Atualização

Permite alterar o nome de um hóspede utilizando seu índice.

---

## Remoção

Permite excluir hóspedes cadastrados utilizando seu índice.

---


# ⚙️ Tecnologias Utilizadas

* HTML5
* JavaScript ES6
* Browser API (Alert, Prompt e Confirm)

---

# 📂 Estrutura do Projeto

├── Hotel.html
├── CadastroDeHospedes.html
└── README.md

---

# 👨‍💻 Autor

Projeto acadêmico desenvolvido para prática de lógica de programação, manipulação de arrays, funções, estruturas condicionais e desenvolvimento de sistemas em JavaScript.
