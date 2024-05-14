
  
<script>
export let cStockID,cStockName,cNewestRev,cNewestSeason,cSign1,cSign2,cSign3,cSign4,cSign5,cSign6,cAverageScore
</script>

  <style>
  h3 {
    margin: 40px 0 0;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }
  li {
    display: inline-block;
    margin: 0 10px;
  }
  a {
    color: #42b983;
  }
  </style>



<div v-if="cStockName"></div>
<table
  border="2"
  cellpadding="1"
  cellspacing="5"
  style="border: 1px solid black; margin-left: auto; margin-right: auto"
>
  <caption>
    六大指標
  </caption>
  <tr>
    <td style="background-color: #d3a4ff" align="center">
      <div>台股代號：</div>
    </td>
    <td align="center">
      <div>
        { cStockID }
      </div>
    </td>
  </tr>

  <tr>
    <td style="background-color: #d3a4ff" align="center">
      <div>股票名稱：</div>
    </td>
    <td align="center">
      <div>
        { cStockName }
      </div>
    </td>
  </tr>
  <tr>
    <td style="background-color: #d3a4ff" align="center">
      <div>最新營收月份：</div>
    </td>
    <td align="center">
      <div>
        { cNewestRev }
      </div>
    </td>
  </tr>
  <tr>
    <td style="background-color: #d3a4ff" align="center">
      <div>最新財報季度：</div>
    </td>
    <td align="center">
      <div>
        { cNewestSeason }
      </div>
    </td>
  </tr>

  <tr>
    <td style="background-color: #ffa6ff" align="center">
      <div>營收評等：</div>
    </td>
    <td align="center">
      <div>
        { cSign1 }
      </div>
    </td>
  </tr>

  <tr>
    <td style="background-color: #ffa6ff" align="center">
      <div>營益率評等：</div>
    </td>
    <td align="center">
      <div>
        { cSign2 }
      </div>
    </td>
  </tr>

  <tr>
    <td style="background-color: #ffa6ff" align="center">
      <div>稅後淨利評等：/div>
    </td>
    <td align="center">
      <div>
        { cSign3 }
      </div>
    </td>
  </tr>

  <tr>
    <td style="background-color: #ffa6ff" align="center">
      <div>EPS評等：</div>
    </td>
    <td align="center">
      <div>
        { cSign4 }
      </div>
    </td>
  </tr>

  <tr>
    <td style="background-color: #ffa6ff" align="center">
      <div>存貨週轉率評等：</div>
    </td>
    <td align="center">
      <div>
        { cSign5 }
      </div>
    </td>
  </tr>

  <tr>
    <td style="background-color: #ffa6ff" align="center">
      <div>現金流量評等：</div>
    </td>
    <td align="center">
      <div>
        { cSign6 }
      </div>
    </td>
  </tr>

  <tr>
    <td style="background-color: #ff2d2d" align="center">
      <div>總平均：</div>
    </td>
    <td align="center">
      <div>
        { cAverageScore }
      </div>
    </td>
  </tr>
</table>

  