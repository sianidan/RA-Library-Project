# RA-Library-Project

This is my Week 5 Project for the Reskill Americans Full-Stack Program. We were tasked with building a website for a library using a Figma design from one of the UX/UI program participants.

[Click here to see the live site.](https://sianidan.github.io/RA-Library-Project/)

## Table of Contents
- [Overview](#overview)
    - [Site Details](#site-details)
    - [Design](#design)
- [Helpful Resources](#helpful-resources)
    - [Design Elements](#design-elements)
    - [Accessibility](#accessibility)
    - [Responsive Design](#responsive-design)
- [Continued Development](#continued-development)
    - [Future Intentions](#future-intentions-for-this-project)

## Overview

### Site Details
So far, the website only appears as intended on desktop browsers as I'm still in the process of adding media queries for responsiveness. 

There are currently 10 different pages:
- Home Page
- About Us
    - The links on the left of the page don't direct anywhere yet.
- My Account (Login)
    - Clicking on the "Create an Account" button redirects to the registration page
- My Account (Register)
- Books & More
    - Clicking on the cover for *Twice as Hard* by Jasmine Brown redirects to its book description page. At the moment, this is the only book link that redirects.
- Book Description
    - Clicking on the link for the amount of reviews redirects to its reviews page
    - Clicking on the "Check Out" button redirects to the checkout page
- Book Reviews
    - Clicking on the book's title takes you back to the description page
- My Cart (Checkout)
    - After filling out the required fields, clicking the "Check Out" button redirects to the order confirmation page
- Order Confirmation
- Search Page
    - This page is accessed by clicking (or pressing the Enter key when focused) on the magnifying glass button in the header's search bar.
    - Hovering over the "Filter" button opens a filter menu, but the search and filter features aren't yet functional.
    - The links in the search results lead to external sites.
    - The page navigation at the bottom also isn't functional, and was just added for the overall page design.

### Design

[Click here to preview the design I chose.](https://www.figma.com/file/qIYJMGekw1joRsDLGpI3ku/Wk-5%3A-Library-Website-Project?t=o5oFetAOm7n1zL13-0)
- There are a few elements where I deviated from the original design. The primary purpose of this was to make general styles consistent across all pages, such as that for buttons and form inputs. I also changed text styling for very few specific parts of the site to increase visibility for those who are visually impaired and need more color contrast.

## Helpful Resources

### Design Elements

- [Search bar in the header](https://nikitahl.com/search-icon-inside-input#:~:text=Create%20a%20search%20icon%20inside%20input%20box%20with,submit%20button%20from%20the%20form.%20...%204%20Demo)
    - I referenced this tutorial in order to build the search bar in the website's header using only HTML and CSS. I previously had an idea of using this general approach, but this tutorial helped me to iron out any kinks.

### Accessibility

- [Labels on the checkout page](https://www.w3.org/WAI/tutorials/forms/labels/#hiding-label-text)
    - This website is an excellent resource for anyone who may be unfamiliar with different aspects of accessibility in web development. I used this particular reference to visually hide form input labels while ensuring that they're still accessible for people who use screen readers.

### Responsive Design

- [MDN: CSS Media Queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)
    - I'm still working on adding media queries to make the website responsive, and this is the article that I frequently use to streamline the process.

## Continued Development
As of now, this website was built using only HTML5 and vanilla CSS. The first improvements will be making the website fully responsive. 

As my cohort in the Reskill Americans program progresses, we will be revisiting and building upon this project in the following weeks. We will become familiarized with adding JavaScript for the frontend and backend, then implement those acquired skills into this project.
### Future intentions for this project
As I continue to build on this website, I would like to implement/add features to make it fully functional. These changes include, but are not limited to: 
- Collect and store user information entered in form submissions, which will make sign-up and login available
    - Hide/show password option
    - Login page "Keep me signed in" submission and Forgot password option
    - My Account will include a user profile and a place to view your checkout history, holds, and a favorites list
- Search/Filter features and page navigation for search results
- Reviews page
    - Users can see all reviews for a book and submit their own
    - Option to filter reviews by rating, positive/negative, date written, etc.
    - Users can give a rating out of 5 stars
    - Automate the percentage breakdown of ratings
    - Thumbs-up button to rate a review as helpful; automate to increase the count when clicked
- Books & More page
    - Implement an API to fetch books based on the category selected from the navigation at the top of the page
    - Possibly adding a preview of a book's description (title, author, year published, overall rating) when you hover over or focus on the cover image. This might increase accessibility.
- Check Out
    - Send email confirmation to the user's email address
    - Add a book to cart when you click the "Check Out" button on its description page
    - Automate the order review on the Checkout page
