Vou adicionar as referencias da DOM do GPU para executar a compra dos presos com o assistente de lançamento. 

1 - fazer login no GPU (copiar do PIX Selenium)
2 - clicar em cadastrar compras - xPATH: /html/body/div/div[3]/div[1]/ul/li[5]/form/button/span/p
3 - clicar em 'NÃO' (deseja encerrar a compra?) - xPath: /html/body/div/div[3]/div[2]/div[1]/div/form/div/div/input[2]
4 - Iniciar o loop de cadastro de compra:
- verificar a sequencia da folha de compra, pegando a matricula que esta no pdf da folha de compra 
- adicionar a matricula no input: xPATH: /html/body/div/div[3]/div[2]/div[1]/div/div[2]/div/form/table[1]/tbody/tr[1]/td/input
- pressionar 'enter' para carregar as informações do preso na tela e computar a sua compra.
aparecerá nessa div: <div id="resultadoBusca" bis_skin_checked="1">&nbsp;</div>
o saldo das comrpas parcial aparecerá nessa tabela:
                     <td style="font-size: 10pt;">
                        <span>Total Compras:</span>
                        <span name="total_compra" id="total_compra"></span>
                        <input size="8" type="hidden" onkeypress="event.returnValue=&quot;false&quot;" name="totalcompra">
                    </td>
