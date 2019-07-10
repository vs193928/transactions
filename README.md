# transactions
<h2>Demo showing transaction handling in Mule4</h2>

<br/>

<b>db_transactions</b>: This component demonstartes transaction handling while doind db inserts. There are 2 inserts in configuration. There is a error in second insert statement, which forces the roll back of the first insert. Both the inserts are part of single transaction. <br/>
<b>jms_transactions</b>: This component demonstartes transaction handling while reading from jms. To demo, if it reads a string, the flow will error out, will retry 5 more times and then move the message to dead letter queue. If it reads a number, message is processed all good. 
