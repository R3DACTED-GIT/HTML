# Guide to Creating a Basic First Webpage using Visual Studio Code and Live Preview

## Step 1: Install the Required Software
Before we get started, make sure you have the following software installed on your computer:
- Visual Studio Code (VS Code) - Download and install it from the official website: https://code.visualstudio.com/
- Web browser (e.g., Google Chrome, Mozilla Firefox, etc.) - To preview your webpage.
- After VS Code has downloaded, on the left sidebar go to Extensions and search for "Live Server" and install.

## Step 2: Create a New HTML File
- Open Visual Studio Code.
- Click on "File" in the top-left corner and choose "New File."
- Save the file with a meaningful name and the .html extension (e.g., index.html). Save it in a location where you can easily find it later.

## Step 3: Set Up the Basic Structure
Inside your index.html file, start by setting up the basic structure of an HTML document:

```
<!DOCTYPE html>
<html>
<head>
    <title>Your Page Title</title>
</head>
<body>

</body>
</html>
```

# Step 4: Adding Content
Now, let's add the elements you want to include in your webpage.

## Title:
Inside the <title> tag within the <head> section, set the title of your webpage. This title appears on the browser's tab.

## Headings:
In the <body> section, add various headings using ```<h1>, <h2>, <h5>, and <h6>``` tags.
```
<body>
    <h1>Main Heading (h1)</h1>
    <h2>Subheading (h2)</h2>
    <h5>Sub-subheading (h5)</h5>
    <h6>Sub-sub-subheading (h6)</h6>
</body>
```
## Paragraphs:

Add paragraphs using the ```<p>``` tag:
```
<body>
    <!-- Headings added above (h1, h2, h5, h6) -->

    <p>This is a paragraph. You can write a good amount of text here to convey your message to the readers.</p>
    <p>Another paragraph follows this one.</p>
</body>
```
## Link to a Webpage:
Add a link to another webpage using the <a> tag. Replace your_link_url with the actual URL of the webpage you want to link to, and Link Text with the text you want to display for the link.
```
<body>
    <!-- Headings and paragraphs added above -->

    <a href="your_link_url">Link Text</a>
</body>
<head> and <body>:
```
Note that we have already set up the <head> and <body> sections as shown in the basic structure (Step 3).

## Text and a Photo:
To add text and a photo, use the appropriate tags. Replace your_image_url with the actual URL (Drag and drop your image into the side bar where your files are at, right click and "copy relative path" of the image you want to display.
```
<body>
    <!-- Headings, paragraphs, and link added above -->

    <p>Here is some text with an image:</p>
    <img src="your_image_url" alt="Description of the image">
</body>
```

## Step 5: Preview Your Webpage
To see the results of your work, right-click anywhere inside the index.html file in VS Code and select "Open with Live Server." This will open your webpage in your default web browser.
#
## Your website should look simular to this: 
![image](https://github.com/R3DACTED-GIT/HTML/assets/140674398/e5593e97-1616-443a-a3bd-2a018302f434)

# Part 2: A basic Nav Bar and Favicon.
A favicon image is the little icon you see on the left side of the browser tab, just beside the page title. It's like a small representation of your website. To include a favicon on your site, you have two options: either save the favicon image directly to the root directory of your web server, or create a folder named "images" within the root directory and place the favicon image there. A popular and conventional name for a favicon image file is "favicon.ico". By doing this, your website will have its own distinctive and recognizable icon displayed in the browser tab, providing a more polished and professional look.
```
<head>
  <title>Your Page Title</title>
  <link rel="icon" type="image" href="image address">
</head>
```
The <link> element is used in HTML to define the relationship between a document and an external resource. It is typically included in the <head> section of an HTML document and is commonly used to link to external stylesheets, such as CSS files. By using the <link> element, you can easily connect your HTML document to other resources, like stylesheets or icon files, which allows for better organization and separation of concerns in web development. This helps in maintaining clean and structured code, making it easier to update and manage various aspects of a webpage independently.

## Nav bar:
```
<body>
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
</body>
```

The ```<nav>``` element is used in HTML to represent a navigation section on a webpage. It is typically used to define a collection of navigation links, menus, or any other content that aids in navigating the website. The ```<nav>``` element helps in organizing and structuring the navigation menu, making it semantically clear that it contains navigation-related information. When using ```<nav>```, it's essential to include lists of links or other navigation elements inside it to create a well-structured and accessible navigation system for your website.

The ```<ul>``` element is used in HTML to create an unordered list. It stands for "unordered list" and is used to group a collection of related items, presented in no particular order. Each item in the list is represented by the ```<li>``` (list item) element. The ```<ul>``` element is ideal for creating bullet-point lists, navigation menus, or any content that doesn't require a specific sequence. By using ```<ul>```, you can present information in a clear and concise manner, making it easier for users to scan through the content and grasp key points without any predetermined ordering.

# Part 3: Your Basic Form
```
<form action="">
  <label for="first">First name:</label><br>
  <label for="last">Last name:</label><br>
  <input type="text" id="First" name="First" value="John"><br>
  <input type="text" id="Last" name="Last" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form> 
```
## ```<forms>``` Element:
The ```<form>``` element is used to create a form on a webpage. It is a container that holds various form elements like input fields, checkboxes, radio buttons, and buttons. The ```action``` attribute in the ```<form>``` tag specifies the URL to which the form data will be submitted when the user clicks the submit button.

## ```<labels>``` Elements:
The ```<label>``` element is used to associate a label with a form control, improving accessibility and user experience. The ```for``` attribute in the ```<label>``` tag specifies the ```id``` of the corresponding form control. In this example, there are two labels, one for the "First name" input and one for the "Last name" input.

## ```<inputs>``` Elements:
The ```<input>``` element is used to create various types of form controls, such as text inputs, checkboxes, radio buttons, and submit buttons. In this code, two text inputs are used with the ```type="text"``` attribute. The ```id``` and ```name``` attributes are used to uniquely identify and name the form fields. The ```value``` attribute sets the initial value for each input field. For the "First name" input, the value is set to "John," and for the "Last name" input, the value is set to "Doe."

## ```<br>``` Element:
The ```<br>``` element is a line break that creates a new line, forcing the next element to appear on the next line. In this example, it is used to place the "Last name" input on a new line, creating a line break after the "First name" input and its corresponding label.

## ```<submit>``` Input Element:
The last ```<input>``` element in this form has ```type="submit"```. This creates a submit button that users can click to submit the form data to the URL specified in the ```action``` attribute of the ```<form>``` element. The value of the button is set to "Submit," which appears as the text on the button.







# So far recap: 
![image](https://github.com/R3DACTED-GIT/HTML/assets/140674398/36095d57-54f8-4d4b-8cf3-0a8417c7ad6c)

