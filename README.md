# Admin Dashboard
___
The live site can be found [here](https://stephaniequintana.github.io/Admin-Dashboard/)
> This is the final project from **The Odin Project's** [Intermediate HTML and CSS](https://www.theodinproject.com/paths/full-stack-javascript/courses/intermediate-html-and-css) course. The major focus is layout design, incorporating nested grids and utilizing flexbox where beneficial. This is an all encompassing challenge and can be found [here](https://www.theodinproject.com/paths/full-stack-javascript/courses/intermediate-html-and-css/lessons/admin-dashboard) should you like to try it out for yourself.
<!-- > Live demo [_here_](https://www.example.com). If you have the project hosted somewhere, include the link here. -->
___
![image](https://user-images.githubusercontent.com/81270711/154956398-7e6531dc-7068-4d7d-9fb4-87f68b229230.png)
___
## Table of Contents
* [Design Plan](#design-plan)
* [Challenges Encountered and Knowledge Gained](#challenges-encountered-and-knowledge-gained)
* [Languages](#languages)
___
## Design Plan
- The first phase of the project entails setting up the project and layout:
    Setting up your HTML and CSS with some simple dummy content.
    Applying Grid properties for the basic layout.
    Taking each section at a time targeting nested elements into Grid cells or Flexbox containers.
___
## Challenges Encountered and Knowledge Gained
* The ease of CSS variables is by far more convenient for updating overall styling.
    ```CSS
        :root{
            --blue: rgb(25,146,212);
            --yellow: rgb(255,198,0);
            --lite-text: hsl(0, 2%, 12%);
        }
    ```
* In my excitement to begin the project, I did not realize that icons were furnished. It was quite an experience to create my own. I faced challenges with sizing in different areas of the layout, but prevailed with a simple transform:
    ```css
        .profile i{
            color: var(--blue);
            transform: scale(1.7);
            }
    ```
* I found grid-template-areas to be the simplest way of defining cell placement.
    ```css
        .main{
            display: grid;
            grid-gap: 1.5em;
            grid-template-columns: repeat(2, minmax(150px, 500px)) 25%;
            grid-template-areas: "project-title . announce-title"
                                 "projects projects announcements"
                                 "projects projects trend-title"
                                 "projects projects trending";
        }
    ```
## Languages
- HTML 5
- CSS
