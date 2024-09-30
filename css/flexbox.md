## Flex Display 
If you use the diplay of flex in a container this will be displayed in columns and you can use the gap property to set the gap between the columns. 

``` .container {display: flex; gap: 10px;} ```

### display: inline-flex;
- This allows you to only ocupy the content it needs. It means it also allows for more content to be placed. Otherwise if you use ``` display: flex; ``` this will ocupy 100% width of the page like a block 

![alt image shows``` display: flex; ```](img/displayflex.png)

----

## Flex-Direction 

### flex-direction: row; 
- What is flex-direction? This will be set to "row " - by default - from left to right on the main - axis 

### flex-direction: column;
- This will make all the items inside the flex container line up from top to bottom - we changed the main axis and the cross axis is now left to right

### Flex-basis: 100px;
- If you use the ``` flex-basis: 100px; ``` this will expand it along the axisif this is applied on  ``` flex-direction: column;```
- If you set the ``` flex-basis: 100px; ``` to ``` flex-direction: row;``` then the main axis is across, then it will set the width not the height inside the container. 

