# `@lucasmod/pokemon.js`

<div align="center">
  
  ✨ **A maneira mais fácil de interagir com a PokéAPI no Node.js!** ✨
  
  <br>
  
  <!-- Badges Dinâmicos (Substituir 'lucasmod' pelo nome de usuário correto no GitHub para os badges de estrela/fork, se necessário) -->
  [![NPM Version](https://img.shields.io/npm/v/@lucasmod/pokemon.js?style=flat&logo=npm&color=red)](https://www.npmjs.com/package/@lucasmod/pokemon.js)
  [![NPM Downloads](https://img.shields.io/npm/dt/@lucasmod/pokemon.js?style=flat&logo=npm&color=blue)](https://www.npmjs.com/package/@lucasmod/pokemon.js)
  [![Node.js Version](https://img.shields.io/badge/Node.js-v12+-success?style=flat&logo=node.js)](https://nodejs.org/)
  [![License](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat)](https://opensource.org/licenses/MIT)
  
  <br>
  
  <!-- Imagem de Destaque (Mantendo a imagem original, mas centralizada com Markdown) -->
  <img src="https://i.postimg.cc/Sx7sKrmx/pokemon.png" alt="pokemon.js - Interaja com a PokéAPI" width="546" />
  
  <br>
  
</div>

---

## ⚡️ Sobre o Projeto

Esta é uma **versão corrigida e mantida** do pacote original `pokemon.js` [1], desenvolvida por **lucasmod**.

O foco desta versão é garantir a **compatibilidade total** com as versões mais recentes do Node.js, corrigindo o problema de importação de módulos (ESM) que afetava o pacote original. `@lucasmod/pokemon.js` é um módulo **Node.js** que simplifica a interação com a [PokéAPI](https://pokeapi.co/) [2], permitindo que você acesse dados de Pokémon, habilidades, movimentos e muito mais de forma rápida e eficiente.

## 🛠 Instalação

**Requisito:** Node.js **12.0.0** ou superior. Nenhuma dependência externa é necessária.

Utilize o `npm` para instalar o pacote em seu projeto:

```bash
npm install @lucasmod/pokemon.js
```

## 🚀 Exemplo de Uso

O pacote utiliza a sintaxe moderna de **ESM** (`import/export`).

```javascript
import Pokemon from '@lucasmod/pokemon.js';

// Busca os dados do Pokémon 'zorua' e imprime no console
Pokemon.get_pokemon('zorua').then(console.log);

/*
  Saída (Exemplo - Retorna o JSON completo da PokéAPI):
  {
    id: 570,
    name: 'zorua',
    height: 7,
    weight: 125,
    base_experience: 66,
    abilities: [ ... ],
    types: [ ... ],
    ... // O objeto completo é muito maior!
  }
*/
```

## 📚 Referência da API (Métodos)

Abaixo estão os métodos principais disponíveis no objeto `Pokemon`:

| Método | Descrição | Parâmetros | Retorno |
| :--- | :--- | :--- | :--- |
| `get_pokemon` | Retorna dados detalhados de um Pokémon. | `pokemon` (string), `fields` (array, opcional) | `Promise<Object>` (JSON do Pokémon) |
| `get_type` | Retorna dados de um tipo ou os tipos de um Pokémon. | `name` (string), `is_pokemon` (boolean, opcional), `fields` (array, opcional) | `Promise<Object>` (JSON do Tipo) ou `Promise<Array>` (Tipos do Pokémon) |
| `get_ability` | Retorna dados de uma habilidade ou as habilidades de um Pokémon. | `name` (string), `is_pokemon` (boolean, opcional), `fields` (array, opcional) | `Promise<Object>` (JSON da Habilidade) ou `Promise<Array>` (Habilidades do Pokémon) |
| `get_evolution_line` | Retorna a linha evolutiva completa de um Pokémon. | `pokemon` (string), `fields` (array, opcional) | `Promise<Array>` (Linha Evolutiva) |
| `get_move` | Retorna dados detalhados sobre um movimento (ataque). | `move` (string), `fields` (array, opcional) | `Promise<Object>` (JSON do Movimento) |
| `get_nature` | Retorna os atributos afetados por uma Natureza. | `nature` (string), `fields` (array, opcional) | `Promise<Object>` (Atributos de Natureza) |
| `get_item` | Retorna dados detalhados sobre um item. | `item` (string), `fields` (array, opcional) | `Promise<Object>` (JSON do Item) |
| `get_generation` | Retorna dados sobre uma Geração específica. | `generation` (string/number), `fields` (array, opcional) | `Promise<Object>` (JSON da Geração) |
| `get_region` | Retorna dados sobre uma Região específica. | `region` (string), `fields` (array, opcional) | `Promise<Object>` (JSON da Região) |
| `get_all` | Retorna uma lista de todos os recursos de um tipo. | `type` (string: 'pokemon', 'type', 'ability', etc.) | `Promise<Array>` (Lista de Nomes) |

## 🔗 Recursos e Links

*   **NPM:** [https://www.npmjs.com/package/@lucasmod/pokemon.js] [3]
*   **GitHub (Original):** [https://github.com/musubi3/pokemon.js.git] [4]
*   **PokéAPI (Fonte de Dados):** [https://pokeapi.co/] [2]

---

### 🌟 Contribuição

Sinta-se à vontade para abrir *issues* ou enviar *pull requests* no repositório do GitHub para melhorias, correções de bugs ou novas funcionalidades.

### 📜 Licença

Este projeto está licenciado sob a Licença **MIT**.

---

## 📱 Conecte-se com o Autor

<div align="center">
  
  **lucasmod**
  
  <br>
  
  <!-- IMPORTANTE: Substitua os links e nomes de usuário pelos seus reais! -->
  
  [![Instagram](https://img.shields.io/badge/Instagram-@lucasmod-E4405F?style=flat&logo=instagram&logoColor=white)](https://instagram.com/lucas_mod_domina)
  [![YouTube](https://img.shields.io/badge/YouTube-Canal_Lucasmod-FF0000?style=flat&logo=youtube&logoColor=white)](https://youtube.com/@Otaku.mp4)
  [![GitHub](https://img.shields.io/badge/GitHub-lucasmod-181717?style=flat&logo=github&logoColor=white)](https://github.com/Otakump4)
  [![WhatsApp](https://img.shields.io/badge/WhatsApp-Contato-25D366?style=flat&logo=whatsapp&logoColor=white)](https://wa.me/559491569380)
  [![Telegram](https://img.shields.io/badge/Telegram-Contato-26A5E4?style=flat&logo=telegram&logoColor=white)](https://t.me/LUCAS_MOD_DOMINA)
  
</div>

[1]: https://www.npmjs.com/package/pokemon.js "Pacote Original pokemon.js"
[2]: https://pokeapi.co/ "PokéAPI - The Pokémon API"
[3]: https://www.npmjs.com/package/@lucasmod/pokemon.js "NPM - @lucasmod/pokemon.js"
[4]: https://github.com/musubi3/pokemon.js.git "GitHub - Repositório Original"
