# DSCP and Precedence Values
Первоисточник:
https://www.cisco.com/c/en/us/td/docs/switches/datacenter/nexus1000/sw/4_0_4_s_v_1_3/qos/configuration/guide/n1000v_qos/n1000v_qos_6dscpval.html

This appendix provides the DSCP and precedence values used in QoS class maps and policy maps.

## Commonly Used DSCP Values
Unless noted as a restriction, you can mark both incoming and outgoing packets.

Table 6-1 lists the commonly used DSCP values that are described in RFC 2475 http://www.ietf.org/rfc/rfc2475.txt.


<table border="1" cellpadding="3" cellspacing="0" width="96%" bordercolor="#808080"> 
    <caption> 
     <p class="pTC_TableCap"> <a name="pgfId-1111851"></a>Table 6-1 <a name="47900"></a>Commonly Used DSCP Values </p> 
    </caption> 
    <tbody> 
     <tr align="left" valign="top"> 
      <th scope="col"> 
       <section class="pCH1_CellHead1"> 
        <a name="pgfId-1111951"></a>DSCP Value 
       </section> </th> 
      <th scope="col"> 
       <section class="pCH1_CellHead1"> 
        <a name="pgfId-1114034"></a>Decimal Value 
       </section> </th> 
      <th scope="col"> 
       <section class="pCH1_CellHead1"> 
        <a name="pgfId-1112021"></a>Meaning 
       </section> </th> 
      <th scope="col"> 
       <section class="pCH1_CellHead1"> 
        <a name="pgfId-1112254"></a>Drop Probability 
       </section> </th> 
      <th scope="col"> 
       <section class="pCH1_CellHead1"> 
        <a name="pgfId-1111857"></a>Equivalent IP Precedence Value 
       </section> </th> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112123"></a>101 110 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114036"></a>46</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112141"></a>High Priority</p> <p class="pB1_Body1"> <a name="pgfId-1112125"></a>Expedited Forwarding (EF)</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112256"></a>N/A</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112127"></a>101 - Critical</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112324"></a>000 000 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114038"></a>0</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112306"></a>Best Effort</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112308"></a>N/A</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112310"></a>000 - Routine</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111953"></a>001 010 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114040"></a>10</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112073"></a>AF11</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112258"></a>Low</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111861"></a>001 - Priority</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111955"></a>001 100 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114042"></a>12</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112075"></a>AF12</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112260"></a>Medium</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111865"></a>001 - Priority</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111957"></a>001 110 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114044"></a>14</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112077"></a>AF13</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112262"></a>High</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111869"></a>001 - Priority</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111959"></a>010 010 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114046"></a>18</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112079"></a>AF21</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112264"></a>Low</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111873"></a>010 - Immediate</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111961"></a>010 100 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114048"></a>20</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112081"></a>AF22</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112266"></a>Medium</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111877"></a>010 - Immediate</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111963"></a>010 110 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114050"></a>22</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112083"></a>AF23</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112268"></a>High</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111881"></a>010 - Immediate</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111965"></a>011 010 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114052"></a>26</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112085"></a>AF31</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112270"></a>Low</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111885"></a>011 - Flash</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111967"></a>011 100 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114054"></a>28</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112087"></a>AF32</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112272"></a>Medium</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111889"></a>011 - Flash</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111969"></a>011 110 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114056"></a>30</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112089"></a>AF33</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112274"></a>High</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111893"></a>011 - Flash</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111971"></a>100 010 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114058"></a>34</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112091"></a>AF41</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112276"></a>Low</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111897"></a>100 - Flash Override</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111973"></a>100 100 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114060"></a>36</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112093"></a>AF42</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112278"></a>Medium</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111901"></a>100 - Flash Override</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111975"></a>100 110 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114062"></a>38</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112095"></a>AF43</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1112280"></a>High</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1111905"></a>100 - Flash Override</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113618"></a>001 000 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114064"></a>8</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113620"></a>CS1</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113596"></a>&nbsp;</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113598"></a>1</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113622"></a>010 000 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114066"></a>16</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113624"></a>CS2 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113588"></a>&nbsp;</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113590"></a>2</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113626"></a>011 000 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114068"></a>24</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113628"></a>CS3 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113580"></a>&nbsp;</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113582"></a>3</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113630"></a>100 000 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114070"></a>32</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113632"></a>CS4 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113572"></a>&nbsp;</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113574"></a>4</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113634"></a>101 000 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114072"></a>40</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113636"></a>CS5 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113564"></a>&nbsp;</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113566"></a>5</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113638"></a>110 000 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114074"></a>48</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113640"></a>CS6 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113556"></a>&nbsp;</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113558"></a>6</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113642"></a>111 000 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114076"></a>56</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113644"></a>CS7</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113548"></a>&nbsp;</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113550"></a>7</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113646"></a>000 000 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114078"></a>0</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113648"></a>Default </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113540"></a>&nbsp;</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113542"></a>&nbsp;</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113650"></a>101 110 </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1114080"></a>46</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113652"></a>EF </p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113532"></a>&nbsp;</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113534"></a>&nbsp;</p> </td> 
     </tr> 
    </tbody> 
   </table>


## IP Precedence Values
Table 6-2 lists the RFC 791 precedence values from least to most important.


<table border="1" cellpadding="3" cellspacing="0" width="96%" bordercolor="#808080"> 
    <caption> 
     <p class="pTC_TableCap"> <a name="pgfId-1090429"></a>Table 6-2 <a name="21470"></a>Precedence Values </p> 
    </caption> 
    <tbody> 
     <tr align="left" valign="top"> 
      <th scope="col"> 
       <section class="pCH1_CellHead1"> 
        <a name="pgfId-1090433"></a>Value 
       </section> </th> 
      <th scope="col"> 
       <section class="pCH1_CellHead1"> 
        <a name="pgfId-1090435"></a>Description 
       </section> </th> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1090441"></a>000 (0)</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1090443"></a>Routine or Best Effort</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1090445"></a>001 (1)</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1090447"></a>Priority </p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1090449"></a>010 (2)</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1090451"></a>Immediate</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1090453"></a>011 (3)</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1113030"></a>Flash (mainly used for voice signaling or for video)</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1090457"></a>100 (4)</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1090459"></a>Flash Override </p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1090461"></a>101 (5)</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1090463"></a>Critical (mainly used for voice RTP)</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1090465"></a>110 (6)</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1090467"></a>Internet</p> </td> 
     </tr> 
     <tr align="left" valign="top"> 
      <td><p class="pB1_Body1"> <a name="pgfId-1090469"></a>111 (7)</p> </td> 
      <td><p class="pB1_Body1"> <a name="pgfId-1090471"></a>Network </p> </td> 
     </tr> 
    </tbody> 
   </table>