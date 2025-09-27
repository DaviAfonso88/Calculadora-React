# 🧮 Calculadora em React

Este projeto é uma **calculadora funcional** desenvolvida em **React**, criada para consolidar conceitos estudados como **componentização**, **props**, **estado**, **eventos** e **estilização modularizada**.
A aplicação segue a lógica de uma calculadora básica, permitindo realizar operações matemáticas simples de forma clara e organizada.

---

## 🚀 Tecnologias utilizadas

* [React](https://react.dev/) (componentes funcionais e de classe)
* JavaScript (ES6+)
* CSS3 com variáveis customizadas
* Fonte [Roboto Mono](https://fonts.google.com/specimen/Roboto+Mono)

---

## 📂 Estrutura do projeto

```
src/
├── components/
│   ├── Button.css       # Estilos dos botões
│   ├── Button.jsx       # Componente de botão reutilizável
│   ├── Display.css      # Estilos do display
│   └── Display.jsx      # Componente que exibe os valores
│
├── fonts/
│   └── RobotoMono-Thin.ttf  # Fonte customizada
│
├── main/
│   ├── Calculator.css   # Estilos da calculadora
│   └── Calculator.jsx   # Componente principal com toda a lógica
│
├── App.js               # Estrutura base do projeto
├── index.js             # Ponto de entrada da aplicação
└── index.css            # Estilos globais (fonte e layout)
```

---

## 🎯 Funcionalidades

✔️ Interface com **botões reutilizáveis**
✔️ **Display dinâmico** que mostra números e resultados
✔️ Operações: **adição, subtração, multiplicação e divisão**
✔️ Botão **AC** (limpar memória)
✔️ Suporte a números decimais com `.`
✔️ Layout responsivo baseado em **CSS Grid**
✔️ Uso de **props** para comunicação entre componentes
✔️ Estado controlado no componente principal (`Calculator`)

---

## 🔎 Detalhes dos componentes

### 🔘 Button

* Recebe `props.label` para definir o texto do botão.
* Pode ter variações de estilo:

  * `operation` → botões de operações (+, -, *, /, =)
  * `double` e `triple` → botões que ocupam mais espaço no grid
* Dispara uma função `props.click` ao ser clicado, enviando o valor do botão.

### 🖥️ Display

* Componente simples que recebe `props.value` e exibe no display da calculadora.

### 🧮 Calculator

* Componente **de classe** que contém toda a lógica da calculadora.
* Gerencia o **estado interno**:

  ```js
  const initialState = {
    displayValue: "0",
    clearDisplay: false,
    operation: null,
    values: [0, 0],
    current: 0
  };
  ```
* Principais métodos:

  * `clearMemory()` → limpa o estado.
  * `setOperation(op)` → define ou executa a operação matemática.
  * `addDigit(n)` → insere números e trata ponto decimal.

---

## ⚙️ Como executar o projeto

1. Clone este repositório:

   ```bash
   git clone https://github.com/seu-usuario/calculadora-react.git
   ```

2. Acesse a pasta:

   ```bash
   cd calculadora-react
   ```

3. Instale as dependências:

   ```bash
   npm install
   ```

4. Execute o projeto:

   ```bash
   npm start
   ```

5. Acesse no navegador:

   ```
   http://localhost:3000
   ```

---

## 📖 O que foi aprendido

* Criação e organização de componentes em React.
* Diferença entre **componentes funcionais** e **de classe**.
* Uso de **props** para reutilização de componentes.
* Controle de **estado** com arrays e objetos.
* Estilização usando **CSS Grid** e variáveis CSS.
* Importação de fontes customizadas e aplicação global no projeto.

---

## ✨ Demonstração

*(adicione prints ou um GIF do projeto rodando aqui)*

---

## 📜 Licença

Este projeto é de uso livre para fins de estudo.
