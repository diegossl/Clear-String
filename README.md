# Removedor de caracteres

Essa biblioteca tem a finalidade de tratar strings removendo ou subistituindo caracteres específicos ou genericos que estejam dentro do padrão UTF-8 (Hexadecimal).

## Uso

```javascript
const CharacterRemover = require('character-remover') 
```

## Features

A biblioteca possui as seguintes funcionalidades:

```javascript
  /*
    Nome: removeAccents
    Descrição: Remove todos os acentos de uma string.
    parametro: text = 'áàâãäéèêëíìïîóòôõöúûùüçñÁÀÂÃÄÉÊÈËÍÌÏÎÓÒÔÕÖÚÛÙÜÇÑ'
    saída: 'aaaaaeeeeiiiiooooouuuucnAAAAAEEEEIIIIOOOOOUUUUCN'
  */
  removeAccents (text)

  /*
    Nome: removeAll
    Descrição: Remove todos os caracteres especiais de uma string.
    parametro: text = '  ]-{&  } --- //          %   [~ Olá *-*. Tudo {[ bem?'
    saída: 'OláTudobem'
  */
  removeAll (text)

  /*
    Nome: removeOnly
    Descrição: Remove de uma string somente os caracteres especiais selecionados.
    parametro 1: text = 'Olá *-*. Tudo bem?'
    parametro 2: chars = ['*', '-']
    saída: 'Olá . Tudo bem?'
  */
  removeOnly (text, chars = [])

  /*
    Nome: removeExcept
    Descrição: Remove de uma string todos os caracteres especiais, exceto os selecionados.
    parametro 1: text = '  ]-{&  } --- //;          %   [~ Olá *-*. Tudo {[ bem?'
    parametro 2: chars = ['?', '.', ' ']
    saída: '                    Olá . Tudo  bem?'
  */
  removeExcept (text, chars = [])

  /*
    Nome: removeExtraSpaces
    Descrição: Remove todos os espaços extras de uma string.
    parametro: text = '                    Olá.                Tudo      bem?'
    saída: 'Olá. Tudo bem?'
  */
  removeExtraSpaces (text)
```

# Licença

MIT
