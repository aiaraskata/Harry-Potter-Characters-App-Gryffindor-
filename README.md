# Harry Potter Characters App (Gryffindor) / App de Personagens de Harry Potter (Gryffindor)

> **Languages / Idiomas:** [Português](#português) | [English](#english)

---

<a name="português"></a>
## 🇧🇷 Português

### 📝 Descrição do Projeto
Este projeto é um aplicativo iOS desenvolvido em **SwiftUI** utilizando a arquitetura **MVVM** (Model-View-ViewModel) e o framework **Combine**. O app realiza requisições assíncronas a uma API REST externa ([HP-API](https://hp-api.onrender.com/)) para buscar e exibir informações detalhadas dos personagens da casa **Gryffindor** (Grifinória) do universo de Harry Potter.

#### Principais Funcionalidades:
- **Consumo de API REST Assíncrono:** Utiliza `URLSession.shared.dataTaskPublisher` e `Combine` para consumir dados JSON diretamente da API.
- **Listagem de Personagens (`PrimeiraTela`):** Exibe uma lista com as fotos dos personagens (carregadas via `AsyncImage`) e seus respectivos nomes sobre um fundo temático na cor vinho (`wine`).
- **Navegação Hierárquica (`NavigationStack`):** Permite selecionar qualquer personagem para ver suas informações detalhadas.
- **Tela de Detalhes (`SegundaTela`):** Apresenta o retrato do personagem selecionado com efeito circular e cartão com informações adicionais:
  - Casa (`House`)
  - Nome completo (`Name`)
  - Data de nascimento (`Birth`)
  - Cor dos olhos (`Eyes`)
  - Fundo desfocado com o logotipo do universo bruxo.

---

### 🛠️ Tecnologias Utilizadas
- **Linguagem:** Swift
- **Frameworks:** SwiftUI, Combine (`ObservableObject`, `@Published`, `AnyCancellable`)
- **Arquitetura:** MVVM (Model - View - ViewModel)
- **Networking:** `URLSession` / Data Task Publisher
- **API Utilizada:** [HP-API (Gryffindor Characters)](https://hp-api.onrender.com/api/characters/house/gryffindor)
- **IDE:** Xcode
- **Plataforma Target:** iOS / iPadOS

---

### 🚀 Como Executar o Projeto

#### Pré-requisitos
* Um computador Mac executando **macOS**.
* **Xcode 14** ou superior instalado.
* Conexão com a **internet** ativa (necessária para realizar a requisição HTTP e carregar as imagens).

#### Passo a Passo
1. **Clonar ou Baixar o Repositório:**
   ```bash
   git clone <URL_DO_REPOSITORIO>
   ```
2. **Abrir o Projeto no Xcode:**
   * Navegue até a pasta do projeto.
   * Dê um duplo clique no arquivo `.xcodeproj` (ex: `Desafio7 - 03-06.xcodeproj`).
3. **Verificar Assets / Ativos:**
   * Verifique se a cor personalizada `wine` e a imagem `logo` estão devidamente cadastradas no `Assets.xcassets`.
4. **Executar no Simulador:**
   * Escolha o simulador desejado na barra superior do Xcode (ex: *iPhone 15*).
   * Pressione `Cmd + R` ou clique no botão **Play (▶)** para compilar e rodar a aplicação.

---

<a name="english"></a>
## 🇬🇧 English

### 📝 Project Description
This is an iOS application built with **SwiftUI** adopting the **MVVM** design pattern and the **Combine** framework. The app fetches and displays character data from the **Gryffindor** house in the Harry Potter universe by consuming the public [HP-API](https://hp-api.onrender.com/).

#### Key Features:
- **Asynchronous REST API Consumption:** Leverages `URLSession.shared.dataTaskPublisher` combined with `Combine` reactive streams to parse remote JSON data into model objects.
- **Character List (`PrimeiraTela`):** Renders a scrollable list featuring character avatars (`AsyncImage`) and names styled over a themed wine-colored background.
- **Hierarchical Navigation (`NavigationStack`):** Tapping a character item pushes the view hierarchy to a detailed summary card.
- **Detail Screen (`SegundaTela`):** Displays a high-resolution circular portrait alongside character information:
  - House
  - Full Name
  - Date of Birth
  - Eye Color
  - Blurred background overlay with the wizarding world logo.

---

### 🛠️ Tech Stack
- **Language:** Swift
- **Frameworks:** SwiftUI, Combine (`ObservableObject`, `@Published`, `AnyCancellable`)
- **Architecture Pattern:** MVVM (Model - View - ViewModel)
- **Networking:** `URLSession` / Data Task Publisher
- **API:** [HP-API (Gryffindor Endpoint)](https://hp-api.onrender.com/api/characters/house/gryffindor)
- **IDE:** Xcode
- **Target Platform:** iOS / iPadOS

---

### 🚀 How to Run the Project

#### Prerequisites
* A Mac computer running **macOS**.
* **Xcode 14** or higher installed.
* An active **internet connection** (required for API requests and fetching remote image assets).

#### Step-by-Step
1. **Clone or Download the Repository:**
   ```bash
   git clone <REPOSITORY_URL>
   ```
2. **Open the Project in Xcode:**
   * Navigate to the project directory.
   * Double-click the `.xcodeproj` file (e.g., `Desafio7 - 03-06.xcodeproj`).
3. **Check Asset Catalog:**
   * Ensure that the `wine` custom color and `logo` image asset exist in `Assets.xcassets`.
4. **Run in Simulator:**
   * Select your target iOS Simulator from the Xcode top bar (e.g., *iPhone 15*).
   * Press `Cmd + R` or click the **Play (▶)** button to build and launch the app.
