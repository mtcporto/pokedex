# Pokédex

## Visão Geral

Este projeto é uma aplicação web Pokédex que permite aos usuários navegar, pesquisar e ver informações detalhadas sobre Pokémon. Construído com JavaScript puro, HTML e CSS, a aplicação utiliza a [PokéAPI](https://pokeapi.co/) para buscar e exibir dados abrangentes sobre os Pokémon.

## Funcionalidades

- **Listagem de Pokémon**: Navegue por todos os Pokémon disponíveis com suporte à paginação
- **Busca**: Pesquise Pokémon por nome ou número de ID
- **Filtragem por Tipo**: Filtre Pokémon por seus tipos (Fogo, Água, Planta, etc.)
- **Informações Detalhadas**: Veja informações completas sobre cada Pokémon:
  - Estatísticas base com barras visuais
  - Efetividade de tipos e fraquezas
  - Atributos físicos (altura, peso)
  - Cadeia evolutiva
  - Habilidades com descrições detalhadas
  - Classificação e informações de habitat

- **Otimizações de Desempenho**:
  - Carregamento lazy de imagens
  - Carregamento progressivo de dados (carrega dados essenciais primeiro)
  - Cache em armazenamento local para reduzir chamadas à API
  - Armazenamento em chunks para lidar com grandes conjuntos de dados

- **Design Responsivo**: Layout totalmente responsivo que funciona em dispositivos desktop e móveis

## Tecnologias Utilizadas

- **HTML5**: Estrutura e marcação semântica
- **CSS3**: Estilização com recursos como:
  - Layouts Flexbox e Grid
  - Variáveis CSS para tematização
  - Animações e transições
  - Media queries para design responsivo
- **JavaScript Puro**: Sem frameworks, apenas JavaScript com:
  - Recursos modernos ES6+
  - Promises e async/await para chamadas à API
  - Manipulação do DOM
  - Tratamento de eventos
  - API LocalStorage para cache

- **APIs Externas**:
  - [PokéAPI](https://pokeapi.co/) para todos os dados de Pokémon
  - Google Fonts para tipografia

## Estrutura do Projeto

O projeto consiste em duas páginas principais:

1. **index.html**: A página principal de listagem que exibe todos os Pokémon em um grid de cards com opções de filtragem
2. **pokemon-detail.html**: Página de visualização detalhada para Pokémon individuais com informações abrangentes

## Considerações de Desempenho

- **Carregamento Otimizado**: A aplicação inicialmente carrega apenas o primeiro lote de Pokémon para exibição imediata, então busca dados adicionais em segundo plano
- **Estratégia de Cache**: Implementa um sistema sofisticado de cache usando LocalStorage para armazenar dados de Pokémon por 24 horas, reduzindo chamadas à API
- **Armazenamento Mínimo de Dados**: Armazena apenas dados essenciais para evitar exceder limites de armazenamento do navegador
- **Localização**: Tenta exibir informações de Pokémon em português quando disponíveis, com inglês como alternativa

## Suporte a Navegadores

A aplicação utiliza recursos modernos de JavaScript e foi projetada para funcionar nas versões atuais dos principais navegadores, incluindo Chrome, Firefox, Safari e Edge.

## Como Começar

Basta abrir o arquivo index.html em um navegador web para começar a explorar a Pokédex. Não é necessário processo de build ou configuração de servidor.