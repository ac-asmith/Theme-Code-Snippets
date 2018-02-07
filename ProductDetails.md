
# Product Details



## Add Variant Dropdown to Product Group Table


```html
<ac:visibilityarea id="ProductGroupArea">
      <div id="dvProductGroupGrid">
        <ac:visibilityarea id="ProductGroups">
          <div id="divProductDisplay" class="overflow-x-scroll">
            <table class="ProductGroup table">
              <thead>
                <tr class="ProductGroupHeader no-wrap">
                  <th id="thProductGroupDisplayItemNumber">Item #</th>
                  <th id="thProductGroupDisplayDescription">Description/Size</th>
                  <th id="thProductGroupDisplayAvailability">Availability</th>
                  <th id="thProductGroupDisplayPriceBreaks">Qty Break</th>
                  <th id="thProductGroupDisplayVariant">Variant</th>
                  <th id="thProductGroupDisplayPricing">Price</th>
                  <th id="thProductGroupDisplayQuantity">Quantity</th>
                </tr>
              </thead>
              <ac:layoutarea id="ProductGroupDetail">
                <tr class="ProductGroupItem">
                  <td class="tdProductGroupDisplayItemNumber">$$ITEMNR$$</td>
                  <td class="tdProductGroupDisplayDescription">$$LONGDESCRIPTION$$</td>
                  <td class="tdProductGroupDisplayAvailability">$$AVAILABILITY$$</td>
                  <td class="tdProductGroupDisplayPriceBreaks">$$QTYBREAKS$$</td>
                  <td class="tdProductGroupDisplayVariant">$$VARIANTS$$</td>
                  <td class="tdProductGroupDisplayPricing" style="white-space:nowrap;">$$PRICE$$</td>
                  <td class="tdProductGroupDisplayQuantity">$$QUANTITY$$$$ADDTOCART$$</td>
                </tr>
              </ac:layoutarea>
              <ac:layoutarea id="ProductGroupDetailAlt">
                <tr class="ProductGroupAlternatingItem">
                  <td class="tdProductGroupDisplayAltItemNumber">$$ITEMNR$$</td>
                  <td class="tdProductGroupDisplayAltDescription">$$LONGDESCRIPTION$$</td>
                  <td class="tdProductGroupDisplayAltAvailability">$$AVAILABILITY$$</td>
                  <td class="tdProductGroupDisplayAltPriceBreaks">$$QTYBREAKS$$</td>
                  <td class="tdProductGroupDisplayAltVariant">$$VARIANTS$$</td>
                  <td class="tdProductGroupDisplayAltPricing" style="white-space:nowrap;">$$PRICE$$</td>
                  <td class="tdProductGroupDisplayAltQuantity">$$QUANTITY$$$$ADDTOCART$$</td>
                </tr>
              </ac:layoutarea>
            </table>
            <ac:layoutarea id="ProductGroupVariant">
              <div class="pad-b-10">
                <div class="child-var-group"><strong>$$VARIANTGROUPNAME$$</strong></div>
                $$VARIANTGROUPCONTROLS$$
              </div>
            </ac:layoutarea>
            <ac:layoutarea id="ProductGroupPersonalization">
              <div class="pad-b-10">
                <div class="child-personalization-question"><strong>$$PERSONALIZATIONQUESTION$$</strong></div>
                $$PERSONALIZATIONCONTROLS$$
              </div>
              <ac:visibilityarea id="UpdateGroupPrice">
                <br>
                <div align="right" class="ProductDetailsPricing">
                  $$PRODUCTGROUPTOTAL$$
                </div>
                <div align="right" class="ProductGroupUpdatePrice">
                  $$PRODUCTGROUPUPDATEPRICE$$
                </div>
                <br>
              </ac:visibilityarea>
            </ac:layoutarea></div>
          <div class="right ProductGroupAddToCart">$$PRODUCTGROUPADDTOCARTBUTTON$$</div>
        </ac:visibilityarea>
      </div>
    </ac:visibilityarea>
```

## Add Images to Product Group Table

### HTML:
```html
<table class="ProductGroup table">
  <thead>
    <tr class="ProductGroupHeader no-wrap">
      <th id="thProductGroupDisplayItemNumber">Photo</th>
      <th id="thProductGroupDisplayItemNumber">Item #</th>
      <th id="thProductGroupDisplayDescription">Description/Size</th>
      <th id="thProductGroupDisplayAvailability">Availability</th>
      <th id="thProductGroupDisplayPriceBreaks">Qty Break</th>
      <th id="thProductGroupDisplayPricing">Price</th>
      <th id="thProductGroupDisplayQuantity">Quantity</th>
    </tr>
  </thead>
  <ac:layoutarea id="ProductGroupDetail">
    <tr class="ProductGroupItem">
      <td class="tdProductGroupDisplayItemNumber"><img class="ItemPhoto" src="##ITEMPHOTOURL##"></td>
      <td class="tdProductGroupDisplayItemNumber">$$ITEMNR$$</td>
      <td class="tdProductGroupDisplayDescription">$$LONGDESCRIPTION$$</td>
      <td class="tdProductGroupDisplayAvailability">$$AVAILABILITY$$</td>
      <td class="tdProductGroupDisplayPriceBreaks">$$QTYBREAKS$$</td>
      <td class="tdProductGroupDisplayPricing" style="white-space:nowrap;">$$PRICE$$</td>
      <td class="tdProductGroupDisplayQuantity">$$QUANTITY$$$$ADDTOCART$$</td>
    </tr>
  </ac:layoutarea>
  <ac:layoutarea id="ProductGroupDetailAlt">
    <tr class="ProductGroupAlternatingItem">
      <td class="tdProductGroupDisplayItemNumber"><img class="ItemPhoto" src="##ITEMPHOTOURL##"></td>
      <td class="tdProductGroupDisplayAltItemNumber">$$ITEMNR$$</td>
      <td class="tdProductGroupDisplayAltDescription">$$LONGDESCRIPTION$$</td>
      <td class="tdProductGroupDisplayAltAvailability">$$AVAILABILITY$$</td>
      <td class="tdProductGroupDisplayAltPriceBreaks">$$QTYBREAKS$$</td>
      <td class="tdProductGroupDisplayAltPricing" style="white-space:nowrap;">$$PRICE$$</td>
      <td class="tdProductGroupDisplayAltQuantity">$$QUANTITY$$$$ADDTOCART$$</td>
    </tr>
  </ac:layoutarea>
</table> 
```

### CSS: 
```css
/ * change dimensions as needed */
.ItemPhoto { hieght: 28px; width: 52px; }
```
    
