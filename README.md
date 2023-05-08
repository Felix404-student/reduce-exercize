# reduce-exercize
reduce practice lesson for UMass/Springboard bootcamp

Written in Javascript and HTML

<div class="section" id="extractvalue">
<h3>extractValue</h3>
<p>Write a function called extractValue which accepts an array of objects and a key and returns a new array with the value of each object at the key.</p>
<div class="highlight-js notranslate"><div class="highlight"><pre><span></span><span class="kr">const</span> <span class="nx">arr</span> <span class="o">=</span> <span class="p">[{</span><span class="nx">name</span><span class="o">:</span> <span class="s1">&#39;Elie&#39;</span><span class="p">},</span> <span class="p">{</span><span class="nx">name</span><span class="o">:</span> <span class="s1">&#39;Tim&#39;</span><span class="p">},</span> <span class="p">{</span><span class="nx">name</span><span class="o">:</span> <span class="s1">&#39;Matt&#39;</span><span class="p">},</span> <span class="p">{</span><span class="nx">name</span><span class="o">:</span> <span class="s1">&#39;Colt&#39;</span><span class="p">}]</span>
<span class="nx">extractValue</span><span class="p">(</span><span class="nx">arr</span><span class="p">,</span><span class="s1">&#39;name&#39;</span><span class="p">)</span> <span class="c1">// [&#39;Elie&#39;, &#39;Tim&#39;, &#39;Matt&#39;, &#39;Colt&#39;]</span>
</pre></div>
</div>
</div>
<div class="section" id="vowelcount">
<h3>vowelCount</h3>
<p>Write a function called vowelCount which accepts a string and returns an object with the keys as the vowel and the values as the number of times the vowel appears in the string. This function should be case insensitive so a lowercase letter and uppercase letter should count</p>
<div class="highlight-js notranslate"><div class="highlight"><pre><span></span><span class="nx">vowelCount</span><span class="p">(</span><span class="s1">&#39;Elie&#39;</span><span class="p">)</span> <span class="c1">// {e:2,i:1};</span>
<span class="nx">vowelCount</span><span class="p">(</span><span class="s1">&#39;Tim&#39;</span><span class="p">)</span> <span class="c1">// {i:1};</span>
<span class="nx">vowelCount</span><span class="p">(</span><span class="s1">&#39;Matt&#39;</span><span class="p">)</span> <span class="c1">// {a:1})</span>
<span class="nx">vowelCount</span><span class="p">(</span><span class="s1">&#39;hmmm&#39;</span><span class="p">)</span> <span class="c1">// {};</span>
<span class="nx">vowelCount</span><span class="p">(</span><span class="s1">&#39;I Am awesome and so are you&#39;</span><span class="p">)</span> <span class="c1">// {i: 1, a: 4, e: 3, o: 3, u: 1};</span>
</pre></div>
</div>
</div>
<div class="section" id="addkeyandvalue">
<h3>addKeyAndValue</h3>
<p>Write a function called addKeyAndValue which accepts an array of objects and returns the array of objects passed to it with each object now including the key and value passed to the function.</p>
<div class="highlight-js notranslate"><div class="highlight"><pre><span></span><span class="kr">const</span> <span class="nx">arr</span> <span class="o">=</span> <span class="p">[{</span><span class="nx">name</span><span class="o">:</span> <span class="s1">&#39;Elie&#39;</span><span class="p">},</span> <span class="p">{</span><span class="nx">name</span><span class="o">:</span> <span class="s1">&#39;Tim&#39;</span><span class="p">},</span> <span class="p">{</span><span class="nx">name</span><span class="o">:</span> <span class="s1">&#39;Matt&#39;</span><span class="p">},</span> <span class="p">{</span><span class="nx">name</span><span class="o">:</span> <span class="s1">&#39;Colt&#39;</span><span class="p">}];</span>

<span class="nx">addKeyAndValue</span><span class="p">(</span><span class="nx">arr</span><span class="p">,</span> <span class="s1">&#39;title&#39;</span><span class="p">,</span> <span class="s1">&#39;Instructor&#39;</span><span class="p">)</span> <span class="c1">//</span>

<span class="p">[</span>
  <span class="p">{</span><span class="nx">title</span><span class="o">:</span> <span class="s1">&#39;Instructor&#39;</span><span class="p">,</span> <span class="nx">name</span><span class="o">:</span> <span class="s1">&#39;Elie&#39;</span><span class="p">},</span>
  <span class="p">{</span><span class="nx">title</span><span class="o">:</span> <span class="s1">&#39;Instructor&#39;</span><span class="p">,</span> <span class="nx">name</span><span class="o">:</span> <span class="s1">&#39;Tim&#39;</span><span class="p">},</span>
  <span class="p">{</span><span class="nx">title</span><span class="o">:</span> <span class="s1">&#39;Instructor&#39;</span><span class="p">,</span> <span class="nx">name</span><span class="o">:</span> <span class="s1">&#39;Matt&#39;</span><span class="p">},</span>
  <span class="p">{</span><span class="nx">title</span><span class="o">:</span> <span class="s1">&#39;Instructor&#39;</span><span class="p">,</span> <span class="nx">name</span><span class="o">:</span> <span class="s1">&#39;Colt&#39;</span><span class="p">}</span>
<span class="p">]</span>
</pre></div>
</div>
</div>
<div class="section" id="partition">
<h3>partition</h3>
<p>Write a function called partition which accepts an array and a callback and returns an array with two arrays inside of it. The partition function should run the callback function on each value in the array and if the result of the callback function at that specific value is true, the value should be placed in the first subarray. If the result of the callback function at that specific value is false, the value should be placed in the second subarray.</p>
<div class="highlight-js notranslate"><div class="highlight"><pre><span></span><span class="kd">function</span> <span class="nx">isEven</span><span class="p">(</span><span class="nx">val</span><span class="p">){</span>
  <span class="k">return</span> <span class="nx">val</span> <span class="o">%</span> <span class="mi">2</span> <span class="o">===</span> <span class="mi">0</span><span class="p">;</span>
<span class="p">}</span>

<span class="kr">const</span> <span class="nx">arr</span> <span class="o">=</span> <span class="p">[</span><span class="mi">1</span><span class="p">,</span><span class="mi">2</span><span class="p">,</span><span class="mi">3</span><span class="p">,</span><span class="mi">4</span><span class="p">,</span><span class="mi">5</span><span class="p">,</span><span class="mi">6</span><span class="p">,</span><span class="mi">7</span><span class="p">,</span><span class="mi">8</span><span class="p">];</span>

<span class="nx">partition</span><span class="p">(</span><span class="nx">arr</span><span class="p">,</span> <span class="nx">isEven</span><span class="p">)</span> <span class="c1">// [[2,4,6,8], [1,3,5,7]];</span>

<span class="kd">function</span> <span class="nx">isLongerThanThreeCharacters</span><span class="p">(</span><span class="nx">val</span><span class="p">){</span>
  <span class="k">return</span> <span class="nx">val</span><span class="p">.</span><span class="nx">length</span> <span class="o">&gt;</span> <span class="mi">3</span><span class="p">;</span>
<span class="p">}</span>

<span class="kr">const</span> <span class="nx">names</span> <span class="o">=</span> <span class="p">[</span><span class="s1">&#39;Elie&#39;</span><span class="p">,</span> <span class="s1">&#39;Colt&#39;</span><span class="p">,</span> <span class="s1">&#39;Tim&#39;</span><span class="p">,</span> <span class="s1">&#39;Matt&#39;</span><span class="p">];</span>

<span class="nx">partition</span><span class="p">(</span><span class="nx">names</span><span class="p">,</span> <span class="nx">isLongerThanThreeCharacters</span><span class="p">)</span> <span class="c1">// [[&#39;Elie&#39;, &#39;Colt&#39;, &#39;Matt&#39;], [&#39;Tim&#39;]]</span>
</pre></div>
</div>
