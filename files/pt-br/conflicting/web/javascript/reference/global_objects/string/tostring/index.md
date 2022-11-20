---
title: String.prototype.toSource()
slug: conflicting/Web/JavaScript/Reference/Global_Objects/String/toString
tags:
  - JavaScript
  - Non-standard
  - Obsoleto
  - Prototipo
  - String
  - metodo
translation_of: Web/JavaScript/Reference/Global_Objects/String/toSource
original_slug: Web/JavaScript/Reference/Global_Objects/String/toSource
---
<div>{{JSRef}} {{obsolete_header}}</div>

<p>O método <code>toSource()</code> retorna uma string que representa o código-fonte do objeto.</p>

<h2 id="Sintaxe">Sintaxe</h2>

<pre class="syntaxbox notranslate"><code>String.toSource()
<var>str</var>.toSource()
</code></pre>

<h3 id="Valor_retornado">Valor retornado</h3>

<p>Uma string que representa o código-fonte do objeto chamado.</p>

<h2 id="Exemplos">Exemplos</h2>

<h3 id="Função_nativa">Função nativa</h3>

<p>Para o objeto {{jsxref("String")}} , <code>toSource()</code> retorna  a seguinte string (indicando que o código-fonte não está disponível):</p>

<pre class="brush: js notranslate">function String() {
    [native code]
}
</pre>

<p>Ao chamar {{jsxref("String")}} ou string literais, <code>toSource()</code> retorna a string que representa o código-fonte.</p>

<p>Esse método é usualmente invocado internamente pelo JavaScript e não explicitamente no código.</p>

<h2 id="Especificação">Especificação</h2>

<p>Não é parte de nenhum padrão.</p>

<h2 id="Navegadores_compatíveis">Navegadores compatíveis</h2>

<div>{{Compat}}</div>

<h2 id="Veja_também">Veja também</h2>

<ul>
 <li>{{jsxref("Object.prototype.toSource()")}}</li>
</ul>
