# Consulta CEP

Aplicação web simples para consultar endereços a partir de um CEP brasileiro usando a API pública ViaCEP.

## Visão Geral

O projeto consiste em uma interface web estática feita com HTML, CSS e JavaScript puro. O usuário informa um CEP, a aplicação valida o valor digitado, faz a requisição para a API e exibe os dados retornados do endereço.

## Preview
<img width="998" height="837" alt="image" src="https://github.com/user-attachments/assets/ad9eadbf-a364-4f02-927d-c0df28b60182" />


## Funcionalidades

- Consulta de CEPs do Brasil via API ViaCEP
- Validação de campo vazio
- Validação de CEP com exatamente 8 dígitos
- Exibição de mensagem para CEP inválido
- Interface visual moderna com layout centralizado

## Tecnologias

- HTML5
- CSS3
- JavaScript
- API ViaCEP

## Estrutura do Projeto

```text
Consulta CEP/
├── index.html
├── README.md
└── src/
	├── script.js
	└── style.css
```

## Instalação

Como este projeto é estático, não há necessidade de instalação de dependências.


## Como Funciona

1. O valor digitado no campo é capturado pelo JavaScript.
2. Todos os caracteres não numéricos são removidos.
3. O sistema verifica se o CEP foi informado corretamente.
4. A aplicação faz uma requisição para `https://viacep.com.br/ws/{cep}/json/`.
5. Os dados do endereço são exibidos na tela.

## Exemplo de Retorno Exibido

- CEP
- Logradouro
- Bairro
- Cidade
- Estado

## Regras de Validação

- Se o campo estiver vazio, a aplicação solicita que o usuário informe um CEP.
- Se o CEP não tiver 8 dígitos, a aplicação exibe uma mensagem de erro.
- Se a API retornar um CEP inexistente, a aplicação informa que o CEP é inválido.

## Observações

- O projeto depende de conexão com a internet para consultar a API.
- Atualmente não há tratamento específico para falhas de rede ou indisponibilidade da API.

## Melhorias planejadas

- [ ] Buscar o CEP ao pressionar Enter
- [ ] Adicionar máscara de preenchimento no campo
- [ ] Exibir estado de carregamento durante a consulta
- [ ] Tratar erros de conexão com mensagens mais clara

## API Utilizada

Documentação oficial: https://viacep.com.br/

## Autor
Desenvolvido por Gabriel Izidoro para estudos de desenvolvimento web.
