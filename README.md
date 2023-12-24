**适用于所有EVM链**



**依赖:**
pip install web3
pip install httpx




**使用教程** 
输入地址：这是你接收铭文的地址
输入私钥：付gas账号私钥
输入RPC：打哪个链用哪个链的RPC，有的RPC不支持batchRequest，多换几个
输入是否EIP1559：1159就是输入最大gasPrice，小费gasPrice那种，非1159就是直接输入gasPrice
输入gasPrice：就是gasPrice
输入maxFeePerGas：这个是最大gasPrice，可以多给点
输入maxPriorityFeePerGas：这个是小费gasPrice
输入data：支持直接复制铭文文本，或者十六进制（必须0x开头）


**其它说明**
输入的私钥账号可以和接收铭文账号不是同一个，也可以是同一个。不同就是小号给大号打，相同就是自转

请尽量不要使用大号私钥打，请为每个项目专门搞个小号，不论是直接双压卖私钥，还是卡交易都好处理

一包100个，循环100次，理论上是会跑10000个，但是实际上会卡nonce，多跑几遍就是
