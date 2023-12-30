##  HTML FORMATTING
```html 
<b> - Bold text
<strong> - Important text
<i> - Italic text
<em> - Emphasized text
<mark> - Marked text
<small> - Smaller text
<del> - Deleted text
<ins> - Inserted text
<sub> - Subscript text
<sup> - Superscript text
```
## Quatitation
```html
<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 60 years, WWF has worked to help people and nature thrive. As the world's leading conservation organization, WWF works in nearly 100 countries. At every level, we collaborate with people around the world to develop and deliver innovative solutions that protect communities, wildlife, and the places in which they live.
</blockquote>

<p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>

<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>

<address>
Written by John Doe.<br>
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>

<p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>

<bdo dir="rtl">This text will be written from right to left</bdo>
```

## IMAGES
```html
<img src="workplace.jpg" alt="Workplace" usemap="#workmap">

<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="computer.htm">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="phone.htm">
  <area shape="circle" coords="337,300,44" alt="Coffee" href="coffee.htm">
</map>

rect - defines a rectangular region
circle - defines a circular region
poly - defines a polygonal region
default - defines the entire region

<picture>
  <source media="(min-width: 650px)" srcset="img_food.jpg">
  <source media="(min-width: 465px)" srcset="img_car.jpg">
  <img src="img_girl.jpg">
</picture>
```
## TABLE

```html
<table>
    <caption>Title Table</caption>
    <thead>
        <tr>
            <th>Person 1</th>
            <th>Person 2</th>
            <th>Person 3</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Emil</td>
            <td>Tobias</td>
            <td>Linus</td>
        </tr>
        <tr>
            <td>16</td>
            <td>14</td>
            <td>10</td>
        </tr>
    </tbody>
</table>
```
```css
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
 th, td {
  border-style: 
  dotted,
  dashed,
  solid,
  double,
  groove,
  ridge,
  inset,
  outset,
  none,
  hidden;
}
```

## LIST
```html
<ul style="list-style-type:disk,circle,square,none">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
<ol type="1,A,a,I,i">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>
```
## COMPUTER CODE
```html
<pre>
    <code>
        x = 5;
        y = 6;
        z = x + y;
    </code>
</pre>
<p>The area of a triangle is: 1/2 x <var>b</var> x <var>h</var> and press <kbd>Ctrl + S</kbd></p>
<p>
    <samp>File not found.<br>Press F1 to continue</samp>
</p>
```

## SEMANTIC
```html
<!DOCTYPE html>
<html>
    <head></head>
    <body>
        <nav></nav>
        <main>
            <header>
                <h1>Title Web</h1>
            </header>
            <article>
                <header>
                    <h2>Google Chrome</h2>
                    <figure>
                        <img src="pic_trulli.jpg" alt="Trulli">
                        <figcaption   figcaption>Fig1. - Trulli, Puglia, Italy.</figcaption>
                    </figure>
                </header>
                <details>
                    <summary>Epcot Center</summary>
                    <p>Google Chrome is a web browser developed by Google, released in 2008. Chrome is the world's most popular web browser today! <time>20:00 WIB</time></p>
                </details>
            </article>
        </main>
        <aside></aside>
        <footer></footer>
    </body>
</html>
```
## FORM

```html
<input>
<label>
<select>
<textarea>
<button>
<fieldset>
<legend>
<datalist>
<output>
<option>
<optgroup>

<input type="button">
<input type="checkbox">
<input type="color">
<input type="date">
<input type="datetime-local">
<input type="email">
<input type="file">
<input type="hidden">
<input type="image">
<input type="month">
<input type="number">
<input type="password">
<input type="radio">
<input type="range">
<input type="reset">
<input type="search">
<input type="submit">
<input type="tel">
<input type="text">
<input type="time">
<input type="url">
<input type="week">

<form action="/action_page.php">
  <fieldset>
    <legend>Personalia:</legend>
    <input list="browsers">
    <datalist id="browsers">
        <option value="Edge">
        <option value="Firefox">
        <option value="Chrome">
        <option value="Opera">
        <option value="Safari">
    </datalist>
    <label for="fname">First name:</label><br>
    <input type="text" id="fname" name="fname" value="John"><br>
    <label for="lname">Last name:</label><br>
    <input type="text" id="lname" name="lname" value="Doe"><br>
    <select name="cars" id="cars">
        <optgroup label="Swedish Cars">
            <option value="volvo">Volvo</option>
            <option value="saab">Saab</option>
        </optgroup>
        <optgroup label="German Cars">
            <option value="mercedes">Mercedes</option>
            <option value="audi">Audi</option>
        </optgroup>
  </select>
    <input type="submit" value="Submit">
  </fieldset>
</form>
```
