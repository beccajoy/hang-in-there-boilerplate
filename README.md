# Hang In There

A boilerplate repo.

## Contributors
- Kyle Jones ([Kyle's GitHub](https://github.com/KJJones13)) & Becca Steinbrecher ([Becca's GitHub](https://github.com/beccajoy))
- [GitHub Pages Deployed Site](https://beccajoy.github.io/hang-in-there-boilerplate/)

## About
Sometimes you need a pick me up. Remember those motivational posters that were all over the place in classrooms and online? We're going to make our own!

## Set Up

1. Fork this repository
2. Clone down this repository
3. `cd` into the repository
4. Run `open index.html` to view it in the browser

## Project Goals
- Write clean, DRY JavaScript to store our data
- Use a provided class by creating object instances using the new keyword
- Manipulate the page after it has loaded adding, removing, and updating elements on the DOM
- Understand event bubbling and use event delegation on dynamic elements
- Begin to understand how to write effective, clean HTML & CSS

### Wins
- Understanding and implementing git commands and branches
- Working with DOM

### Challenges
- Mitigating differences in personal work preferences
- Getting through the learning curve of code-pairing while 100% remote

## Technologies Used
- JavaScript

## In Action

### Iteration 0 - Main Page

![screenshot of main page showing poster](/readme-imgs/homepage.png)

- When the page loads, we should see a poster with a randomly selected image, title, and quote
- We enabled the "Show Another Random Button" to also load a randomly selected image, title, and quote when clicked on

### Iteration 1 - Switching Views

Form page:
![screenshot of form](/readme-imgs/form.png)

Saved posters page (once working with extra saved posters):
![screenshot of saved posters page](/readme-imgs/saved.png)

- When a user clicks the "Make Your Own Poster" button, we should see the form, and the main poster should be hidden
- When a user clicks the "View Saved Posters" button, we should see the saved posters area, and the main poster should be hidden
- When a user clicks the "Nevermind, take me back!" or "Back to Main" buttons, we should only see the main poster section
- In summary: Be able to switch between the three views (main poster, form, and saved posters) on the correct button clicks

_Hint: go check out the HTML and CSS files to see how the form and saved posters sections are being hidden in the first place_

## Iteration 2 - Creating a New Poster

Form being filled out:
![screenshot of form](/readme-imgs/form.png)

Once poster is saved:
![screenshot of result](/readme-imgs/form-result.png)

- On the new poster form view, users should be able to fill out the three input fields and then hit the save button
- When the save button is clicked, several things will happen:
  - Save the submitted data into the respective arrays (image URL into the images array, etc) so that future random posters can use the user-created data
  - Use the values from the inputs to create a new instance of our Poster class
  - Change back to the main poster view (hiding the form view again)
  - Display the newly created poster image, title, and quote in the main view

## Iteration 3 - Saving Posters

- When a user clicks the "Save This Poster" button, the current main poster will be added to the `savedPosters` array.
- If a user clicks the "Save This Poster" more than once on a single poster, it will still only be saved once (no duplicates)
- Since our Saved Posters Section is not currently revealing the grid of mini posters, which displays the Saved Posters array, we have left a `console.log(savedPosters)` (on line 171). Within the Dev Tools, when "Save This Poster" is clicked, the current savedPosters array will show, and demonstrate that duplicate poster's are not accepted.

( Project spec & rubric can be found [here](https://frontend.turing.io/projects/module-1/hang-in-there.html) )