- de forma assistida ajudar no preenchimento dos pedidos de compras de cada item da tabela:
<table style="width: 100%; border: 0; text-align: center; font-family:Arial, Helvetica, sans-serif;">
                <tbody><tr style="text-align: center;">
                    <td style="text-align: right;">
                        <b> Produto </b>
                    </td>
                    <td>
                        <b>Qtde</b>
                    </td>
                    <td>
                        <b>Limite</b>
                    </td>
                    <td>
                        <b>Preço</b>
                    </td>
                    <td>
                        <b>Subtotal</b>
                    </td>
                </tr>
                
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            137451 -  ACHOCOLATADO MUKY 400 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_1" onchange="subtot(document.formCompra.qtde_1,formCompra.preco_1,formCompra.limite_1,formCompra.subtotal_1,document.getElementById('subtotald_1'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_1" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_1" size="4" value="7.50">
                            R$ 7.50                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_1" id="subtotald_1" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_1" name="subtotal_1" size="4">
                        </td>

                        <input type="hidden" name="codfor_1" id="987" value="987">
                        <input type="hidden" name="codP_id1" id="2003" value="2003">
                        <input type="hidden" name="prodNomeSimples1" id="ACHOCOLATADO" value="ACHOCOLATADO">
                        <input type="hidden" name="pro_percaptamaxima1" id="400" value="400">
                        <input type="hidden" name="pro_percaptamaximaSap1" id="800" value="800">
                        <input type="hidden" name="uni_nome1" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd1" id="400" value="400">
                        <input type="hidden" name="cod_1" id="137451" value="137451">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            130524 -  ADOCANTE ADOCYL 100 MILILITRO                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_2" onchange="subtot(document.formCompra.qtde_2,formCompra.preco_2,formCompra.limite_2,formCompra.subtotal_2,document.getElementById('subtotald_2'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_2" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_2" size="4" value="4.95">
                            R$ 4.95                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_2" id="subtotald_2" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_2" name="subtotal_2" size="4">
                        </td>

                        <input type="hidden" name="codfor_2" id="1232" value="1232">
                        <input type="hidden" name="codP_id2" id="2006" value="2006">
                        <input type="hidden" name="prodNomeSimples2" id="ADOCANTE" value="ADOCANTE">
                        <input type="hidden" name="pro_percaptamaxima2" id="100" value="100">
                        <input type="hidden" name="pro_percaptamaximaSap2" id="100" value="100">
                        <input type="hidden" name="uni_nome2" id="MILILITRO" value="MILILITRO">
                        <input type="hidden" name="proUniQtd2" id="100" value="100">
                        <input type="hidden" name="cod_2" id="130524" value="130524">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            103703 -  AGUA SANITARIA  1000 MILILITRO                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_3" onchange="subtot(document.formCompra.qtde_3,formCompra.preco_3,formCompra.limite_3,formCompra.subtotal_3,document.getElementById('subtotald_3'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_3" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_3" size="4" value="2.38">
                            R$ 2.38                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_3" id="subtotald_3" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_3" name="subtotal_3" size="4">
                        </td>

                        <input type="hidden" name="codfor_3" id="2737" value="2737">
                        <input type="hidden" name="codP_id3" id="2011" value="2011">
                        <input type="hidden" name="prodNomeSimples3" id="AGUA SANITARIA" value="AGUA SANITARIA">
                        <input type="hidden" name="pro_percaptamaxima3" id="2000" value="2000">
                        <input type="hidden" name="pro_percaptamaximaSap3" id="2000" value="2000">
                        <input type="hidden" name="uni_nome3" id="MILILITRO" value="MILILITRO">
                        <input type="hidden" name="proUniQtd3" id="1000" value="1000">
                        <input type="hidden" name="cod_3" id="103703" value="103703">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            137450 -  AGULHA DE COSTURA  1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_4" onchange="subtot(document.formCompra.qtde_4,formCompra.preco_4,formCompra.limite_4,formCompra.subtotal_4,document.getElementById('subtotald_4'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_4" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_4" size="4" value="0.85">
                            R$ 0.85                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_4" id="subtotald_4" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_4" name="subtotal_4" size="4">
                        </td>

                        <input type="hidden" name="codfor_4" id="987" value="987">
                        <input type="hidden" name="codP_id4" id="2013" value="2013">
                        <input type="hidden" name="prodNomeSimples4" id="AGULHA DE COSTURA" value="AGULHA DE COSTURA">
                        <input type="hidden" name="pro_percaptamaxima4" id="2" value="2">
                        <input type="hidden" name="pro_percaptamaximaSap4" id="2" value="2">
                        <input type="hidden" name="uni_nome4" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd4" id="1" value="1">
                        <input type="hidden" name="cod_4" id="137450" value="137450">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            116207 -  AMACIANTE DE ROUPAS DOWNY CONCENTRADO 500 MILILITRO                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_5" onchange="subtot(document.formCompra.qtde_5,formCompra.preco_5,formCompra.limite_5,formCompra.subtotal_5,document.getElementById('subtotald_5'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_5" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_5" size="4" value="10.98">
                            R$ 10.98                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_5" id="subtotald_5" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_5" name="subtotal_5" size="4">
                        </td>

                        <input type="hidden" name="codfor_5" id="1232" value="1232">
                        <input type="hidden" name="codP_id5" id="2019" value="2019">
                        <input type="hidden" name="prodNomeSimples5" id="AMACIANTE DE ROUPAS" value="AMACIANTE DE ROUPAS">
                        <input type="hidden" name="pro_percaptamaxima5" id="500" value="500">
                        <input type="hidden" name="pro_percaptamaximaSap5" id="2000" value="2000">
                        <input type="hidden" name="uni_nome5" id="MILILITRO" value="MILILITRO">
                        <input type="hidden" name="proUniQtd5" id="500" value="500">
                        <input type="hidden" name="cod_5" id="116207" value="116207">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            136998 -  AMENDOIM TIPO JAPONES 400 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_6" onchange="subtot(document.formCompra.qtde_6,formCompra.preco_6,formCompra.limite_6,formCompra.subtotal_6,document.getElementById('subtotald_6'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_6" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_6" size="4" value="9.20">
                            R$ 9.20                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_6" id="subtotald_6" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_6" name="subtotal_6" size="4">
                        </td>

                        <input type="hidden" name="codfor_6" id="987" value="987">
                        <input type="hidden" name="codP_id6" id="2020" value="2020">
                        <input type="hidden" name="prodNomeSimples6" id="AMENDOIM" value="AMENDOIM">
                        <input type="hidden" name="pro_percaptamaxima6" id="400" value="400">
                        <input type="hidden" name="pro_percaptamaximaSap6" id="500" value="500">
                        <input type="hidden" name="uni_nome6" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd6" id="400" value="400">
                        <input type="hidden" name="cod_6" id="136998" value="136998">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            109268 -  APARELHO DE BARBEAR GILLETTE PRESTOBARBA C/ 2 UNID. 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_7" onchange="subtot(document.formCompra.qtde_7,formCompra.preco_7,formCompra.limite_7,formCompra.subtotal_7,document.getElementById('subtotald_7'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_7" size="4" value="5">
                            5                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_7" size="4" value="4.18">
                            R$ 4.18                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_7" id="subtotald_7" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_7" name="subtotal_7" size="4">
                        </td>

                        <input type="hidden" name="codfor_7" id="2737" value="2737">
                        <input type="hidden" name="codP_id7" id="2023" value="2023">
                        <input type="hidden" name="prodNomeSimples7" id="APARELHO DE BARBEAR" value="APARELHO DE BARBEAR">
                        <input type="hidden" name="pro_percaptamaxima7" id="5" value="5">
                        <input type="hidden" name="pro_percaptamaximaSap7" id="10" value="10">
                        <input type="hidden" name="uni_nome7" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd7" id="1" value="1">
                        <input type="hidden" name="cod_7" id="109268" value="109268">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            103715 -  AVEIA EM FLOCOS QUAKER 165 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_8" onchange="subtot(document.formCompra.qtde_8,formCompra.preco_8,formCompra.limite_8,formCompra.subtotal_8,document.getElementById('subtotald_8'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_8" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_8" size="4" value="4.89">
                            R$ 4.89                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_8" id="subtotald_8" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_8" name="subtotal_8" size="4">
                        </td>

                        <input type="hidden" name="codfor_8" id="1232" value="1232">
                        <input type="hidden" name="codP_id8" id="2025" value="2025">
                        <input type="hidden" name="prodNomeSimples8" id="AVEIA EM FLOCOS" value="AVEIA EM FLOCOS">
                        <input type="hidden" name="pro_percaptamaxima8" id="250" value="250">
                        <input type="hidden" name="pro_percaptamaximaSap8" id="250" value="250">
                        <input type="hidden" name="uni_nome8" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd8" id="165" value="165">
                        <input type="hidden" name="cod_8" id="103715" value="103715">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            127802 -  BALA  CHITA / ERLAN SORTIDA 500 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_9" onchange="subtot(document.formCompra.qtde_9,formCompra.preco_9,formCompra.limite_9,formCompra.subtotal_9,document.getElementById('subtotald_9'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_9" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_9" size="4" value="8.49">
                            R$ 8.49                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_9" id="subtotald_9" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_9" name="subtotal_9" size="4">
                        </td>

                        <input type="hidden" name="codfor_9" id="1232" value="1232">
                        <input type="hidden" name="codP_id9" id="2028" value="2028">
                        <input type="hidden" name="prodNomeSimples9" id="BALA " value="BALA ">
                        <input type="hidden" name="pro_percaptamaxima9" id="500" value="500">
                        <input type="hidden" name="pro_percaptamaximaSap9" id="700" value="700">
                        <input type="hidden" name="uni_nome9" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd9" id="500" value="500">
                        <input type="hidden" name="cod_9" id="127802" value="127802">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            114831 -  BALDE LISTA 15 LITRO                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_10" onchange="subtot(document.formCompra.qtde_10,formCompra.preco_10,formCompra.limite_10,formCompra.subtotal_10,document.getElementById('subtotald_10'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_10" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_10" size="4" value="13.40">
                            R$ 13.40                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_10" id="subtotald_10" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_10" name="subtotal_10" size="4">
                        </td>

                        <input type="hidden" name="codfor_10" id="987" value="987">
                        <input type="hidden" name="codP_id10" id="2029" value="2029">
                        <input type="hidden" name="prodNomeSimples10" id="BALDE" value="BALDE">
                        <input type="hidden" name="pro_percaptamaxima10" id="15" value="15">
                        <input type="hidden" name="pro_percaptamaximaSap10" id="20" value="20">
                        <input type="hidden" name="uni_nome10" id="LITRO" value="LITRO">
                        <input type="hidden" name="proUniQtd10" id="15" value="15">
                        <input type="hidden" name="cod_10" id="114831" value="114831">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            126514 -  BISCOITO EM PACOTE PANCO ROSQUINHA 500G 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_11" onchange="subtot(document.formCompra.qtde_11,formCompra.preco_11,formCompra.limite_11,formCompra.subtotal_11,document.getElementById('subtotald_11'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_11" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_11" size="4" value="6.98">
                            R$ 6.98                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_11" id="subtotald_11" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_11" name="subtotal_11" size="4">
                        </td>

                        <input type="hidden" name="codfor_11" id="2737" value="2737">
                        <input type="hidden" name="codP_id11" id="2035" value="2035">
                        <input type="hidden" name="prodNomeSimples11" id="BISCOITO EM PACOTE" value="BISCOITO EM PACOTE">
                        <input type="hidden" name="pro_percaptamaxima11" id="1" value="1">
                        <input type="hidden" name="pro_percaptamaximaSap11" id="3" value="3">
                        <input type="hidden" name="uni_nome11" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd11" id="1" value="1">
                        <input type="hidden" name="cod_11" id="126514" value="126514">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            135638 -  BISCOITO WAFER PANCO 112 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_12" onchange="subtot(document.formCompra.qtde_12,formCompra.preco_12,formCompra.limite_12,formCompra.subtotal_12,document.getElementById('subtotald_12'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_12" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_12" size="4" value="3.44">
                            R$ 3.44                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_12" id="subtotald_12" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_12" name="subtotal_12" size="4">
                        </td>

                        <input type="hidden" name="codfor_12" id="1232" value="1232">
                        <input type="hidden" name="codP_id12" id="2036" value="2036">
                        <input type="hidden" name="prodNomeSimples12" id="BISCOITO WAFER" value="BISCOITO WAFER">
                        <input type="hidden" name="pro_percaptamaxima12" id="112" value="112">
                        <input type="hidden" name="pro_percaptamaximaSap12" id="140" value="140">
                        <input type="hidden" name="uni_nome12" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd12" id="112" value="112">
                        <input type="hidden" name="cod_12" id="135638" value="135638">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            135642 -  BISNAGUINHA PANCO 300 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_13" onchange="subtot(document.formCompra.qtde_13,formCompra.preco_13,formCompra.limite_13,formCompra.subtotal_13,document.getElementById('subtotald_13'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_13" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_13" size="4" value="8.45">
                            R$ 8.45                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_13" id="subtotald_13" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_13" name="subtotal_13" size="4">
                        </td>

                        <input type="hidden" name="codfor_13" id="1232" value="1232">
                        <input type="hidden" name="codP_id13" id="2037" value="2037">
                        <input type="hidden" name="prodNomeSimples13" id="BISNAGUINHA" value="BISNAGUINHA">
                        <input type="hidden" name="pro_percaptamaxima13" id="300" value="300">
                        <input type="hidden" name="pro_percaptamaximaSap13" id="300" value="300">
                        <input type="hidden" name="uni_nome13" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd13" id="300" value="300">
                        <input type="hidden" name="cod_13" id="135642" value="135642">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            103744 -  BOLACHA AGUA E SAL MARILAN 350G 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_14" onchange="subtot(document.formCompra.qtde_14,formCompra.preco_14,formCompra.limite_14,formCompra.subtotal_14,document.getElementById('subtotald_14'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_14" size="4" value="4">
                            4                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_14" size="4" value="4.46">
                            R$ 4.46                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_14" id="subtotald_14" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_14" name="subtotal_14" size="4">
                        </td>

                        <input type="hidden" name="codfor_14" id="2737" value="2737">
                        <input type="hidden" name="codP_id14" id="2040" value="2040">
                        <input type="hidden" name="prodNomeSimples14" id="BOLACHA AGUA E SAL" value="BOLACHA AGUA E SAL">
                        <input type="hidden" name="pro_percaptamaxima14" id="4" value="4">
                        <input type="hidden" name="pro_percaptamaximaSap14" id="5" value="5">
                        <input type="hidden" name="uni_nome14" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd14" id="1" value="1">
                        <input type="hidden" name="cod_14" id="103744" value="103744">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            133295 -  BOLACHA DE MAISENA MARILAN 300G	 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_15" onchange="subtot(document.formCompra.qtde_15,formCompra.preco_15,formCompra.limite_15,formCompra.subtotal_15,document.getElementById('subtotald_15'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_15" size="4" value="4">
                            4                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_15" size="4" value="4.46">
                            R$ 4.46                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_15" id="subtotald_15" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_15" name="subtotal_15" size="4">
                        </td>

                        <input type="hidden" name="codfor_15" id="2737" value="2737">
                        <input type="hidden" name="codP_id15" id="2041" value="2041">
                        <input type="hidden" name="prodNomeSimples15" id="BOLACHA DE MAISENA" value="BOLACHA DE MAISENA">
                        <input type="hidden" name="pro_percaptamaxima15" id="4" value="4">
                        <input type="hidden" name="pro_percaptamaximaSap15" id="5" value="5">
                        <input type="hidden" name="uni_nome15" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd15" id="1" value="1">
                        <input type="hidden" name="cod_15" id="133295" value="133295">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            130017 -  BOLACHA RECHEADA PASSATEMPO NESTLE  1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_16" onchange="subtot(document.formCompra.qtde_16,formCompra.preco_16,formCompra.limite_16,formCompra.subtotal_16,document.getElementById('subtotald_16'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_16" size="4" value="4">
                            4                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_16" size="4" value="2.08">
                            R$ 2.08                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_16" id="subtotald_16" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_16" name="subtotal_16" size="4">
                        </td>

                        <input type="hidden" name="codfor_16" id="2737" value="2737">
                        <input type="hidden" name="codP_id16" id="2043" value="2043">
                        <input type="hidden" name="prodNomeSimples16" id="BOLACHA RECHEADA" value="BOLACHA RECHEADA">
                        <input type="hidden" name="pro_percaptamaxima16" id="4" value="4">
                        <input type="hidden" name="pro_percaptamaximaSap16" id="5" value="5">
                        <input type="hidden" name="uni_nome16" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd16" id="1" value="1">
                        <input type="hidden" name="cod_16" id="130017" value="130017">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            121814 -  BOLO INDUSTRIALIZADO PULLMAN / PANCO- SABORES 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_17" onchange="subtot(document.formCompra.qtde_17,formCompra.preco_17,formCompra.limite_17,formCompra.subtotal_17,document.getElementById('subtotald_17'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_17" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_17" size="4" value="8.59">
                            R$ 8.59                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_17" id="subtotald_17" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_17" name="subtotal_17" size="4">
                        </td>

                        <input type="hidden" name="codfor_17" id="1232" value="1232">
                        <input type="hidden" name="codP_id17" id="2045" value="2045">
                        <input type="hidden" name="prodNomeSimples17" id="BOLO INDUSTRIALIZADO" value="BOLO INDUSTRIALIZADO">
                        <input type="hidden" name="pro_percaptamaxima17" id="2" value="2">
                        <input type="hidden" name="pro_percaptamaximaSap17" id="4" value="4">
                        <input type="hidden" name="uni_nome17" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd17" id="1" value="1">
                        <input type="hidden" name="cod_17" id="121814" value="121814">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            121813 -  BOMBOM CAIXA NESTLE ESPECIALIDADES 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_18" onchange="subtot(document.formCompra.qtde_18,formCompra.preco_18,formCompra.limite_18,formCompra.subtotal_18,document.getElementById('subtotald_18'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_18" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_18" size="4" value="12.58">
                            R$ 12.58                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_18" id="subtotald_18" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_18" name="subtotal_18" size="4">
                        </td>

                        <input type="hidden" name="codfor_18" id="1232" value="1232">
                        <input type="hidden" name="codP_id18" id="2047" value="2047">
                        <input type="hidden" name="prodNomeSimples18" id="BOMBOM CAIXA" value="BOMBOM CAIXA">
                        <input type="hidden" name="pro_percaptamaxima18" id="2" value="2">
                        <input type="hidden" name="pro_percaptamaximaSap18" id="6" value="6">
                        <input type="hidden" name="uni_nome18" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd18" id="1" value="1">
                        <input type="hidden" name="cod_18" id="121813" value="121813">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            137495 -  BOMBOM LACTA Ouro Branco Pcte 1kg 1 CAIXA                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_19" onchange="subtot(document.formCompra.qtde_19,formCompra.preco_19,formCompra.limite_19,formCompra.subtotal_19,document.getElementById('subtotald_19'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_19" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_19" size="4" value="59.00">
                            R$ 59.00                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_19" id="subtotald_19" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_19" name="subtotal_19" size="4">
                        </td>

                        <input type="hidden" name="codfor_19" id="987" value="987">
                        <input type="hidden" name="codP_id19" id="2170" value="2170">
                        <input type="hidden" name="prodNomeSimples19" id="BOMBOM LACTA" value="BOMBOM LACTA">
                        <input type="hidden" name="pro_percaptamaxima19" id="1" value="1">
                        <input type="hidden" name="pro_percaptamaximaSap19" id="3" value="3">
                        <input type="hidden" name="uni_nome19" id="CAIXA" value="CAIXA">
                        <input type="hidden" name="proUniQtd19" id="1" value="1">
                        <input type="hidden" name="cod_19" id="137495" value="137495">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            108514 -  CADERNO BROCHURA  BROCHURAO 80 FOLHA (GRANDE) 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_20" onchange="subtot(document.formCompra.qtde_20,formCompra.preco_20,formCompra.limite_20,formCompra.subtotal_20,document.getElementById('subtotald_20'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_20" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_20" size="4" value="4.98">
                            R$ 4.98                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_20" id="subtotald_20" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_20" name="subtotal_20" size="4">
                        </td>

                        <input type="hidden" name="codfor_20" id="2737" value="2737">
                        <input type="hidden" name="codP_id20" id="2050" value="2050">
                        <input type="hidden" name="prodNomeSimples20" id="CADERNO BROCHURA " value="CADERNO BROCHURA ">
                        <input type="hidden" name="pro_percaptamaxima20" id="2" value="2">
                        <input type="hidden" name="pro_percaptamaximaSap20" id="2" value="2">
                        <input type="hidden" name="uni_nome20" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd20" id="1" value="1">
                        <input type="hidden" name="cod_20" id="108514" value="108514">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            103773 -  CALCADOS CHINELO TIPO HAVAIANAS 37-38 1 PAR                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_21" onchange="subtot(document.formCompra.qtde_21,formCompra.preco_21,formCompra.limite_21,formCompra.subtotal_21,document.getElementById('subtotald_21'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_21" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_21" size="4" value="17.88">
                            R$ 17.88                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_21" id="subtotald_21" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_21" name="subtotal_21" size="4">
                        </td>

                        <input type="hidden" name="codfor_21" id="2737" value="2737">
                        <input type="hidden" name="codP_id21" id="2165" value="2165">
                        <input type="hidden" name="prodNomeSimples21" id="CALCADOS CHINELO" value="CALCADOS CHINELO">
                        <input type="hidden" name="pro_percaptamaxima21" id="1" value="1">
                        <input type="hidden" name="pro_percaptamaximaSap21" id="1" value="1">
                        <input type="hidden" name="uni_nome21" id="PAR" value="PAR">
                        <input type="hidden" name="proUniQtd21" id="1" value="1">
                        <input type="hidden" name="cod_21" id="103773" value="103773">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            103774 -  CALCADOS CHINELO TIPO HAVAIANAS 39-40 1 PAR                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_22" onchange="subtot(document.formCompra.qtde_22,formCompra.preco_22,formCompra.limite_22,formCompra.subtotal_22,document.getElementById('subtotald_22'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_22" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_22" size="4" value="17.88">
                            R$ 17.88                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_22" id="subtotald_22" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_22" name="subtotal_22" size="4">
                        </td>

                        <input type="hidden" name="codfor_22" id="2737" value="2737">
                        <input type="hidden" name="codP_id22" id="2165" value="2165">
                        <input type="hidden" name="prodNomeSimples22" id="CALCADOS CHINELO" value="CALCADOS CHINELO">
                        <input type="hidden" name="pro_percaptamaxima22" id="1" value="1">
                        <input type="hidden" name="pro_percaptamaximaSap22" id="1" value="1">
                        <input type="hidden" name="uni_nome22" id="PAR" value="PAR">
                        <input type="hidden" name="proUniQtd22" id="1" value="1">
                        <input type="hidden" name="cod_22" id="103774" value="103774">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            103775 -  CALCADOS CHINELO TIPO HAVAIANAS 41-42 1 PAR                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_23" onchange="subtot(document.formCompra.qtde_23,formCompra.preco_23,formCompra.limite_23,formCompra.subtotal_23,document.getElementById('subtotald_23'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_23" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_23" size="4" value="17.88">
                            R$ 17.88                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_23" id="subtotald_23" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_23" name="subtotal_23" size="4">
                        </td>

                        <input type="hidden" name="codfor_23" id="2737" value="2737">
                        <input type="hidden" name="codP_id23" id="2165" value="2165">
                        <input type="hidden" name="prodNomeSimples23" id="CALCADOS CHINELO" value="CALCADOS CHINELO">
                        <input type="hidden" name="pro_percaptamaxima23" id="1" value="1">
                        <input type="hidden" name="pro_percaptamaximaSap23" id="1" value="1">
                        <input type="hidden" name="uni_nome23" id="PAR" value="PAR">
                        <input type="hidden" name="proUniQtd23" id="1" value="1">
                        <input type="hidden" name="cod_23" id="103775" value="103775">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            103776 -  CALCADOS CHINELO TIPO HAVAIANAS 43-44 1 PAR                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_24" onchange="subtot(document.formCompra.qtde_24,formCompra.preco_24,formCompra.limite_24,formCompra.subtotal_24,document.getElementById('subtotald_24'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_24" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_24" size="4" value="17.89">
                            R$ 17.89                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_24" id="subtotald_24" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_24" name="subtotal_24" size="4">
                        </td>

                        <input type="hidden" name="codfor_24" id="1232" value="1232">
                        <input type="hidden" name="codP_id24" id="2165" value="2165">
                        <input type="hidden" name="prodNomeSimples24" id="CALCADOS CHINELO" value="CALCADOS CHINELO">
                        <input type="hidden" name="pro_percaptamaxima24" id="1" value="1">
                        <input type="hidden" name="pro_percaptamaximaSap24" id="1" value="1">
                        <input type="hidden" name="uni_nome24" id="PAR" value="PAR">
                        <input type="hidden" name="proUniQtd24" id="1" value="1">
                        <input type="hidden" name="cod_24" id="103776" value="103776">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            127353 -  CANETA ESFEROGRAFICA BIC - VERDE/VERMELHA 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_25" onchange="subtot(document.formCompra.qtde_25,formCompra.preco_25,formCompra.limite_25,formCompra.subtotal_25,document.getElementById('subtotald_25'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_25" size="4" value="3">
                            3                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_25" size="4" value="0.78">
                            R$ 0.78                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_25" id="subtotald_25" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_25" name="subtotal_25" size="4">
                        </td>

                        <input type="hidden" name="codfor_25" id="2737" value="2737">
                        <input type="hidden" name="codP_id25" id="2058" value="2058">
                        <input type="hidden" name="prodNomeSimples25" id="CANETA ESFEROGRAFICA" value="CANETA ESFEROGRAFICA">
                        <input type="hidden" name="pro_percaptamaxima25" id="3" value="3">
                        <input type="hidden" name="pro_percaptamaximaSap25" id="3" value="3">
                        <input type="hidden" name="uni_nome25" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd25" id="1" value="1">
                        <input type="hidden" name="cod_25" id="127353" value="127353">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            135639 -  CATCHUP D AJUDA 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_26" onchange="subtot(document.formCompra.qtde_26,formCompra.preco_26,formCompra.limite_26,formCompra.subtotal_26,document.getElementById('subtotald_26'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_26" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_26" size="4" value="2.12">
                            R$ 2.12                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_26" id="subtotald_26" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_26" name="subtotal_26" size="4">
                        </td>

                        <input type="hidden" name="codfor_26" id="2737" value="2737">
                        <input type="hidden" name="codP_id26" id="2060" value="2060">
                        <input type="hidden" name="prodNomeSimples26" id="CATCHUP" value="CATCHUP">
                        <input type="hidden" name="pro_percaptamaxima26" id="2" value="2">
                        <input type="hidden" name="pro_percaptamaximaSap26" id="2" value="2">
                        <input type="hidden" name="uni_nome26" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd26" id="1" value="1">
                        <input type="hidden" name="cod_26" id="135639" value="135639">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            134369 -  CHOCOLATE EM BARRA  NESTLE 90 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_27" onchange="subtot(document.formCompra.qtde_27,formCompra.preco_27,formCompra.limite_27,formCompra.subtotal_27,document.getElementById('subtotald_27'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_27" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_27" size="4" value="7.48">
                            R$ 7.48                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_27" id="subtotald_27" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_27" name="subtotal_27" size="4">
                        </td>

                        <input type="hidden" name="codfor_27" id="2737" value="2737">
                        <input type="hidden" name="codP_id27" id="2062" value="2062">
                        <input type="hidden" name="prodNomeSimples27" id="CHOCOLATE EM BARRA " value="CHOCOLATE EM BARRA ">
                        <input type="hidden" name="pro_percaptamaxima27" id="180" value="180">
                        <input type="hidden" name="pro_percaptamaximaSap27" id="200" value="200">
                        <input type="hidden" name="uni_nome27" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd27" id="90" value="90">
                        <input type="hidden" name="cod_27" id="134369" value="134369">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            107354 -  CIGARRO MACO ROTHMANS (HILTON) 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_28" onchange="subtot(document.formCompra.qtde_28,formCompra.preco_28,formCompra.limite_28,formCompra.subtotal_28,document.getElementById('subtotald_28'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_28" size="4" value="20">
                            20                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_28" size="4" value="7.60">
                            R$ 7.60                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_28" id="subtotald_28" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_28" name="subtotal_28" size="4">
                        </td>

                        <input type="hidden" name="codfor_28" id="987" value="987">
                        <input type="hidden" name="codP_id28" id="2064" value="2064">
                        <input type="hidden" name="prodNomeSimples28" id="CIGARRO MACO" value="CIGARRO MACO">
                        <input type="hidden" name="pro_percaptamaxima28" id="20" value="20">
                        <input type="hidden" name="pro_percaptamaximaSap28" id="40" value="40">
                        <input type="hidden" name="uni_nome28" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd28" id="1" value="1">
                        <input type="hidden" name="cod_28" id="107354" value="107354">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            103821 -  CORTADOR DE UNHAS  1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_29" onchange="subtot(document.formCompra.qtde_29,formCompra.preco_29,formCompra.limite_29,formCompra.subtotal_29,document.getElementById('subtotald_29'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_29" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_29" size="4" value="2.08">
                            R$ 2.08                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_29" id="subtotald_29" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_29" name="subtotal_29" size="4">
                        </td>

                        <input type="hidden" name="codfor_29" id="2737" value="2737">
                        <input type="hidden" name="codP_id29" id="2068" value="2068">
                        <input type="hidden" name="prodNomeSimples29" id="CORTADOR DE UNHAS" value="CORTADOR DE UNHAS">
                        <input type="hidden" name="pro_percaptamaxima29" id="1" value="1">
                        <input type="hidden" name="pro_percaptamaximaSap29" id="1" value="1">
                        <input type="hidden" name="uni_nome29" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd29" id="1" value="1">
                        <input type="hidden" name="cod_29" id="103821" value="103821">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            135646 -  CORTINA DE BOX 1/CELA - PAGO NA INCLUSAO 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_30" onchange="subtot(document.formCompra.qtde_30,formCompra.preco_30,formCompra.limite_30,formCompra.subtotal_30,document.getElementById('subtotald_30'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_30" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_30" size="4" value="45.00">
                            R$ 45.00                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_30" id="subtotald_30" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_30" name="subtotal_30" size="4">
                        </td>

                        <input type="hidden" name="codfor_30" id="987" value="987">
                        <input type="hidden" name="codP_id30" id="2168" value="2168">
                        <input type="hidden" name="prodNomeSimples30" id="CORTINA DE BOX" value="CORTINA DE BOX">
                        <input type="hidden" name="pro_percaptamaxima30" id="1" value="1">
                        <input type="hidden" name="pro_percaptamaximaSap30" id="1" value="1">
                        <input type="hidden" name="uni_nome30" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd30" id="1" value="1">
                        <input type="hidden" name="cod_30" id="135646" value="135646">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            119942 -  CREME DE BARBEAR BOZZANO 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_31" onchange="subtot(document.formCompra.qtde_31,formCompra.preco_31,formCompra.limite_31,formCompra.subtotal_31,document.getElementById('subtotald_31'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_31" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_31" size="4" value="7.98">
                            R$ 7.98                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_31" id="subtotald_31" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_31" name="subtotal_31" size="4">
                        </td>

                        <input type="hidden" name="codfor_31" id="1232" value="1232">
                        <input type="hidden" name="codP_id31" id="2071" value="2071">
                        <input type="hidden" name="prodNomeSimples31" id="CREME DE BARBEAR" value="CREME DE BARBEAR">
                        <input type="hidden" name="pro_percaptamaxima31" id="1" value="1">
                        <input type="hidden" name="pro_percaptamaximaSap31" id="1" value="1">
                        <input type="hidden" name="uni_nome31" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd31" id="1" value="1">
                        <input type="hidden" name="cod_31" id="119942" value="119942">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            107355 -  CREME DENTAL COLGATE  90 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_32" onchange="subtot(document.formCompra.qtde_32,formCompra.preco_32,formCompra.limite_32,formCompra.subtotal_32,document.getElementById('subtotald_32'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_32" size="4" value="4">
                            4                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_32" size="4" value="3.66">
                            R$ 3.66                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_32" id="subtotald_32" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_32" name="subtotal_32" size="4">
                        </td>

                        <input type="hidden" name="codfor_32" id="2737" value="2737">
                        <input type="hidden" name="codP_id32" id="2073" value="2073">
                        <input type="hidden" name="prodNomeSimples32" id="CREME DENTAL" value="CREME DENTAL">
                        <input type="hidden" name="pro_percaptamaxima32" id="360" value="360">
                        <input type="hidden" name="pro_percaptamaximaSap32" id="360" value="360">
                        <input type="hidden" name="uni_nome32" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd32" id="90" value="90">
                        <input type="hidden" name="cod_32" id="107355" value="107355">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            103845 -  CREME HIDRATANTE MONANGE 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_33" onchange="subtot(document.formCompra.qtde_33,formCompra.preco_33,formCompra.limite_33,formCompra.subtotal_33,document.getElementById('subtotald_33'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_33" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_33" size="4" value="8.48">
                            R$ 8.48                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_33" id="subtotald_33" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_33" name="subtotal_33" size="4">
                        </td>

                        <input type="hidden" name="codfor_33" id="1232" value="1232">
                        <input type="hidden" name="codP_id33" id="2075" value="2075">
                        <input type="hidden" name="prodNomeSimples33" id="CREME HIDRATANTE" value="CREME HIDRATANTE">
                        <input type="hidden" name="pro_percaptamaxima33" id="1" value="1">
                        <input type="hidden" name="pro_percaptamaximaSap33" id="1" value="1">
                        <input type="hidden" name="uni_nome33" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd33" id="1" value="1">
                        <input type="hidden" name="cod_33" id="103845" value="103845">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            113026 -  DESINFETANTE URCA 2000 MILILITRO                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_34" onchange="subtot(document.formCompra.qtde_34,formCompra.preco_34,formCompra.limite_34,formCompra.subtotal_34,document.getElementById('subtotald_34'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_34" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_34" size="4" value="5.94">
                            R$ 5.94                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_34" id="subtotald_34" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_34" name="subtotal_34" size="4">
                        </td>

                        <input type="hidden" name="codfor_34" id="1232" value="1232">
                        <input type="hidden" name="codP_id34" id="2079" value="2079">
                        <input type="hidden" name="prodNomeSimples34" id="DESINFETANTE" value="DESINFETANTE">
                        <input type="hidden" name="pro_percaptamaxima34" id="2000" value="2000">
                        <input type="hidden" name="pro_percaptamaximaSap34" id="2000" value="2000">
                        <input type="hidden" name="uni_nome34" id="MILILITRO" value="MILILITRO">
                        <input type="hidden" name="proUniQtd34" id="2000" value="2000">
                        <input type="hidden" name="cod_34" id="113026" value="113026">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            122495 -  DESODORANTE ROLL-ON REXONA 50ml 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_35" onchange="subtot(document.formCompra.qtde_35,formCompra.preco_35,formCompra.limite_35,formCompra.subtotal_35,document.getElementById('subtotald_35'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_35" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_35" size="4" value="10.54">
                            R$ 10.54                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_35" id="subtotald_35" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_35" name="subtotal_35" size="4">
                        </td>

                        <input type="hidden" name="codfor_35" id="1232" value="1232">
                        <input type="hidden" name="codP_id35" id="2080" value="2080">
                        <input type="hidden" name="prodNomeSimples35" id="DESODORANTE ROLL-ON" value="DESODORANTE ROLL-ON">
                        <input type="hidden" name="pro_percaptamaxima35" id="2" value="2">
                        <input type="hidden" name="pro_percaptamaximaSap35" id="2" value="2">
                        <input type="hidden" name="uni_nome35" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd35" id="1" value="1">
                        <input type="hidden" name="cod_35" id="122495" value="122495">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            137461 -  DETERGENTE NEUTRO MINUANO/LIMPOL/YPE 500 MILILITRO                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_36" onchange="subtot(document.formCompra.qtde_36,formCompra.preco_36,formCompra.limite_36,formCompra.subtotal_36,document.getElementById('subtotald_36'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_36" size="4" value="3">
                            3                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_36" size="4" value="2.38">
                            R$ 2.38                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_36" id="subtotald_36" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_36" name="subtotal_36" size="4">
                        </td>

                        <input type="hidden" name="codfor_36" id="2737" value="2737">
                        <input type="hidden" name="codP_id36" id="2081" value="2081">
                        <input type="hidden" name="prodNomeSimples36" id="DETERGENTE NEUTRO" value="DETERGENTE NEUTRO">
                        <input type="hidden" name="pro_percaptamaxima36" id="1500" value="1500">
                        <input type="hidden" name="pro_percaptamaximaSap36" id="1500" value="1500">
                        <input type="hidden" name="uni_nome36" id="MILILITRO" value="MILILITRO">
                        <input type="hidden" name="proUniQtd36" id="500" value="500">
                        <input type="hidden" name="cod_36" id="137461" value="137461">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            114830 -  ENVELOPE CARTA LISTA 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_37" onchange="subtot(document.formCompra.qtde_37,formCompra.preco_37,formCompra.limite_37,formCompra.subtotal_37,document.getElementById('subtotald_37'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_37" size="4" value="20">
                            20                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_37" size="4" value="0.26">
                            R$ 0.26                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_37" id="subtotald_37" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_37" name="subtotal_37" size="4">
                        </td>

                        <input type="hidden" name="codfor_37" id="1232" value="1232">
                        <input type="hidden" name="codP_id37" id="2083" value="2083">
                        <input type="hidden" name="prodNomeSimples37" id="ENVELOPE CARTA" value="ENVELOPE CARTA">
                        <input type="hidden" name="pro_percaptamaxima37" id="20" value="20">
                        <input type="hidden" name="pro_percaptamaximaSap37" id="20" value="20">
                        <input type="hidden" name="uni_nome37" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd37" id="1" value="1">
                        <input type="hidden" name="cod_37" id="114830" value="114830">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            103861 -  ESCOVA DENTAL ORAL B 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_38" onchange="subtot(document.formCompra.qtde_38,formCompra.preco_38,formCompra.limite_38,formCompra.subtotal_38,document.getElementById('subtotald_38'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_38" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_38" size="4" value="2.82">
                            R$ 2.82                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_38" id="subtotald_38" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_38" name="subtotal_38" size="4">
                        </td>

                        <input type="hidden" name="codfor_38" id="2737" value="2737">
                        <input type="hidden" name="codP_id38" id="2085" value="2085">
                        <input type="hidden" name="prodNomeSimples38" id="ESCOVA DENTAL" value="ESCOVA DENTAL">
                        <input type="hidden" name="pro_percaptamaxima38" id="1" value="1">
                        <input type="hidden" name="pro_percaptamaximaSap38" id="2" value="2">
                        <input type="hidden" name="uni_nome38" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd38" id="1" value="1">
                        <input type="hidden" name="cod_38" id="103861" value="103861">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            111249 -  ESCOVA P/ LAVAR ROUPA   1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_39" onchange="subtot(document.formCompra.qtde_39,formCompra.preco_39,formCompra.limite_39,formCompra.subtotal_39,document.getElementById('subtotald_39'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_39" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_39" size="4" value="3.00">
                            R$ 3.00                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_39" id="subtotald_39" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_39" name="subtotal_39" size="4">
                        </td>

                        <input type="hidden" name="codfor_39" id="987" value="987">
                        <input type="hidden" name="codP_id39" id="2087" value="2087">
                        <input type="hidden" name="prodNomeSimples39" id="ESCOVA P/ LAVAR ROUPA " value="ESCOVA P/ LAVAR ROUPA ">
                        <input type="hidden" name="pro_percaptamaxima39" id="1" value="1">
                        <input type="hidden" name="pro_percaptamaximaSap39" id="1" value="1">
                        <input type="hidden" name="uni_nome39" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd39" id="1" value="1">
                        <input type="hidden" name="cod_39" id="111249" value="111249">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            135647 -  ESPELHO N 12 COMUM 1/CELA - PAGO NA INCLUSAO 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_40" onchange="subtot(document.formCompra.qtde_40,formCompra.preco_40,formCompra.limite_40,formCompra.subtotal_40,document.getElementById('subtotald_40'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_40" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_40" size="4" value="5.50">
                            R$ 5.50                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_40" id="subtotald_40" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_40" name="subtotal_40" size="4">
                        </td>

                        <input type="hidden" name="codfor_40" id="987" value="987">
                        <input type="hidden" name="codP_id40" id="2089" value="2089">
                        <input type="hidden" name="prodNomeSimples40" id="ESPELHO N 12 COMUM" value="ESPELHO N 12 COMUM">
                        <input type="hidden" name="pro_percaptamaxima40" id="1" value="1">
                        <input type="hidden" name="pro_percaptamaximaSap40" id="1" value="1">
                        <input type="hidden" name="uni_nome40" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd40" id="1" value="1">
                        <input type="hidden" name="cod_40" id="135647" value="135647">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            103868 -  ESPONJA COZINHA  1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_41" onchange="subtot(document.formCompra.qtde_41,formCompra.preco_41,formCompra.limite_41,formCompra.subtotal_41,document.getElementById('subtotald_41'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_41" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_41" size="4" value="0.69">
                            R$ 0.69                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_41" id="subtotald_41" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_41" name="subtotal_41" size="4">
                        </td>

                        <input type="hidden" name="codfor_41" id="987" value="987">
                        <input type="hidden" name="codP_id41" id="2090" value="2090">
                        <input type="hidden" name="prodNomeSimples41" id="ESPONJA COZINHA" value="ESPONJA COZINHA">
                        <input type="hidden" name="pro_percaptamaxima41" id="2" value="2">
                        <input type="hidden" name="pro_percaptamaximaSap41" id="2" value="2">
                        <input type="hidden" name="uni_nome41" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd41" id="1" value="1">
                        <input type="hidden" name="cod_41" id="103868" value="103868">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            135643 -  FARINHA LACTEA  NESTLE 210 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_42" onchange="subtot(document.formCompra.qtde_42,formCompra.preco_42,formCompra.limite_42,formCompra.subtotal_42,document.getElementById('subtotald_42'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_42" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_42" size="4" value="8.66">
                            R$ 8.66                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_42" id="subtotald_42" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_42" name="subtotal_42" size="4">
                        </td>

                        <input type="hidden" name="codfor_42" id="2737" value="2737">
                        <input type="hidden" name="codP_id42" id="2092" value="2092">
                        <input type="hidden" name="prodNomeSimples42" id="FARINHA LACTEA " value="FARINHA LACTEA ">
                        <input type="hidden" name="pro_percaptamaxima42" id="420" value="420">
                        <input type="hidden" name="pro_percaptamaximaSap42" id="500" value="500">
                        <input type="hidden" name="uni_nome42" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd42" id="210" value="210">
                        <input type="hidden" name="cod_42" id="135643" value="135643">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            103878 -  FARINHA TEMPERADA YOKI 400 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_43" onchange="subtot(document.formCompra.qtde_43,formCompra.preco_43,formCompra.limite_43,formCompra.subtotal_43,document.getElementById('subtotald_43'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_43" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_43" size="4" value="4.46">
                            R$ 4.46                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_43" id="subtotald_43" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_43" name="subtotal_43" size="4">
                        </td>

                        <input type="hidden" name="codfor_43" id="2737" value="2737">
                        <input type="hidden" name="codP_id43" id="2093" value="2093">
                        <input type="hidden" name="prodNomeSimples43" id="FARINHA TEMPERADA" value="FARINHA TEMPERADA">
                        <input type="hidden" name="pro_percaptamaxima43" id="400" value="400">
                        <input type="hidden" name="pro_percaptamaximaSap43" id="500" value="500">
                        <input type="hidden" name="uni_nome43" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd43" id="400" value="400">
                        <input type="hidden" name="cod_43" id="103878" value="103878">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            110667 -  FIO DENTAL   100 METRO                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_44" onchange="subtot(document.formCompra.qtde_44,formCompra.preco_44,formCompra.limite_44,formCompra.subtotal_44,document.getElementById('subtotald_44'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_44" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_44" size="4" value="3.58">
                            R$ 3.58                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_44" id="subtotald_44" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_44" name="subtotal_44" size="4">
                        </td>

                        <input type="hidden" name="codfor_44" id="2737" value="2737">
                        <input type="hidden" name="codP_id44" id="2094" value="2094">
                        <input type="hidden" name="prodNomeSimples44" id="FIO DENTAL " value="FIO DENTAL ">
                        <input type="hidden" name="pro_percaptamaxima44" id="100" value="100">
                        <input type="hidden" name="pro_percaptamaximaSap44" id="100" value="100">
                        <input type="hidden" name="uni_nome44" id="METRO" value="METRO">
                        <input type="hidden" name="proUniQtd44" id="100" value="100">
                        <input type="hidden" name="cod_44" id="110667" value="110667">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            131595 -  FUMO DESFIADO JURITI 30 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_45" onchange="subtot(document.formCompra.qtde_45,formCompra.preco_45,formCompra.limite_45,formCompra.subtotal_45,document.getElementById('subtotald_45'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_45" size="4" value="30">
                            30                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_45" size="4" value="4.48">
                            R$ 4.48                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_45" id="subtotald_45" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_45" name="subtotal_45" size="4">
                        </td>

                        <input type="hidden" name="codfor_45" id="1232" value="1232">
                        <input type="hidden" name="codP_id45" id="2096" value="2096">
                        <input type="hidden" name="prodNomeSimples45" id="FUMO DESFIADO" value="FUMO DESFIADO">
                        <input type="hidden" name="pro_percaptamaxima45" id="900" value="900">
                        <input type="hidden" name="pro_percaptamaximaSap45" id="900" value="900">
                        <input type="hidden" name="uni_nome45" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd45" id="30" value="30">
                        <input type="hidden" name="cod_45" id="131595" value="131595">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            115582 -  HASTES FLEXIVEIS TIPO COTONETES 75 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_46" onchange="subtot(document.formCompra.qtde_46,formCompra.preco_46,formCompra.limite_46,formCompra.subtotal_46,document.getElementById('subtotald_46'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_46" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_46" size="4" value="1.68">
                            R$ 1.68                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_46" id="subtotald_46" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_46" name="subtotal_46" size="4">
                        </td>

                        <input type="hidden" name="codfor_46" id="2737" value="2737">
                        <input type="hidden" name="codP_id46" id="2099" value="2099">
                        <input type="hidden" name="prodNomeSimples46" id="HASTES FLEXIVEIS" value="HASTES FLEXIVEIS">
                        <input type="hidden" name="pro_percaptamaxima46" id="75" value="75">
                        <input type="hidden" name="pro_percaptamaximaSap46" id="150" value="150">
                        <input type="hidden" name="uni_nome46" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd46" id="75" value="75">
                        <input type="hidden" name="cod_46" id="115582" value="115582">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            116558 -  ISQUEIRO  HYPER - TIPO CLICK 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_47" onchange="subtot(document.formCompra.qtde_47,formCompra.preco_47,formCompra.limite_47,formCompra.subtotal_47,document.getElementById('subtotald_47'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_47" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_47" size="4" value="1.34">
                            R$ 1.34                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_47" id="subtotald_47" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_47" name="subtotal_47" size="4">
                        </td>

                        <input type="hidden" name="codfor_47" id="2737" value="2737">
                        <input type="hidden" name="codP_id47" id="2101" value="2101">
                        <input type="hidden" name="prodNomeSimples47" id="ISQUEIRO" value="ISQUEIRO">
                        <input type="hidden" name="pro_percaptamaxima47" id="1" value="1">
                        <input type="hidden" name="pro_percaptamaximaSap47" id="3" value="3">
                        <input type="hidden" name="uni_nome47" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd47" id="1" value="1">
                        <input type="hidden" name="cod_47" id="116558" value="116558">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            103909 -  LEITE EM PO ITALAC / ITAMB? 400 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_48" onchange="subtot(document.formCompra.qtde_48,formCompra.preco_48,formCompra.limite_48,formCompra.subtotal_48,document.getElementById('subtotald_48'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_48" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_48" size="4" value="13.86">
                            R$ 13.86                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_48" id="subtotald_48" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_48" name="subtotal_48" size="4">
                        </td>

                        <input type="hidden" name="codfor_48" id="2737" value="2737">
                        <input type="hidden" name="codP_id48" id="2107" value="2107">
                        <input type="hidden" name="prodNomeSimples48" id="LEITE EM PO" value="LEITE EM PO">
                        <input type="hidden" name="pro_percaptamaxima48" id="800" value="800">
                        <input type="hidden" name="pro_percaptamaximaSap48" id="1140" value="1140">
                        <input type="hidden" name="uni_nome48" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd48" id="400" value="400">
                        <input type="hidden" name="cod_48" id="103909" value="103909">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            131597 -  LENCO UMEDECIDO  75 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_49" onchange="subtot(document.formCompra.qtde_49,formCompra.preco_49,formCompra.limite_49,formCompra.subtotal_49,document.getElementById('subtotald_49'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_49" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_49" size="4" value="6.90">
                            R$ 6.90                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_49" id="subtotald_49" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_49" name="subtotal_49" size="4">
                        </td>

                        <input type="hidden" name="codfor_49" id="987" value="987">
                        <input type="hidden" name="codP_id49" id="2110" value="2110">
                        <input type="hidden" name="prodNomeSimples49" id="LENCO UMEDECIDO" value="LENCO UMEDECIDO">
                        <input type="hidden" name="pro_percaptamaxima49" id="75" value="75">
                        <input type="hidden" name="pro_percaptamaximaSap49" id="96" value="96">
                        <input type="hidden" name="uni_nome49" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd49" id="75" value="75">
                        <input type="hidden" name="cod_49" id="131597" value="131597">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            113109 -  MAIONESE DAJUDA/CALCUTA SACHE 200g 200 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_50" onchange="subtot(document.formCompra.qtde_50,formCompra.preco_50,formCompra.limite_50,formCompra.subtotal_50,document.getElementById('subtotald_50'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_50" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_50" size="4" value="1.62">
                            R$ 1.62                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_50" id="subtotald_50" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_50" name="subtotal_50" size="4">
                        </td>

                        <input type="hidden" name="codfor_50" id="2737" value="2737">
                        <input type="hidden" name="codP_id50" id="2113" value="2113">
                        <input type="hidden" name="prodNomeSimples50" id="MAIONESE" value="MAIONESE">
                        <input type="hidden" name="pro_percaptamaxima50" id="400" value="400">
                        <input type="hidden" name="pro_percaptamaximaSap50" id="500" value="500">
                        <input type="hidden" name="uni_nome50" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd50" id="200" value="200">
                        <input type="hidden" name="cod_50" id="113109" value="113109">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            116561 -  MORTADELA MARBA TRADICIONAL (marbinha) 400 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_51" onchange="subtot(document.formCompra.qtde_51,formCompra.preco_51,formCompra.limite_51,formCompra.subtotal_51,document.getElementById('subtotald_51'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_51" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_51" size="4" value="5.98">
                            R$ 5.98                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_51" id="subtotald_51" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_51" name="subtotal_51" size="4">
                        </td>

                        <input type="hidden" name="codfor_51" id="1232" value="1232">
                        <input type="hidden" name="codP_id51" id="2119" value="2119">
                        <input type="hidden" name="prodNomeSimples51" id="MORTADELA" value="MORTADELA">
                        <input type="hidden" name="pro_percaptamaxima51" id="800" value="800">
                        <input type="hidden" name="pro_percaptamaximaSap51" id="1000" value="1000">
                        <input type="hidden" name="uni_nome51" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd51" id="400" value="400">
                        <input type="hidden" name="cod_51" id="116561" value="116561">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            113111 -  MOSTARDA DAJUDA/CALCUTA SACHE 200g 200 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_52" onchange="subtot(document.formCompra.qtde_52,formCompra.preco_52,formCompra.limite_52,formCompra.subtotal_52,document.getElementById('subtotald_52'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_52" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_52" size="4" value="1.46">
                            R$ 1.46                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_52" id="subtotald_52" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_52" name="subtotal_52" size="4">
                        </td>

                        <input type="hidden" name="codfor_52" id="2737" value="2737">
                        <input type="hidden" name="codP_id52" id="2120" value="2120">
                        <input type="hidden" name="prodNomeSimples52" id="MOSTARDA" value="MOSTARDA">
                        <input type="hidden" name="pro_percaptamaxima52" id="200" value="200">
                        <input type="hidden" name="pro_percaptamaximaSap52" id="200" value="200">
                        <input type="hidden" name="uni_nome52" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd52" id="200" value="200">
                        <input type="hidden" name="cod_52" id="113111" value="113111">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            108512 -  PACOCA TIPO CASEIRA 250 GRAMAS 250 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_53" onchange="subtot(document.formCompra.qtde_53,formCompra.preco_53,formCompra.limite_53,formCompra.subtotal_53,document.getElementById('subtotald_53'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_53" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_53" size="4" value="3.68">
                            R$ 3.68                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_53" id="subtotald_53" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_53" name="subtotal_53" size="4">
                        </td>

                        <input type="hidden" name="codfor_53" id="2737" value="2737">
                        <input type="hidden" name="codP_id53" id="2122" value="2122">
                        <input type="hidden" name="prodNomeSimples53" id="PACOCA" value="PACOCA">
                        <input type="hidden" name="pro_percaptamaxima53" id="500" value="500">
                        <input type="hidden" name="pro_percaptamaximaSap53" id="500" value="500">
                        <input type="hidden" name="uni_nome53" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd53" id="250" value="250">
                        <input type="hidden" name="cod_53" id="108512" value="108512">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            134356 -  PAO DE FORMA PANCO  1 PACOTE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_54" onchange="subtot(document.formCompra.qtde_54,formCompra.preco_54,formCompra.limite_54,formCompra.subtotal_54,document.getElementById('subtotald_54'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_54" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_54" size="4" value="8.46">
                            R$ 8.46                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_54" id="subtotald_54" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_54" name="subtotal_54" size="4">
                        </td>

                        <input type="hidden" name="codfor_54" id="1232" value="1232">
                        <input type="hidden" name="codP_id54" id="2128" value="2128">
                        <input type="hidden" name="prodNomeSimples54" id="PAO DE FORMA" value="PAO DE FORMA">
                        <input type="hidden" name="pro_percaptamaxima54" id="2" value="2">
                        <input type="hidden" name="pro_percaptamaximaSap54" id="4" value="4">
                        <input type="hidden" name="uni_nome54" id="PACOTE" value="PACOTE">
                        <input type="hidden" name="proUniQtd54" id="1" value="1">
                        <input type="hidden" name="cod_54" id="134356" value="134356">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            121817 -  PAPEL HIGIENICO (ROLO) FOLHA DUPLA 4 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_55" onchange="subtot(document.formCompra.qtde_55,formCompra.preco_55,formCompra.limite_55,formCompra.subtotal_55,document.getElementById('subtotald_55'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_55" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_55" size="4" value="5.96">
                            R$ 5.96                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_55" id="subtotald_55" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_55" name="subtotal_55" size="4">
                        </td>

                        <input type="hidden" name="codfor_55" id="2737" value="2737">
                        <input type="hidden" name="codP_id55" id="2129" value="2129">
                        <input type="hidden" name="prodNomeSimples55" id="PAPEL HIGIENICO (ROLO)" value="PAPEL HIGIENICO (ROLO)">
                        <input type="hidden" name="pro_percaptamaxima55" id="8" value="8">
                        <input type="hidden" name="pro_percaptamaximaSap55" id="32" value="32">
                        <input type="hidden" name="uni_nome55" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd55" id="4" value="4">
                        <input type="hidden" name="cod_55" id="121817" value="121817">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            103944 -  PAPEL PARA FUMO (FOLHAS) PACOTE 50 FOLHAS 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_56" onchange="subtot(document.formCompra.qtde_56,formCompra.preco_56,formCompra.limite_56,formCompra.subtotal_56,document.getElementById('subtotald_56'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_56" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_56" size="4" value="0.89">
                            R$ 0.89                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_56" id="subtotald_56" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_56" name="subtotal_56" size="4">
                        </td>

                        <input type="hidden" name="codfor_56" id="1232" value="1232">
                        <input type="hidden" name="codP_id56" id="2130" value="2130">
                        <input type="hidden" name="prodNomeSimples56" id="PAPEL PARA FUMO (FOLHAS)" value="PAPEL PARA FUMO (FOLHAS)">
                        <input type="hidden" name="pro_percaptamaxima56" id="2" value="2">
                        <input type="hidden" name="pro_percaptamaximaSap56" id="250" value="250">
                        <input type="hidden" name="uni_nome56" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd56" id="1" value="1">
                        <input type="hidden" name="cod_56" id="103944" value="103944">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            135640 -  PRENDEDOR DE ROUPA  DE PLASTICO S/ METAL 12 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_57" onchange="subtot(document.formCompra.qtde_57,formCompra.preco_57,formCompra.limite_57,formCompra.subtotal_57,document.getElementById('subtotald_57'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_57" size="4" value="2">
                            2                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_57" size="4" value="7.50">
                            R$ 7.50                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_57" id="subtotald_57" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_57" name="subtotal_57" size="4">
                        </td>

                        <input type="hidden" name="codfor_57" id="987" value="987">
                        <input type="hidden" name="codP_id57" id="2134" value="2134">
                        <input type="hidden" name="prodNomeSimples57" id="PRENDEDOR DE ROUPA " value="PRENDEDOR DE ROUPA ">
                        <input type="hidden" name="pro_percaptamaxima57" id="24" value="24">
                        <input type="hidden" name="pro_percaptamaximaSap57" id="24" value="24">
                        <input type="hidden" name="uni_nome57" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd57" id="12" value="12">
                        <input type="hidden" name="cod_57" id="135640" value="135640">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            135645 -  REFRIGERANTE VENCETEX 2L 2000 MILILITRO                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_58" onchange="subtot(document.formCompra.qtde_58,formCompra.preco_58,formCompra.limite_58,formCompra.subtotal_58,document.getElementById('subtotald_58'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_58" size="4" value="4">
                            4                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_58" size="4" value="4.48">
                            R$ 4.48                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_58" id="subtotald_58" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_58" name="subtotal_58" size="4">
                        </td>

                        <input type="hidden" name="codfor_58" id="1232" value="1232">
                        <input type="hidden" name="codP_id58" id="2139" value="2139">
                        <input type="hidden" name="prodNomeSimples58" id="REFRIGERANTE" value="REFRIGERANTE">
                        <input type="hidden" name="pro_percaptamaxima58" id="8000" value="8000">
                        <input type="hidden" name="pro_percaptamaximaSap58" id="12000" value="12000">
                        <input type="hidden" name="uni_nome58" id="MILILITRO" value="MILILITRO">
                        <input type="hidden" name="proUniQtd58" id="2000" value="2000">
                        <input type="hidden" name="cod_58" id="135645" value="135645">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            121818 -  REPELENTE LIQUIDO CREME  100 MILILITRO                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_59" onchange="subtot(document.formCompra.qtde_59,formCompra.preco_59,formCompra.limite_59,formCompra.subtotal_59,document.getElementById('subtotald_59'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_59" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_59" size="4" value="19.00">
                            R$ 19.00                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_59" id="subtotald_59" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_59" name="subtotal_59" size="4">
                        </td>

                        <input type="hidden" name="codfor_59" id="987" value="987">
                        <input type="hidden" name="codP_id59" id="2142" value="2142">
                        <input type="hidden" name="prodNomeSimples59" id="REPELENTE LIQUIDO" value="REPELENTE LIQUIDO">
                        <input type="hidden" name="pro_percaptamaxima59" id="100" value="100">
                        <input type="hidden" name="pro_percaptamaximaSap59" id="100" value="100">
                        <input type="hidden" name="uni_nome59" id="MILILITRO" value="MILILITRO">
                        <input type="hidden" name="proUniQtd59" id="100" value="100">
                        <input type="hidden" name="cod_59" id="121818" value="121818">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            134371 -  RODO PARA LIMPEZA SEM CABO 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_60" onchange="subtot(document.formCompra.qtde_60,formCompra.preco_60,formCompra.limite_60,formCompra.subtotal_60,document.getElementById('subtotald_60'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_60" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_60" size="4" value="7.90">
                            R$ 7.90                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_60" id="subtotald_60" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_60" name="subtotal_60" size="4">
                        </td>

                        <input type="hidden" name="codfor_60" id="987" value="987">
                        <input type="hidden" name="codP_id60" id="2144" value="2144">
                        <input type="hidden" name="prodNomeSimples60" id="RODO PARA LIMPEZA" value="RODO PARA LIMPEZA">
                        <input type="hidden" name="pro_percaptamaxima60" id="1" value="1">
                        <input type="hidden" name="pro_percaptamaximaSap60" id="1" value="1">
                        <input type="hidden" name="uni_nome60" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd60" id="1" value="1">
                        <input type="hidden" name="cod_60" id="134371" value="134371">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            132554 -  SABAO EM BARRA YPE NEUTRO 160g	 160 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_61" onchange="subtot(document.formCompra.qtde_61,formCompra.preco_61,formCompra.limite_61,formCompra.subtotal_61,document.getElementById('subtotald_61'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_61" size="4" value="5">
                            5                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_61" size="4" value="2.06">
                            R$ 2.06                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_61" id="subtotald_61" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_61" name="subtotal_61" size="4">
                        </td>

                        <input type="hidden" name="codfor_61" id="1232" value="1232">
                        <input type="hidden" name="codP_id61" id="2145" value="2145">
                        <input type="hidden" name="prodNomeSimples61" id="SABAO EM BARRA" value="SABAO EM BARRA">
                        <input type="hidden" name="pro_percaptamaxima61" id="800" value="800">
                        <input type="hidden" name="pro_percaptamaximaSap61" id="1000" value="1000">
                        <input type="hidden" name="uni_nome61" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd61" id="160" value="160">
                        <input type="hidden" name="cod_61" id="132554" value="132554">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            116205 -  SABAO EM PO SURF 800 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_62" onchange="subtot(document.formCompra.qtde_62,formCompra.preco_62,formCompra.limite_62,formCompra.subtotal_62,document.getElementById('subtotald_62'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_62" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_62" size="4" value="7.46">
                            R$ 7.46                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_62" id="subtotald_62" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_62" name="subtotal_62" size="4">
                        </td>

                        <input type="hidden" name="codfor_62" id="2737" value="2737">
                        <input type="hidden" name="codP_id62" id="2146" value="2146">
                        <input type="hidden" name="prodNomeSimples62" id="SABAO EM PO" value="SABAO EM PO">
                        <input type="hidden" name="pro_percaptamaxima62" id="800" value="800">
                        <input type="hidden" name="pro_percaptamaximaSap62" id="1000" value="1000">
                        <input type="hidden" name="uni_nome62" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd62" id="800" value="800">
                        <input type="hidden" name="cod_62" id="116205" value="116205">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            115585 -  SABONETE PROTEX 85 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_63" onchange="subtot(document.formCompra.qtde_63,formCompra.preco_63,formCompra.limite_63,formCompra.subtotal_63,document.getElementById('subtotald_63'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_63" size="4" value="8">
                            8                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_63" size="4" value="2.92">
                            R$ 2.92                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_63" id="subtotald_63" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_63" name="subtotal_63" size="4">
                        </td>

                        <input type="hidden" name="codfor_63" id="2737" value="2737">
                        <input type="hidden" name="codP_id63" id="2148" value="2148">
                        <input type="hidden" name="prodNomeSimples63" id="SABONETE" value="SABONETE">
                        <input type="hidden" name="pro_percaptamaxima63" id="680" value="680">
                        <input type="hidden" name="pro_percaptamaximaSap63" id="720" value="720">
                        <input type="hidden" name="uni_nome63" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd63" id="85" value="85">
                        <input type="hidden" name="cod_63" id="115585" value="115585">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            114829 -  SELO PARA CARTA 1 PORTE COMERCIAL - LISTA 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_64" onchange="subtot(document.formCompra.qtde_64,formCompra.preco_64,formCompra.limite_64,formCompra.subtotal_64,document.getElementById('subtotald_64'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_64" size="4" value="42">
                            42                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_64" size="4" value="4.39">
                            R$ 4.39                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_64" id="subtotald_64" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_64" name="subtotal_64" size="4">
                        </td>

                        <input type="hidden" name="codfor_64" id="1232" value="1232">
                        <input type="hidden" name="codP_id64" id="2152" value="2152">
                        <input type="hidden" name="prodNomeSimples64" id="SELO PARA CARTA" value="SELO PARA CARTA">
                        <input type="hidden" name="pro_percaptamaxima64" id="42" value="42">
                        <input type="hidden" name="pro_percaptamaximaSap64" id="42" value="42">
                        <input type="hidden" name="uni_nome64" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd64" id="1" value="1">
                        <input type="hidden" name="cod_64" id="114829" value="114829">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            115586 -  SHAMPOO PARA CABELO DARLING 2 EM 1 350 MILILITRO                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_65" onchange="subtot(document.formCompra.qtde_65,formCompra.preco_65,formCompra.limite_65,formCompra.subtotal_65,document.getElementById('subtotald_65'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_65" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_65" size="4" value="8.98">
                            R$ 8.98                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_65" id="subtotald_65" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_65" name="subtotal_65" size="4">
                        </td>

                        <input type="hidden" name="codfor_65" id="1232" value="1232">
                        <input type="hidden" name="codP_id65" id="2153" value="2153">
                        <input type="hidden" name="prodNomeSimples65" id="SHAMPOO PARA CABELO" value="SHAMPOO PARA CABELO">
                        <input type="hidden" name="pro_percaptamaxima65" id="350" value="350">
                        <input type="hidden" name="pro_percaptamaximaSap65" id="400" value="400">
                        <input type="hidden" name="uni_nome65" id="MILILITRO" value="MILILITRO">
                        <input type="hidden" name="proUniQtd65" id="350" value="350">
                        <input type="hidden" name="cod_65" id="115586" value="115586">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            111253 -  SUCO EM PO TANG SABORES C/ 18 UNID. 324 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_66" onchange="subtot(document.formCompra.qtde_66,formCompra.preco_66,formCompra.limite_66,formCompra.subtotal_66,document.getElementById('subtotald_66'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_66" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_66" size="4" value="15.95">
                            R$ 15.95                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_66" id="subtotald_66" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_66" name="subtotal_66" size="4">
                        </td>

                        <input type="hidden" name="codfor_66" id="1232" value="1232">
                        <input type="hidden" name="codP_id66" id="2155" value="2155">
                        <input type="hidden" name="prodNomeSimples66" id="SUCO EM PO" value="SUCO EM PO">
                        <input type="hidden" name="pro_percaptamaxima66" id="324" value="324">
                        <input type="hidden" name="pro_percaptamaximaSap66" id="500" value="500">
                        <input type="hidden" name="uni_nome66" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd66" id="324" value="324">
                        <input type="hidden" name="cod_66" id="111253" value="111253">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            116557 -  TEMPERO PRONTO PARA SALADA SAZON - SABORES 60 GRAMAS                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_67" onchange="subtot(document.formCompra.qtde_67,formCompra.preco_67,formCompra.limite_67,formCompra.subtotal_67,document.getElementById('subtotald_67'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_67" size="4" value="5">
                            5                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_67" size="4" value="4.58">
                            R$ 4.58                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_67" id="subtotald_67" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_67" name="subtotal_67" size="4">
                        </td>

                        <input type="hidden" name="codfor_67" id="1232" value="1232">
                        <input type="hidden" name="codP_id67" id="2157" value="2157">
                        <input type="hidden" name="prodNomeSimples67" id="TEMPERO PRONTO PARA SALADA" value="TEMPERO PRONTO PARA SALADA">
                        <input type="hidden" name="pro_percaptamaxima67" id="300" value="300">
                        <input type="hidden" name="pro_percaptamaximaSap67" id="400" value="400">
                        <input type="hidden" name="uni_nome67" id="GRAMAS" value="GRAMAS">
                        <input type="hidden" name="proUniQtd67" id="60" value="60">
                        <input type="hidden" name="cod_67" id="116557" value="116557">

                        </tr>
                                            <tr class="prod-row">
                        
                        
                        <td style="text-align: right;">
                            134372 -  VASSOURA DE LIMPEZA SEM CABO 1 UNIDADE                         </td>

                        <td style="text-align: center;">
                            <input tabindex="2" style="text-align: center;" type="text" class="js-qtde" name="qtde_68" onchange="subtot(document.formCompra.qtde_68,formCompra.preco_68,formCompra.limite_68,formCompra.subtotal_68,document.getElementById('subtotald_68'))" size="4" onkeypress="if((event.keyCode &gt;= 48) &amp;&amp; (event.keyCode &lt;= 57)){} else{event.returnValue=false; }">
                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="limite_68" size="4" value="1">
                            1                        </td>

                        <td style="text-align: center;">
                            <input type="hidden" name="preco_68" size="4" value="5.58">
                            R$ 5.58                        </td>

                        <td style="text-align: center;">
                            <div name="subtotald_68" id="subtotald_68" bis_skin_checked="1"></div>
                            <input type="hidden" id="subtotal_68" name="subtotal_68" size="4">
                        </td>

                        <input type="hidden" name="codfor_68" id="1232" value="1232">
                        <input type="hidden" name="codP_id68" id="2164" value="2164">
                        <input type="hidden" name="prodNomeSimples68" id="VASSOURA DE LIMPEZA" value="VASSOURA DE LIMPEZA">
                        <input type="hidden" name="pro_percaptamaxima68" id="1" value="1">
                        <input type="hidden" name="pro_percaptamaximaSap68" id="1" value="1">
                        <input type="hidden" name="uni_nome68" id="UNIDADE" value="UNIDADE">
                        <input type="hidden" name="proUniQtd68" id="1" value="1">
                        <input type="hidden" name="cod_68" id="134372" value="134372">

                        </tr>
                    <input type="hidden" name="total" value="68">
            </tbody></table>,

5 - após cadastro assistido dos itens - clicar em 'Cadastrar' no botão: /html/body/div/div[3]/div[2]/div[1]/div/div[2]/div/form/div[4]/input
6 - seguir com o Loop para a proxima compra

Obs: será adicionado atalhos e informações via JS
