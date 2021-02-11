Flexbox Tutorial
=
Working through flexbox to learn more CSS techniques.  Documenting so they are easy to see how they work.





## WHY!?
----
Because I suck at CSS and really need to improve my front end styling!





## Table of Context
---
[Control](#control)  
[Flex](#flex)  
[Flex-Direction](#flex-direction)  
[Column](#column)  
[Justify-Content](#justify-content)  
[Align Items](#align-items)






## Control
---
This is the starting code without flex added.  For the Rest I will only be adding flex-box CSS Snippets Unless I change the HTML(which I will include if I do.).



### HTML
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="./assets/style.css">

    <title>Flex Box Tutorial</title>
</head>
<body>

    <div class="container">

        <div class="item">1. First</div>
        <div class="item">2. Second</div>
        <div class="item">3. Third</div>
        <div class="item">4. Fourth</div>
        <div class="item">5. Last</div>

    </div>

</body>
</html>
```


### CSS
```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.container {
    background-color: #ccc;
    padding: 10px;
}

.item {
    background-color: maroon;
    padding: 30px;
    margin: 30px;
    color: #fff;
    font-size: 40px;
}
```



### This Is The Output of the Control
![control image](/assets/img/control.png)




## **Flex**  
-----
This is achieved by just adding ```display: flex;``` onto the ```.container``` class.
The flex items are set inside of the container side by side.



### CSS
```css
.container {
    background-color: #ccc;
    padding: 10px;

//////////////////////////    <
    display: flex;          <---------
//////////////////////////    <

}

```



### This Is The Output
![control image](/assets/img/display-flex.png)



## Flex-Direction  
-----
Flex Direction will can alter the direction the ITEMS are aligned in a flex container.  

This can be achieved either in a row or in a column.  



## Flex-Direction - Row  
----
```flex-direction: row;``` is default.  and will give you the same output as the output above ^



## Flex-Direction - Row-Reverse
----
But ```flex-direction: row-reverse;``` will reverse the order of those ITEMS.



### CSS
```css
.container {
    background-color: #ccc;
    padding: 10px;

//////////////////////////    
    display: flex;                    <
    flex-direction: row-reverse;    <---------
//////////////////////////            <
}
```


### This Is The Output  
Notice the ITEMS in the container are reversed order.
![flex-direction row-reverse](/assets/img/flex-direction-row-reverse.png)



## Column
-----
```css
.container {
    background-color: #ccc;
    padding: 10px;

//////////////////////////    
    display: flex;                <
    flex-direction: column;     <---------------
//////////////////////////        <
}
```


### This Is The Output  
Looks rather similar to the control... but take a look below at what you can do to the ITEMS inside.

![flex-direction row-reverse](/assets/img/flex-direction-column.png)
Notice the ITEMS in the container set in a column almost like the Control but with the ability to do this...



## Column-Reverse
-----
```css
.container {
    background-color: #ccc;
    padding: 10px;

//////////////////////////    
    display: flex;                     <
    flex-direction: column-reverse;  <---------------
//////////////////////////             <
}
```



### This Is The Output  
Looks rather similar to the control... but take a look below at what you can do to the ITEMS inside.

![flex-direction row-reverse](/assets/img/flex-direction-column-reverse.png)  



## Justify-Content  
------
```justify-content``` is another great tool of flexbox.  It allows us to control the ITEMS or "content" of the container.  



## Justify-Content - Center  
------
```justify-content: center;``` Does kinda what you would expect by now through this tutorial... It puts the content in the center of the container.  
```css
.container {
    background-color: #ccc;
    padding: 10px;

////////////////////////////
    display: flex;
    flex-direction: row;          <
    justify-content: center;    <-------
////////////////////////////      <
}                                 
```



### This Is The Output  
* TAKE NOTE!  The only reason there is space between the ITEMS is because of the margin on the "item" class
![Justify-Content Center](/assets/img/justify-content-center.png)  



## Justify-Content - Space Between  
------
```justify-content: space-between;``` Put space in between each of the ITEMS in the container.  
```css
.container {
    background-color: #ccc;
    padding: 10px;

////////////////////////////
    display: flex;
    flex-direction: row;                 <
    justify-content: space-between;    <-------
////////////////////////////             <
}                                 
```



### This Is The Output  
* TAKE NOTE!  The only reason there is space by the 1st and last ITEMS is because of the margin on the "item" class once again.
![Justify-Content Space Between](/assets/img/justify-content-space-between.png)  



## Justify-Content - Space Around  
------
```justify-content: space-around;``` Put an even amount of space on the left and right side of each of the flex ITEMS.  
```css
.container {
    background-color: #ccc;
    padding: 10px;

////////////////////////////
    display: flex;
    flex-direction: row;                 <
    justify-content: space-around;    <-------
////////////////////////////             <
}                                 
```



### This Is The Output  
* TAKE NOTE!  The difference is a little hard to see because of the margin but notice the extra spacing at the 1st and last.
![Justify-Content Space Between](/assets/img/justify-content-space-around.png)  



## Justify-Content - Space Evenly  
------
```justify-content: space-evenly;``` Put space in between each of the ITEMS in the container EVENLY.  
```css
.container {
    background-color: #ccc;
    padding: 10px;

////////////////////////////
    display: flex;
    flex-direction: row;                 <
    justify-content: space-evenly;    <-------
////////////////////////////             <
}                                 
```



### This Is The Output  
* TAKE NOTE!  The only reason there is space by the 1st and last ITEMS is because of the margin on the "item" class once again.
![Justify-Content Space Between](/assets/img/justify-content-space-evenly.png)  



## Justify-Content - Flex Start  
------
```justify-content: flexs-start;``` Aligns the ITEMS at the start of the container Main Axis.  
```css
.container {
    background-color: #ccc;
    padding: 10px;

////////////////////////////
    display: flex;
    flex-direction: row;                 <
    justify-content: flex-start;    <-------
////////////////////////////             <
}                                 
```



### This Is The Output  
* TAKE NOTE!  The only reason there is space by the 1st and last ITEMS is because of the margin on the "item" class once again.
![Justify-Content Flex Start](/assets/img/justify-content-flex-start.png)  



## Justify-Content - Flex End  
------
```justify-content: flex-end;``` Put space in between each of the ITEMS in the container.  
```css
.container {
    background-color: #ccc;
    padding: 10px;

////////////////////////////
    display: flex;
    flex-direction: row;                 <
    justify-content: flex-end;    <-------
////////////////////////////             <
}                                 
```



### This Is The Output  
* TAKE NOTE!  The only reason there is space by the 1st and last ITEMS is because of the margin on the "item" class once again.
![Justify-Content Flex End](/assets/img/justify-content-flex-end.png)  




## Align Items
----
Align Items determines how the items inside the container are aligned.  
For this one I needed to have uneven sized items inside the container so I altered the HTML slightly and added extra classes to 2 and 4.  



## Align Items Center
---
Lets start with ```align-items: center;``` 
* TAKE NOTE - I changed some of the HTML by adding new classes. and some css to change the styling of those 2 ITEMS.

```html
    <div class="container">

        <div class="item">1. First</div>
        <div class="item i2">2. Second</div> <---------  I added class i2
        <div class="item">3. Third</div>
        <div class="item i4">4. Fourth</div> <---------  I added class i4 
        <div class="item">5. Last</div>

    </div>
```
```css
.container {
    background-color: #ccc;
    padding: 10px;

    display: flex;
    flex-direction: row;
    justify-content: center;    <
    align-items: center;      <---------  Also Notice this new property  ;-)  What do you think it does? Let's see..
}                               <

.i2,
.i4 {                 <
    height: 200px   <---------  And gave them a height of 200px
}                     <
```



### This Is The Output  
![Align Items Center](/assets/img/align-items-center.png)  



## Align Items Flex Start
---
```align-items: flex-start;``` makes the content begin at the "start" of the top of the container.
```css
.container {
    background-color: #ccc;
    padding: 10px;

    display: flex;
    flex-direction: row;
    justify-content: center;        <
    align-items: flex-start;      <---------  
}                                   <         
```



### This Is The Output  
![Align Items Flex Start](/assets/img/align-items-flex-start.png)  



## Align Items Flex End
---
```align-items: flex-end;``` makes the content begin at the "end" of the top of the container.
```css
.container {
    background-color: #ccc;
    padding: 10px;

    display: flex;
    flex-direction: row;
    justify-content: center;      <
    align-items: flex-end;      <---------  
}                                 <

```



### This Is The Output  
![Align Items Flex End](/assets/img/align-items-flex-end.png)  



## Align Items Stretch
---
```align-items: stretch;``` stretches all the ITEMS to fill the container.
```css
.container {
    background-color: #ccc;
    padding: 10px;

    display: flex;
    flex-direction: row;
    justify-content: center;    <
    align-items: stretch;      <---------
}                               <
```



### This Is The Output  
![Align Items Stretch](/assets/img/align-items-stretch.png)  



## Align Items Baseline
---
```align-items: baseline;``` aligns the contents by the bottom of the font.
```css
.container {
    background-color: #ccc;
    padding: 10px;

    display: flex;
    flex-direction: row;
    justify-content: center;      <
    align-items: baseline;      <---------
}                                 <
```



### This Is The Output  
![Align Items Baseline](/assets/img/align-items-baseline.png)  