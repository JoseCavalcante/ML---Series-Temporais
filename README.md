# Modelos de Séries Temporais Em Python

<p><B>Modelos Paramétricos:</B> Domínio Temporal (número finito de parâmetros).</p>
<uo>
  <li>Modelos de erro (ou regressão).</li>
  <li>Modelos autorregressivos integrados e de médias móveis (ARIMA).</li>
  <li>Modelos de longas dependências temporais ou memória longa (ARFIMA)</li>
  <li>Modelos não lineares: autorregressivo com limiar (TAR), autorregressivo com transição suave (STAR), troca de regime markoviano (MSM) e redes neurais artificiais autorregressivas (AR-ANN).</li>  
</uo>
<BR>
<p><B>Modelos Não Paramétricos:</B> Domínio de frequências. Modelo de Análise espectral (decompõe a série em componentes de frequência).</p>
<uo>
  <li>Função de autocovariância e sua transformada de Fourier.</li>
</uo>
<BR>
<p><s>Modelo ARIMA</s></p>
<p>Autorregressivo (AR): indica que a variável é regressada em seus valores anteriores.</p>
<p>Integrado (I): indica que os valores de dados foram substituídos com a diferença entre seus valores e os valores anteriores (diferenciação).</p>
 <p>Média móvel (MA): Indica que o erro de regressão é uma combinação linear dos termos de erro dos valores passados.</p>
<BR>
<table>
  <tr>
    <td>
      <table>
        <tr>
          <td>Codificação: (p, d, q) Parâmetro d só pode ser inteiro</td>
        </tr>
        <tr>
          <td>p = ordem da autorregressão.</td>
        </tr>
        <tr>
          <td>d = grau de diferenciação.</td>
        </tr>
        <tr>
          <td>q = ordem da média móvel.</td>
        </tr>
    </td>
    <td>
      <table>
        <tr>
          <td>Modelo ARIMA: (2, 1, 1)</td>
          <td>Modelo AR: (1, 0, 0)</td>
          <td>Modelo MA (0, 0, 3)</td>
          <td>Modelo I: (0, 2, 0)</td>
          <td>Modelo ARMA: (4, 0, 1)</td>
        </tr>
      </table>
    </td>
  </tr>
</table>
<BR>
<p><s>Modelo ARFIMA</s></p>
<p>Autorregressivo (AR): indica que a variável é regressada em seus valores anteriores.</p>
<p>Fractional Integrado (FI)</p>
 <p>Média móvel (MA): Indica que o erro de regressão é uma combinação linear dos termos de erro dos valores passados.</p>
<BR>
<table>
  <tr>
    <td>
      <table>
        <tr>
          <td>Codificação: (p, d, q) Parâmetro d pode ser fracionário</td>
        </tr>
        <tr>
          <td>p = ordem da autorregressão.</td>
        </tr>
        <tr>
          <td>d = grau de diferenciação.</td>
        </tr>
        <tr>
          <td>q = ordem da média móvel.</td>
        </tr>
    </td>
    <td>
      <table>
        <tr>
          <td>Modelo ARIMA: (1, 1, 1)</td>
          <td>Modelo ARFIMA: (1, 0.25, 1)</td>
        </tr>
      </table>
    </td>
  </tr>
</table>
