## Page Layout Techniques
In modern web development, we use semantic HTML elements to structure a webpage properly.

## Basic Page Structure

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page Layout Example</title>
</head>
<body>
    <header>
        <h1>Website Title</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="home">
            <h2>Welcome</h2>
            <p>This is the homepage.</p>
        </section>
        <section id="about">
            <h2>About Us</h2>
            <p>Information about our website.</p>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 My Website</p>
    </footer>
</body>
</html>

 Elements Used for Layout
<header> → Contains the website’s title, navigation, or logo.

<main> → Wraps the main content of the page.

<section> → Groups related content.

<footer> → Contains footer information (copyright, links).


## 2. Anchor (<a>) Tag
Used for linking to pages, sections, or external websites.

#Types of Links
#Internal Link (Same Website)

<a href="about.html">Go to About Page</a>
External Link (New Tab)


<a href="https://www.google.com" target="_blank">Visit Google</a>
Jump to Section (Same Page)


<a href="#contact">Go to Contact</a>
<section id="contact">
    <h2>Contact Us</h2>
</section>


## 3. <div> and <span> Tags
<div> → Block-level element for grouping content.

<span> → Inline element used for styling parts of text.

Example of <div>

<div class="box">
    <h2>Div Example</h2>
    <p>This is a block-level element.</p>
</div>
Example of <span>

<p>This is a <span style="color: red;">red text</span> inside a paragraph.</p>


## 4. Lists in HTML
Lists are used to organize content.

Unordered List (<ul>)

<ul>
    <li>Apple</li>
    <li>Banana</li>
    <li>Orange</li>
</ul>
➡ Displays bullet points.

Ordered List (<ol>)
html
Copy
Edit
<ol>
    <li>First step</li>
    <li>Second step</li>
    <li>Third step</li>
</ol>
➡ Displays numbers (1, 2, 3, ...).


## 5. Tables in HTML
Tables are used to display structured data.

<table border="1">
    <caption>Student Information</caption>
    <thead>
        <tr>
            <th>Name</th>
            <th>Age</th>
            <th>Grade</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Alice</td>
            <td>20</td>
            <td>A</td>
        </tr>
        <tr>
            <td>Bob</td>
            <td>22</td>
            <td>B</td>
        </tr>
    </tbody>
</table>
<caption> → Table title.

<thead> → Table header.

<tbody> → Table body.

<tr> → Table row.

<th> → Table header cell (bold).

<td> → Table data cell.


## 6. Forms in HTML
Forms collect user input.

Basic Form

<form action="submit_form.php" method="POST">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>

    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>

    <input type="submit" value="Submit">
</form>
action → Specifies where to send form data.

method="POST" → Sends data securely.

method="GET" → Sends data via URL.

## Input Types

<input type="text" placeholder="Enter Name">
<input type="password" placeholder="Enter Password">
<input type="email" placeholder="Enter Email">
<input type="number" placeholder="Enter Age">
<input type="date">
<input type="checkbox"> I agree
<input type="radio" name="gender" value="male"> Male
<input type="radio" name="gender" value="female"> Female
<input type="file">
<input type="range" min="1" max="100">
<input type="color">
<input type="submit" value="Submit">
<input type="reset" value="Reset">


## 7. Class and ID in HTML
Class (.) → Used for multiple elements.

ID (#) → Used for one unique element.

Example of Class

<p class="highlight">This text is styled with a class.</p>
css

.highlight {
    color: blue;
    font-weight: bold;
}
Example of ID

<p id="uniqueText">This text is styled with an ID.</p>
css

#uniqueText {
    color: red;
}

## 8. Checkbox and Select Dropdown
Checkbox

<input type="checkbox" id="agree">
<label for="agree">I agree to terms</label>
Dropdown (<select>)


<label for="country">Select Country:</label>
<select id="country" name="country">
    <option value="india">India</option>
    <option value="usa">USA</option>
    <option value="uk">UK</option>
</select>


## 9. Adding Video to a Website

<video width="400" controls>
    <source src="video.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
controls → Adds play, pause, volume buttons.

autoplay → Starts playing automatically.

loop → Repeats video.


## 10. Embedding a Website in Another Website
Use <iframe> to embed a webpage.

Example
<iframe src="https://www.example.com" width="600" height="400"></iframe>
➡ This loads an external website inside the webpage.