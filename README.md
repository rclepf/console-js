# ⚡ JS Web & Terminal Sandbox

O **JS Web & Terminal Sandbox** é um ambiente de desenvolvimento estático e simplificado, projetado especificamente para fins didáticos. Seu objetivo principal é remover todas as barreiras técnicas iniciais (instalação de IDEs, NodeJS, configuração de terminal) para que o estudante foque exclusivamente no aprendizado da lógica de programação e manipulação web.

---

## 🎯 Proposta e Função Pedagógica

Aprender JavaScript pode ser confuso no início porque a linguagem opera em dois ecossistemas muito diferentes: o **Terminal** (lógica pura, scripts, backend) e a **Web** (manipulação visual, DOM, frontend). É comum que alunos iniciantes confundam onde cada código roda.

Este projeto resolve essa dor através de três pilares pedagógicos:

### 1. Separação Visual Conceitual
A interface divide as saídas de forma explícita:
* **O Painel do Console (Preto)** simula o comportamento de um terminal de comandos. O aluno entende o que é fluxo de dados, variáveis e lógica pura via `console.log`.
* **O Painel do Navegador (Branco)** renderiza o comportamento visual (DOM). O aluno vê em tempo real o impacto de alterar o HTML/CSS dinamicamente via JavaScript.

### 2. Ciclo de Feedback Instantâneo (Immediate Feedback Loop)
O erro faz parte do aprendizado. Ao clicar em "Executar", o aluno recebe o feedback visual ou a mensagem de erro imediatamente. Isso acelera a correção de rotas cognitivas e reduz a frustração de ter que salvar arquivos localmente e atualizar o navegador manualmente a cada alteração.

### 3. Ambiente Seguro contra Travamentos (Sandbox)
O código digitado é isolado por meio de um `<iframe>` seguro. Se o aluno escrever um loop infinito (`while(true)`) por engano, **apenas o painel de execução vai travar**, e não o navegador ou o editor de código. Ele pode simplesmente corrigir o código e clicar em executar novamente, sem perder o trabalho.

---

## 🛠️ Como Usar em Aula (Guia do Estudante)

O fluxo de trabalho foi desenhado para ser o mais intuitivo possível:

1. **Escrever ou Colar:** O estudante digita o seu código ou cola um trecho disponibilizado pelo professor no painel da esquerda.
2. **Executar (▶):** Ao clicar em "Executar", o código é processado na hora.
3. **Analisar as Saídas:** * Se o código tiver `console.log`, o resultado aparece no topo direito.
   * Se o código interagir com o HTML (ex: `document.body`), o resultado visual aparece no canto inferior direito.
4. **Baixar o Progresso (💾):** Ao final do exercício, o aluno clica em "Salvar .js" para descarregar o arquivo pronto diretamente no seu computador para entregar como tarefa.

---

## 🎓 Cenários Práticos de Aprendizado (Sugestões para o Professor)

Você pode guiar suas aulas utilizando a ferramenta para demonstrar a evolução do aprendizado:

### Aula 1: Lógica Pura (Modo Terminal)
Esqueça o HTML por enquanto. Peça para os alunos criarem algoritmos de tomada de decisão usando apenas o console.
```javascript
// Desafio: Verificar maioridade
let idade = 19;

if (idade >= 18) {
    console.log("Acesso permitido ao sistema.");
} else {
    console.log("Acesso negado.");
}
