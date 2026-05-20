# HTML basics

HTML is not a coding language, it is a language to describe the website sturcture called markup language

## begin
We start with <!DOCTYPE html>, this declaration comply with basic html standard
<html> tag
Two section, head and body
<head> info about a web page
<body> the info displayed to the user
<h1> -- <h6>, header text, with largest size h1 to the smallest size h6
<p> paragraph text
<br>, closing tag not needed, a line break tool
<hr>, closing tag not needed, horizontal rule that divides the webiste  into section horizontally
<!-- --> comment that user cannot see


## Hyperlinks
Hyperlinks is a URL that you can attachedto a certain text, image
<a href="http://www.thelinkyouwantogo.com"> <!--element--> </a>

add "target=_blank" takes the user to linke with new tab
add "title="msg"" gives description regarding the hyperlinks

People use hyperlinks in their website to switch different page

## Image
<img src="image address">
height: adjusting the size of the img with given value, automatically adjust both height and width and keeps the ratio 
alt: the description about the image for user that failed to load the image or just better understanding about the image
title: give description when cursor stays on the image

## List
Three types of list
- Unordered
- Ordered
- Description

Every list starts with it own tag declaration -- <ul>/<ol>/<dl>
<li>: tags for the item you are storing
<dt>: description term (for dl) the name/term/item that want to describe
<dd>: description details, the description about the item

## Form