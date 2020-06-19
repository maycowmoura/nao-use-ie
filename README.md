# Não use Internet Explorer!
Página de aviso para o usuário deixar o Internet Explorer e baixar outro navegador.

Basta inserir a linha abaixo dentro do seu `index.html`.
De preferência insira antes dos demais scripts e dentro de sua tag `<script>` especifica, pois se o restante do código javascript quebrar, o IE pode não executar essa linha.
  
```
<script type="application/javascript">
  if (/MSIE|Trident/.test(window.navigator.userAgent)) window.location.href = '/ie.html';
</script>
```
  
Usei imagens em base64 e CSS dentro da tag `<style>` pois a intenção é ter um único arquivo `ie.html`, sem dependências e sem alteração desnecessária no código original. Mas podem ser facilmente re-convertidas em sites de "base64 to image".

####Demo

[Redirecionador](https://maycowmoura.github.io/nao-use-ie/) (acesse usando o Internet Explorer)

[Página de Aviso](https://maycowmoura.github.io/nao-use-ie/ie.html)
