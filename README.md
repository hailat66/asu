<HTML>
    <HEAD>
    <TITLE>Order Pizza</TITLE>
    </HEAD>
    <BODY>
          
<TABLE>
    <TR><TD>Pizza</TD>
    <TD>Toppings</TD>
    <TD>Quantity</TD>
    <TD>Order Day</TD>
    </TR>
    <TR><TD>Neil Daswani</TD>
    <TD>1234 1234 9999 1111</TD>
    <TD>11</TD>
    <TD>2007</TD>
    </TR>
    <TR><TD>Christoph Kern</TD>
    <TD>1234 4321 3333 2222</TD>
    <TD>4</TD>
    <TD>2008</TD>
    </TR>
    <TR><TD>Anita Kesavan</TD>
    <TD>2354 7777 1111 1234</TD>
    <TD>3</TD>
    <TD>2007</TD>
    </TR>
    ...
    </TABLE>  
    
    <FORM ACTION="submit_order" METHOD="GET" NAME="f">
    How many pizzas would you like to order?
  
    <INPUT TYPE="text" NAME="qty" VALUE="1" onKeyUp="computePrice();">
    <INPUT TYPE="hidden" NAME="price" VALUE="5.50"><BR>
    <INPUT TYPE="submit" NAME ="Order" VALUE="Pay">
    <INPUT TYPE="submit" NAME ="Cancel" VALUE="Cancel">
    <SCRIPT>
    function computePrice() {
    f.price.value = 5.50 * f.qty.value;
    f.Order.value = "Pay $" + f.price.value
 

}
    </SCRIPT>
    </BODY>
    </HTML>
