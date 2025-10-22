# 🎧 Projeto Spotify Imersão — Alura Front-End

Este projeto foi desenvolvido como parte da **Imersão Front-End da Alura**, e consiste em uma **simulação da interface do Spotify**, criada para praticar conceitos de **HTML, CSS e JavaScript**.  

A aplicação inclui uma **página principal com navegação**, **seção de playlists** e **funcionalidade de busca por artistas**, utilizando dados **mockados** armazenados em um **arquivo JSON local** que simula uma API.

---

## 📋 Visão Geral

O projeto apresenta:

- Uma **interface web inspirada no Spotify**, com *sidebar*, *header* de navegação, seções de playlists e rodapé.  
- Uma **API simulada (mockada)** usando **JSON Server** para fornecer dados de artistas.  
- Uma **busca em tempo real** que filtra artistas com base no termo digitado.

---

## ⚙️ Pré-requisitos

Antes de começar, certifique-se de ter instalado:

- **Node.js** (versão 14 ou superior)  
- **npm** (gerenciador de pacotes do Node.js)  
- Um **navegador web moderno**

---

## 🚀 Instalação

1. **Clone ou baixe** o repositório do projeto (supondo que os arquivos estejam em uma pasta local).

2. **Instale o JSON Server** na versão específica (necessária para o funcionamento da busca):

   ```
   npm install -g json-server@0.17.4
   ```
⚠️ Importante:
A partir da versão 1.0.0 do JSON Server, o operador de busca name_like foi descontinuado.
Por isso, é necessário usar a versão 0.17.4 para garantir o funcionamento correto da pesquisa.

---

## ▶️ Como Rodar o Projeto

**Acesse a pasta da API:**

Antes de iniciar o servidor, certifique-se de estar dentro da pasta api-artists, onde está o arquivo artists.json.
```
cd api-artists
```
**Inicie o servidor JSON:**

Execute o comando:
```
json-server --watch artists.json --port 3000
```
Isso iniciará o servidor na porta 3000, servindo os dados mockados dos artistas.

Abra a página web:

Volte para a pasta principal do projeto, se necessário.

Abra o arquivo index.html em um navegador.

A interface do Spotify será carregada.

Teste a busca:

No campo de busca ("O que você quer ouvir?"), digite o nome de um artista, por exemplo:
```
Foo Fighters
```

A página alternará entre a seção de playlists e os resultados da busca, exibindo o artista correspondente com imagem e nome.

---

## 🧱 Estrutura do Projeto


```
📁 projeto-spotify-imersao/

│

├── 📁 api-artists/

│   └── artists.json          # Dados mockados dos artistas (id, nome, gênero, imagem)

│

├── index.html                # Estrutura principal da página

├── script.js                 # Lógica da busca e manipulação da interface

│

└── src/

    ├── css/
    
    │   ├── reset.css

    │   ├── vars.css

    │   └── style.css

    └── assets/

        ├── icons/
        
        └── playlists/
  ```

  ---
        
        
## ✨ Funcionalidades

🎵 Navegação: Sidebar com links para "Início" e "Buscar", além de biblioteca e playlists.

🎧 Playlists: Lista horizontal de cards com gêneros como Rock, Hip Hop, Sertanejo, etc.

🔍 Busca de Artistas: Campo de pesquisa que consulta a API mockada em tempo real.

📱 Responsividade: Interface adaptável a diferentes tamanhos de tela (com media queries).

---

## 🧠 Conclusão
Este projeto foi desenvolvido como parte da Imersão Front-End da Alura, e serve como base para aprender sobre:

Estrutura e semântica do HTML

Estilização moderna com CSS

Manipulação do DOM e consumo de APIs com JavaScript

🎓 Um ótimo exercício para praticar conceitos de desenvolvimento web moderno com um projeto realista e divertido!

Copiar código
