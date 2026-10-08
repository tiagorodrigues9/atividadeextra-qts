# Técnicas de Inspeção de Acessibilidade no Navegador

Este repositório apresenta uma atividade voltada à análise manual de requisitos não funcionais relacionados à acessibilidade e aos aspectos visuais de uma aplicação web. A avaliação utiliza como referência as diretrizes **WCAG 2.1 (Nível AA)** e a norma **ISO/IEC 25010**.

## Estrutura do Projeto

* `painel-campanha.html` — Página web desenvolvida para a atividade, contendo propositalmente problemas de acessibilidade que serão identificados durante o processo de inspeção.

## Procedimentos de Auditoria Visual (DevTools)

Durante a atividade, foram realizadas diferentes verificações utilizando as ferramentas de desenvolvimento do navegador. As evidências obtidas por meio de capturas de tela contemplam os seguintes testes:

1. **Simulação de Condições Visuais:**

   * Uso do recurso *Rendering* (`More tools > Rendering > Emulate vision deficiencies`) para reproduzir diferentes condições de visão, incluindo *Protanopia* e *Blurred vision*.

2. **Verificação do Contraste dos Elementos:**

   * Análise das cores utilizando o *Color Picker* disponível no DevTools, verificando se os textos atendem ao contraste mínimo de `4.5 : 1` estabelecido pelo Critério 1.4.3 da WCAG 2.1 em nível AA.

3. **Análise da Navegação por Teclado:**

   * Avaliação da sequência de foco utilizando a tecla `Tab`, identificando possíveis problemas causados pela utilização inadequada de valores positivos no atributo `tabindex` e pela falta de um indicador visual apropriado através de `:focus-visible`.
