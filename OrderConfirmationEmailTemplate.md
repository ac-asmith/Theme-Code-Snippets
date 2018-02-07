## Customer Order Item Layout Table
*Add or remove merge order item layout merge codes as needed.* 
```
<table cellpadding="10" border="1">
   <thead>
      <tr>
         <th><h3>SKU</h3></th>
         <th><h3>Item </h3></th>
         <th><h3>Details</h3></th>
         <th><h3>Qty</h3></th>
         <th><h3>Price</h3></th>
         <th><h3>Total</h3></th>
      </tr>
   </thead>
<tbody>
   <!--ORDERITEMLAYOUTSTART-->
      <tr>
         <td>##ITEMNR##</td>
         <td>##ITEMNAME##</td>
         <td>##ITEMDESC##</td>
         <td>##QTY##</td>
         <td>##ITEMPRICE##</td>
         <td>##ITEMTOTAL##</td>
      </tr>
      <!--ORDERITEMLAYOUTEND-->
</table>
```
