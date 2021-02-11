# flexbox-tutorial
Working through flexbox to learn more CSS techniques.  Documenting so they are easy to see how they work.

## WHY!?  
Because I suck at CSS and really need to improve my front end styling!

## Table of Context  
[Control](#control)  
[Flex](#flex)

## Control
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
### This Is The Output
![control image](/assets/img/control.png)

## **Flex**  
This is achieved by just adding ```display: flex;``` onto the ```.container``` class.
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

//////////////////////////    <
    display: flex;          <---------
//////////////////////////    <

}

.item {
    background-color: maroon;
    padding: 30px;
    margin: 30px;
    color: #fff;
    font-size: 40px;
}
```
### This Is The Output
![control image](/assets/img/display-flex.png)