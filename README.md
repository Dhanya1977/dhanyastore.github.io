<html>
<body bgcolor="yellow">

<p>Select a new Item from the list.</p>
<form name="rs">
<select id="item" onchange="itm()">
  <option value="Rice">Rice</option>
  <option value="Oil">Oil</option>
  <option value="Paste">Paste</option>
  <option value="Soap">Soap</option>
  <option value="Ponds">Ponds</option>
</select>
<br>
Qty:<br>
<input type="text" id="q"><br>
Rate:<br>
<input type="text" id="r"><br>
Amount:<br>
<input type="text" id="a"><br>
<input type="button" onclick="cal()" value="Calculate"/>  
</form>  

<script>
function itm()
{
 var i = document.getElementById("item").value;

if(i=="Rice")
document.rs.r.value="80";
if(i=="Oil")
document.rs.r.value="145";
if(i=="Soap")
document.rs.r.value="35";
if(i=="Paste")
document.rs.r.value="88";
if(i=="Ponds")
document.rs.r.value="86";
}

function cal()
{  
var q=document.rs.q.value;  
var r=document.rs.r.value;  
var a=q*r;  
document.rs.a.value=a;  
}
</script>  
</body>
</html>


