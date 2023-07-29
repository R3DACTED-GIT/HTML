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

Congratulations! You have created a basic webpage with headings, paragraphs, a link, and an image using Visual Studio Code and Live Preview. Now, feel free to experiment further and explore more HTML elements to enhance your webpage!
