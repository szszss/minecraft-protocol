#聊天信息

默认的服务器会检查消息是否以‘/’开头。若不是，则将发送者的名字添加到消息前并将它发送给所有客户端端（包括发送者自己）。如果是以‘/’开头，服务器将认为它是一个指令并尝试处理它。如果一条消息长度超过100个字符将导致服务器将客户端踢出。这个改动起初是通过允许客户端不切分超过119个字符的消息（以前的限制），但在服务端上并未做改变。因此，原版服务器端保留了在119个字符的位置切分字符串的代码，不过这并不是协议的限制而且这个限制可以被忽略。  
更多信息请参阅[聊天](http://wiki.vg/Chat)。  
<table>
    <tbody>
        <tr>
            <th> 包标识符 </th>
            <th> 类别 </th>
            <th> 绑定到 </th>
            <th> 字段名 </th>
            <th> 字段类型 </th>
            <th> 备注</th>
        </tr>
        <tr>
            <td> 0x01 </td>
            <td> 游戏 </td>
            <td> 服务器端</td>
            <td> 消息 </td>
            <td> String </td>
            <td></td>
        </tr>
    </tbody>
</table>
