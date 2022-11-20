---
title: Array.prototype.toSource()
slug: conflicting/Web/JavaScript/Reference/Global_Objects/Array/toString
tags:
  - Não-padrão
  - Referencia
  - prototipos
translation_of: Web/JavaScript/Reference/Global_Objects/Array/toSource
original_slug: Web/JavaScript/Reference/Global_Objects/Array/toSource
---
<div>{{JSRef}} {{non-standard_header}}</div>

<p>O método <code><strong>toSource()</strong></code> retorna uma representação string do código fonte do array.</p>

<h2 id="Sintaxe">Sintaxe</h2>

<pre class="syntaxbox"><code><var>arr</var>.toSource()</code></pre>

<h3 id="Parâmetros">Parâmetros</h3>

<p>Nenhum.</p>

<h2 id="Descrição">Descrição</h2>

<p>O método <code>toSource</code> retorna os seguintes valores:</p>

<ul>
 <li>Para o objeto {{jsxref("Array")}} pré-construido, <code>toSource</code> retorna a seguinte string indicando que o código fonte não está disponível:

  <pre class="brush: js">function Array() {
    [native code]
}
</pre>
 </li>
 <li>Para instancias de {{jsxref("Array")}}, <code>toSource</code> retorna uma representação string do código fonte.</li>
</ul>

<p>Este método normalmente é chamando internamente pelo JavaScript e não explicitamente no código. Você pode chamar <code>toSource</code> durante o debug para examinar o conteúdo de um array.</p>

<h2 id="Exemplos">Exemplos</h2>

<h3 id="Examinando_o_código_fonte_de_um_array">Examinando o código fonte de um array</h3>

<p>Para examinar o código fonte de um array:</p>

<pre class="brush: js">var alpha = new Array('a', 'b', 'c');

alpha.toSource();   //retorna ['a', 'b', 'c']
</pre>

<h2 id="Especificações">Especificações</h2>

<p>Não é parte de nenhum padrão. Implementado no JavaScript 1.3.</p>

<h2 id="Browser_compatibility">Compatibilidade com navegadores</h2>

<div>{{Compat}}</div>

<h2 id="Ver_também">Ver também</h2>

<ul>
 <li>{{jsxref("Object.prototype.toSource()")}}</li>
 <li>{{jsxref("Array.prototype.toString()")}}</li>
</ul>
