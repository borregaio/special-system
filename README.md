# Carlos Borrega Portfolio Website

## Description 

The Carlos Borrega Portfolio Website consists in building a portfolio website entirely from scratch. Using HTML and CSS as the primary technologies, the project's main objective is to create a visually appealing and responsive website by implementing key features such as Flexbox, CSS variables, and media queries.

![Screenshot](./images/portfolio.png)


## Deployment

The deployed version of the Caros Borrega Portfolio Website can be accessed [here](https://borregaio.github.io/special-system/).


## Key Objectives

1. **Flexbox Layout:** Utilize Flexbox to create a flexible and efficient layout, ensuring a visually pleasing design that adapts seamlessly to different screen sizes.

2. **CSS Variables:** Implement CSS variables to enhance customization and maintainability, allowing for easy adjustments and updates to the website's styling.

3. **Media Queries:** Incorporate media queries to optimize the website's responsiveness on tablets and mobile phones, providing an optimal viewing experience across various devices.


## Installation

### Clone the repository
```console
git clone https://github.com/borregaio/special-system.git
```

### Navigate to the project directory
```console
cd special-system
```

### Open with VSCode
```console
code .
```

## Steps Followed to Create the Website

1. **HTML Structure:**
   - Develop the HTML structure, focusing on creating sections for different aspects of the portfolio, such as skills, projects, and contact information.
   
         ```html
         <section id="work">
            <h2 class="title">Work</h2>
            <div class="content">
            <div id="projects">
               <div class="project1">
                  <h3>Project 1</h3>
               </div>
               <div class="project2">
                  <h3>Project 2</h3>
               </div>
               <div class="project3">
                  <h3>Project 3</h3>
               </div>
               <div class="project4">
                  <h3>Project 4</h3>
               </div>
               <div class="project5">
                  <h3>Project 5</h3>
               </div>
            </div>
            </div>
         </section>
         ```

         ```html
            <section id="contact">
            <h2 class="title">Contact<br> Me</h2>
            <nav class="contact-links">
            <a href="#">Phone</a>
            <a href="#">Email</a>
            <a href="#">LinkedIn</a>
            <a href="#">GitHub</a>
            <a href="#">Twitter</a>
            </nav>
         </section>
         ```

2. **CSS Styling with Flexbox:**
   - Implement Flexbox to create a flexible and efficient layout for the portfolio.

      ```css
      .hero-banner {
         height: 400px;
         width: 100%;
         background-image: url(../images/main.jpg);
         background-position: center;
         background-repeat: no-repeat;
         background-size: cover;
         display: flex;
         align-items: flex-end;
         justify-content: end;
         }
      ```
   - Style each section with CSS to achieve the desired visual design.

      ```css
         #about,
         #work,
         #contact {
         width: 100%;
         display: grid;
         grid-template-columns: 20% 80%;
         grid-template-areas: "title content";
         padding: 50px 0;
         }
      ```
      ```css
         #projects {
            width: 100%;
            display: grid;
            grid-template-rows: 300px 200px 200px;
            grid-template-columns: 45% 45%;
            grid-template-areas: "project1 project1"
               "project2 project3"
               "project4 project5";
            padding: 50px 0;
            gap: 30px;
            justify-content: center;
            }
      ```

3. **Integrating CSS Variables:**
   - Utilize CSS variables to centralize styling parameters, allowing for easy customization and maintenance.

      ```css
         :root {
         --color1: #F8F6F4;
         --color2: #13005A;
         --color3: #00337C;
         --color4: #1C82AD;
         --color5: #03C988;
         }
      ```

4. **Media Queries for Responsiveness:**
   - Implement media queries to ensure the website is responsive on tablets and mobile phones.

      ```css
         /* Tablet Styles */

         @media only screen and (max-width: 768px)
      ```

      ```css
         /* Phone Styles */

         @media only screen and (max-width: 480px)
      ```

5. **Testing:**
   - Verified that the website maintains its visual consistency after the refactoring.