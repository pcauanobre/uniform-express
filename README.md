(EN-US)
# UniformExpress – Uniform Customization System 

UniformExpress is a **single-page web application** that lets customers submit sports-uniform orders in just **3 quick steps**.  
Built with *HTML 5*, **Tailwind CSS**, and vanilla **JavaScript**, and powered by **Firebase Realtime Database**, it offers automatic saving, live collaboration, and direct sharing to WhatsApp.

![Welcome screen](https://github.com/user-attachments/assets/e8b182da-590d-4a5a-8d0c-15ca2b271612)

***

## 🛠 Technologies Used

- **HTML 5** + **Tailwind CSS** – responsive layout & utility classes  
- **JavaScript (ES Modules)** – front-end logic  
- **Firebase Realtime Database** – data storage & multi-user presence  
- **WhatsApp URL API** – one-click order submission  
- CSS keyframe animations & the `visualViewport` API for mobile UX

***

## 📦 Current Flow

| # | Screen | Function |
|---|--------|----------|
| 1 | **Welcome** | Introduces the app and asks the customer’s phone number |
| 2 | **Quantities by Size** | Inputs total pieces for each size (2 ANOS → XG3) |
| 3 | **Uniform Details** | Adds name, number, optional short & notes for every shirt |

**Screenshots**  
1. ![Welcome](https://github.com/user-attachments/assets/33ba38ac-a116-4e50-8123-6514e35bc13a)  
2. ![Step 2](https://github.com/user-attachments/assets/a6aa49c6-7748-49bc-b931-3382858c64ca)  
3. ![Step 3](https://github.com/user-attachments/assets/54755b54-41c6-49da-8003-72c4d22584b8)

### 1. Welcome

**Function:** Securely identify the order by phone number.  
**Details:** Rejects invalid numbers, loads existing orders or starts a new one, and offers a *“View Order”* read-only mode.

### 2. Quantities by Size

**Function:** Capture how many uniforms of each size are needed.  
**Process:** Plus/Minus buttons (0 ↔ 50), automatic clamping, keyboard-aware *Continue* button, instant presence lock if another user edits.

### 3. Uniform Details

**Function:** Fill personalisation for each uniform.  
**Highlights**

- Real-time **presence badge** (“Someone is here”) with dashed outline  
- **Auto-sequence labels** — *Uniform 01, 02…*  
- One-click **Add/Remove Short** & **Observation** blocks  
- **Filter bar** by size with live counter and smooth scrolling  
- **Auto-save badge** – shows **“✔ Saved automatically”** in 1.5 s

***

## ✨ Additional Features

| Feature | Description |
|---------|-------------|
| **Live Collaboration** | Edits are locked per card; colored outline + badge show who’s inside |
| **Delayed Auto-Save** | Saves to Firebase after 0.9 s idle (text) or instantly (clicks) |
| **WhatsApp Integration** | Generates clean text and opens WA with a pre-filled message |
| **Keyboard-Aware Buttons** | `makeKbAware()` keeps main buttons above the mobile keyboard |
| **View / Delete Order** | Read-only modal and full removal with confirmation |
| **Modal System** | Generic pop-ups for messages, confirmations, phone input, etc. |

***

## 📝 Final Notes

- Coordinates-free — the whole UI is **responsive** and resolution-independent.  
- Data is **device-agnostic**: open the same order on multiple screens to see real-time presence in action.  
- Created for internal use at **InterArt Uniformes**; feel free to fork, suggest improvements, or open a Pull Request.

---

(PT-BR)
# UniformExpress – Sistema de Personalização de Uniformes 

O **UniformExpress** é um aplicativo web *single-page* que permite ao cliente cadastrar pedidos de uniformes esportivos em apenas **3 passos**.  
Desenvolvido com *HTML 5*, **Tailwind CSS** e **JavaScript** puro, e utilizando **Firebase Realtime Database**, oferece salvamento automático, colaboração em tempo real e envio direto para o WhatsApp.

![Tela inicial](https://github.com/user-attachments/assets/e8b182da-590d-4a5a-8d0c-15ca2b271612)

***

## 🛠 Tecnologias Utilizadas

- **HTML 5** + **Tailwind CSS** – layout responsivo & utilitários  
- **JavaScript (ES Modules)** – lógica do front-end  
- **Firebase Realtime Database** – persistência de dados & presença multiusuário  
- **API de URL do WhatsApp** – envio do pedido em um clique  
- Animações CSS e API `visualViewport` para melhor UX no mobile

***

## 📦 Fluxo Atual

| # | Tela | Função |
|---|------|--------|
| 1 | **Bem-vindo** | Apresenta o app e solicita o telefone do responsável |
| 2 | **Quantidades por Tamanho** | Informa o total de peças por tamanho (2 ANOS → XG3) |
| 3 | **Informações dos Uniformes** | Nome, número, short opcional e observações para cada camisa |

**Imagens**  
1. ![Bem-vindo](https://github.com/user-attachments/assets/33ba38ac-a116-4e50-8123-6514e35bc13a)  
2. ![Passo 2](https://github.com/user-attachments/assets/a6aa49c6-7748-49bc-b931-3382858c64ca)  
3. ![Passo 3](https://github.com/user-attachments/assets/54755b54-41c6-49da-8003-72c4d22584b8)

### 1. Bem-vindo

**Função:** Identificar o pedido pelo telefone.  
**Detalhes:** Valida 11 dígitos, carrega pedidos existentes ou cria um novo, e oferece modo *“Ver Pedido”* (somente leitura).

### 2. Quantidades por Tamanho

**Função:** Registrar quantas peças de cada tamanho são necessárias.  
**Processo:** Botões +/− (0 ↔ 50), clamp automático, botão *Continuar* que flutua acima do teclado, bloqueio instantâneo se outro usuário editar.

### 3. Informações dos Uniformes

**Função:** Preencher personalização de cada uniforme.  
**Destaques**

- **Badge de presença** em tempo real (“Tem alguém aqui”) com contorno tracejado  
- **Rótulos automáticos** — *Uniforme 01, 02…*  
- Botões de **Adicionar/Remover Short** e **Obs.** em um clique  
- **Barra de filtro** por tamanho com contador dinâmico e rolagem suave  
- **Aviso de auto-salvo** – mostra **“✔ Salvo automaticamente”** em 1,5 s

***

## ✨ Recursos Adicionais

| Recurso | Descrição |
|---------|-----------|
| **Colaboração ao vivo** | Edição bloqueada por cartão; contorno colorido e badge indicam quem está dentro |
| **Auto-salvamento** | Grava no Firebase após 0,9 s inativo (texto) ou instantaneamente (cliques) |
| **Integração WhatsApp** | Gera texto limpo e abre o WhatsApp com a mensagem pronta |
| **Botões sensíveis ao teclado** | `makeKbAware()` mantém botões principais visíveis |
| **Ver / Excluir Pedido** | Modal somente leitura e remoção total com confirmação |
| **Sistema de Modais** | Pop-ups genéricos para mensagens, confirmações, telefone, etc. |

***

## 📝 Observações Finais

- Interface **100 % responsiva**, sem coordenadas fixas.  
- Dados são **sincronizados em tempo real** entre diversos dispositivos.  
- Projeto criado para uso interno na **InterArt Uniformes**; contribuições são bem-vindas via Issue ou Pull Request.
