# Web Developer

## Part 1 : Front End

### 1.1 Basic CSS
Provide an HTML/CSS that can explain the difference between an id and a class.

In CSS, How would you select `{:.html}<div data-id=’2’>Dog</div>` using the data attribute?

### 1.2 Format Date
Write a javascript (native) that will format a date from `M/D/YYYY` to `YYYYMMDD`.

```javascript
function formatDate(userDate) {
  // @todo format from M/D/YYYY to YYYYMMDD
}
```
```javascript
console.log(formatDate("12/31/2014")); // should return: 20141231
```

### 1.3 CSS Selectors
Describe the difference between the ff:

```css
div.firstclass > .secondclass {}
div.firstclass.secondclass {}
div.firstclass, .secondclass {}
```

### 1.4 HTML Select Tags
Create two (2) select tags with the following options:

```
1st select - Color, Animal, Car
2nd select - Red, Green, Dog, Cat, Rabbit, Mouse, Porsche
```

### 1.5 JS - Select Tags
_Refer to `1.4`_

Create a script to group the second select tag when the first tag changes selection.

Example: When `"Animal"` is selected, the second select tag should only contain the options: `Dog, Cat, Rabbit and Mouse`.

You may use `jQuery`.

### 1.5 JS - Delete Image
An image gallery has a list of images with a remove button labeled `X`. Write a script (jQuery) that will delete the image in the gallery when the `X` button is clicked.

```html
<div class="image">
  <img src="image1.jpg" alt="First">
  <button class="remove">X</button>
</div>
<div class="image">
  <img src="image2.jpg" alt="Second">
  <button class="remove">X</button>
</div>
```

## Part 2 : Back End

### 2.1 Student Class

A `Student` class has the following attributes: `name`, `section`, `grade`. If there is an array of `$students`:

```php
$students = [
	//StudentClass Object #1
	,
	//StudentClass Object #2
	,
	//StudentClass Object #3
	,
	//StudentClass Object #4
	,
);
```

Write a PHP script to display the name, section and grade of the `third object` in the `$students` array.

### 2.2 Fruits

Below is an example of a data structure that defines a fruit’s color:
```php
array(
  "red" => array("apple, strawberry"),
  "yellow" => array("lemon", "ripe mango")
)
```

Implement the function getFruits, which accepts color as a string parameter and returns all fruits for that color in JSON format (see example below).

For example, the call $fruitcolors>getFruits("red") should return:
```json
{ "color":"red", "fruits": ["apple", "strawberry"]}
```

If a call doesn’t have fruits for that $fruitcolors>getFruits("violet") color, it should return:
```json
{ "color":"violet", "fruits":[] }
```

```php
<?php
class FruitColor
{
  private $fruitcolor;

  function FruitColor($fruitcolor)
  {
    $this->fruitcolor = $fruitcolor;
  }

  public function getFruits($color)
  {
    // @todo: implement here
    return NULL;
  }
}

$fruitcolor = new FruitColor(array(
	"red" => array("apple", “strawberry”),
	"yellow" => array("lemon", "ripe mango")
));

echo $fruitcolor->getFruits("red");
echo "\n";
echo $fruitcolor->getFruits("violet");

```

### 2.3 Group by Color

Implement a groupByColor function that:

- Accepts an associative array containing the color for each fruit.
- Returns an associative array containing an array of fruits for each color, in any order.

For example, for associative array `["Ripe Mango" => "Yellow", "Strawberry" => "Red", "Lemon" => "Yellow"]` the groupByColor function should return `["Yellow" => ["Ripe Mango", "Lemon"], "Red" => ["Strawberry"]]`.


### 2.4 SQL

![Tables](https://raw.githubusercontent.com/BrewedLogic/self-assessment/master/tables-2.4.png)

Write an SQL statement that returns:
1. List of all students with their course description and total tuition fee `(units * price_per_unit)` based from their course
2. The name of the student with the most expensive tuition fee
3. Average tuition fee of the course with 15 units or more

## Part 3 : Self-Assessment

_Use Google form_

**Rating (1-10 1-lowest 10-highest)**
