# HoriseonRefactor
## Description
Horiseon, a marketing agency, wants a codebase that follows accessibility standards so their website is optimized for search engines. They have requested we refactor their code to ensure accessibility and clarify and simply their existing code base. 

## Problems
1. The client's codebase does not use semantic HTML elements, so the organization of the site is not immediatley apparent when reviewing its index.html file. 
2. The elements represented in the corresponding stylesheet do not progress in the same order as they are presented in the index.html file. 
3. Images within the index.html file do not include alt text attributes.
4. One link within the existing site is not active.
5. The site lacks a descriptive title.

## Solution
1. Text

**Example of HTML tags before code refactor:** 
...
<div class="content">
        <div class="search-engine-optimization">
            <img src="./assets/images/search-engine-optimization.jpg" class="float-left" />
            <h2>Search Engine Optimization</h2>
            <p>
                The dominance of mobile internet use means that users are searching for the right business as they travel, shop, or sit on their couch at home. Search Engine Optimization (SEO) allows you to increase your visibility and find the right customers for your business.
            </p>
        </div>
...

**Example of HTML tags after code refactor:** 
...
        <section class="content">
            <article id="search-engine-optimization" class="search-engine-optimization">
                <img src="./assets/images/search-engine-optimization.jpg" class="float-left" alt="A photo of a laptop, a cup of coffee, colored pencils, and a notebook with SEO ideas." />
                <h2>Search Engine Optimization</h2>
                <p>
                    The dominance of mobile internet use means that users are searching for the right business as they travel, shop, or sit on their couch at home. Search Engine Optimization (SEO) allows you to increase your visibility and find the right customers for your business.
                </p>
            </article>
...

2. Text
3. Comments were added to both the index.html and style.css files to help future developers better understand the structure of the files and how the elements referenced within each are used.

## Location
Use the following link to access the company's refactored website: [Horiseon Homepage](https://larrygjenkins.github.io/HoriseonRefactor/)

## Example Image
Following is an image of the Horiseon's homepage:

![Horiseon Homepage](./assets/images/Horiseon-Homepage.png)

