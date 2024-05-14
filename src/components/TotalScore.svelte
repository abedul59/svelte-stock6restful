
  
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
    <FONT SIZE="6">六大指標</FONT>
  </caption>
  <tr>
    <td style="background-color: #d3a4ff" align="center">
      <div><FONT SIZE="7">台股代號：</FONT></div>
    </td>
    <td align="center">
      <div>
        <FONT SIZE="7">{{ cStockID }}</FONT>
      </div>
    </td>
  </tr>

  <tr>
    <td style="background-color: #d3a4ff" align="center">
      <div><FONT SIZE="7">股票名稱：</FONT></div>
    </td>
    <td align="center">
      <div>
        <FONT SIZE="7">{{ cStockName }}</FONT>
      </div>
    </td>
  </tr>
  <tr>
    <td style="background-color: #d3a4ff" align="center">
      <div><FONT SIZE="7">最新營收月份：</FONT></div>
    </td>
    <td align="center">
      <div>
        <FONT SIZE="7">{{ cNewestRev }}</FONT>
      </div>
    </td>
  </tr>
  <tr>
    <td style="background-color: #d3a4ff" align="center">
      <div><FONT SIZE="7">最新財報季度：</FONT></div>
    </td>
    <td align="center">
      <div>
        <FONT SIZE="7">{{ cNewestSeason }}</FONT>
      </div>
    </td>
  </tr>

  <tr>
    <td style="background-color: #ffa6ff" align="center">
      <div><FONT SIZE="7">營收評等：</FONT></div>
    </td>
    <td align="center">
      <div>
        <FONT SIZE="7">{{ cSign1 }}</FONT>
      </div>
    </td>
  </tr>

  <tr>
    <td style="background-color: #ffa6ff" align="center">
      <div><FONT SIZE="7">營益率評等：</FONT></div>
    </td>
    <td align="center">
      <div>
        <FONT SIZE="7">{{ cSign2 }}</FONT>
      </div>
    </td>
  </tr>

  <tr>
    <td style="background-color: #ffa6ff" align="center">
      <div><FONT SIZE="7">稅後淨利評等：</FONT></div>
    </td>
    <td align="center">
      <div>
        <FONT SIZE="7">{{ cSign3 }}</FONT>
      </div>
    </td>
  </tr>

  <tr>
    <td style="background-color: #ffa6ff" align="center">
      <div><FONT SIZE="7">EPS評等：</FONT></div>
    </td>
    <td align="center">
      <div>
        <FONT SIZE="7">{{ cSign4 }}</FONT>
      </div>
    </td>
  </tr>

  <tr>
    <td style="background-color: #ffa6ff" align="center">
      <div><FONT SIZE="7">存貨週轉率評等：</FONT></div>
    </td>
    <td align="center">
      <div>
        <FONT SIZE="7">{{ cSign5 }}</FONT>
      </div>
    </td>
  </tr>

  <tr>
    <td style="background-color: #ffa6ff" align="center">
      <div><FONT SIZE="7">現金流量評等：</FONT></div>
    </td>
    <td align="center">
      <div>
        <FONT SIZE="7">{{ cSign6 }}</FONT>
      </div>
    </td>
  </tr>

  <tr>
    <td style="background-color: #ff2d2d" align="center">
      <div><FONT SIZE="7">總平均：</FONT></div>
    </td>
    <td align="center">
      <div>
        <FONT SIZE="7">{{ cAverageScore }}</FONT>
      </div>
    </td>
  </tr>
</table>

  