## This Course

In this course, you'll learn step-by-step how to build parts of [Design+Code 4](http://designcode.io/) from scratch. Everything you'll code exists on the live site, using exactly the same tech stack. You'll use the bleeding edge techniques in React and CSS 3 that will prepare you for your next job, or to make your developers' lives a little easier. The UI templates, source code will be provided along with text content, videos and chat support for better understanding. You don't need programming experience since it'll be explained visually from a designer's perspective, but having minimal knowledge of HTML, CSS will help you tremendously. Finally, you can take a test after completing the course to gain a certificate.

![//images.ctfassets.net/ooa29xqb8tix/1oA3HPnx0b5CHSWt6yigl0/801bd083e1fad4c803bd983a6f828219/dc-web.jpg](//images.ctfassets.net/ooa29xqb8tix/1oA3HPnx0b5CHSWt6yigl0/801bd083e1fad4c803bd983a6f828219/dc-web.jpg)

## React Hooks

[React](https://reactjs.org/) is by far the [most popular](https://medium.com/javascript-scene/top-javascript-frameworks-and-topics-to-learn-in-2020-and-the-new-decade-ced6e9d812f9) javascript framework for modern web development. Hooks make React even simpler by allowing you to create functional components using states without writing complex classes. Think of Hooks as **plugins**, where you can update your states with a single line of code. The main ones provided are **useState** and **useEffect** for controlling the lifecycle of your component, replacing the **componentDidMount** and **componentDidUpdate** altogether.

Note: other useful **Hooks** are **useRef** for referencing an element and **useInView** for detecting if an element is visible. There are also hundreds created by the community, such as in [react-use](https://github.com/streamich/react-use). Most importantly, you can create your own reusable Hooks, like for **Auth** and **Theme**.

```
const [state, setState] = useState("default value")

```

This replaces **componentDidMount**:

```
useEffect(() => {
	// code
}, [])

```

This replaces **componentDidUpdate** for **state**:

```
useEffect(() => {
	// code
}, [state])

```

## Styled Components

CSS by itself is the simplest way to create layouts. But with the **components** approach where you want things to be reusable and adaptive, it becomes hard not to rely on frameworks like [Sass](https://sass-lang.com/documentation/syntax) and javascript [inline styling](https://www.w3schools.com/react/react_css.asp). That's where [Styled Components](https://styled-components.com/) come in. With it, you can write cleaner, reusable CSS, without extremely long class names or a dedicated css file for each component, and with the power of nesting in **Sass** and scripting with **React Props**.

```
<Wrapper>Content</Wrapper>

const Wrapper = styled.div`
	display: grid;
`

// Replaces this
<div className="long-class-name">Content</div>

// Another CSS file
.long-class-name {
	display: grid;
}

```

## Figma Design System

This course comes with a design file made in [Figma](https://www.figma.com/) that includes the entire design system that I use for referencing the layout, colors, text styles and user interface elements. You'll be able to download this and see how our site was designed from the ground up.

![//images.ctfassets.net/ooa29xqb8tix/7FpcJ2sl03mOn7JPd0hLN1/4cec597e135065a53831daafc759d6fa/figma-design.jpg](//images.ctfassets.net/ooa29xqb8tix/7FpcJ2sl03mOn7JPd0hLN1/4cec597e135065a53831daafc759d6fa/figma-design.jpg)

## Install NodeJS

In order to install all the javascript libraries, including React, Styled Components, Gatsby and run your local web project, you'll need [NodeJS](https://nodejs.org/en/). The most reliable way to install it is using their download file.

[https://nodejs.org/en/](https://nodejs.org/en/)

## Install VSCode Code Editor

To write your code, it is essential to use a code editor. The best and most loved out there is [Visual Studio Code](https://code.visualstudio.com/download), which has a plethora of awesome extensions like Prettier for code formatting, Styled Components for code highlighting.

[https://code.visualstudio.com/download](https://code.visualstudio.com/download)

![//images.ctfassets.net/ooa29xqb8tix/2YZMRSBeuTLAWaYDxH5hXM/edaf0033636603dcfb5272947d5bcd00/vs-code-2.jpg](//images.ctfassets.net/ooa29xqb8tix/2YZMRSBeuTLAWaYDxH5hXM/edaf0033636603dcfb5272947d5bcd00/vs-code-2.jpg)

### Install VSCode Extensions

- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) - formats your code in a consistent way. This is important for staying in sync with teammates and while following the course. As a bonus, Prettier will make it easier to find problems in your code.
- [Styled Components](https://marketplace.visualstudio.com/items?itemName=jpoissonnier.vscode-styled-components) - code highlights, auto-completes your css when using Styled Components.
- [GraphQL](https://marketplace.visualstudio.com/items?itemName=kumar-harsh.graphql-for-vscode) - code highlights your graphql queries.
- [Material Theme](https://marketplace.visualstudio.com/items?itemName=Equinusocio.vsc-material-theme) (optional) - themes for VSCode. The one I'm using is called **Ocean**.
- [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme) (optional) - theme for your VSCode icons.
- [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens) (optional) - shows the author of the code. This is great for collaboration. And blaming. ;)
- [Live Share](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare-pack) (optional) - lets you code in real-time with other people. Great for code pairing.

![//images.ctfassets.net/ooa29xqb8tix/1iNND43lSvZfTdtMvbeXu9/8a3d4ae3797f31f5bf728adeee019187/vs-extension.jpg](//images.ctfassets.net/ooa29xqb8tix/1iNND43lSvZfTdtMvbeXu9/8a3d4ae3797f31f5bf728adeee019187/vs-extension.jpg)

### VSCode Built-in Terminal

VSCode comes with an extremely useful terminal where you can run your commands for install libraries and start your local web enviroment in order to preview your site. The keyboard shortcut is **Control `**

### VSCode Keyboard Shortcuts

- **Control `**: toggle terminal.
- **Cmd Shift P**: go to Command Palette to run commands.
- **Cmd P**: open file in project.
- **Cmd B**: toggle left Side Bar.

## Install Gatsby

[Gatsby](https://www.gatsbyjs.com/) is a framework built on top of React with essential features such as pages, templates, search engine optimization, etc. Think of it as a Wordpress for React where you can easily pick pre-made [templates](https://www.gatsbyjs.com/starters/?v=2) and plugins if you choose to. It has useful plugins for Contentful and Netlify.

[https://www.gatsbyjs.com](https://www.gatsbyjs.com/)

We'll use Gatsby mainly for its performance, routing and SEO. To install, type this command in the terminal.

```
npm install -g gatsby-cli

```

To create a new project for Gatsby using the default starter template.

```
cd Downloads
gatsby new designcodeweb <https://github.com/mengto/gatsby-starter-designcode>

```

We're using a simplified [Gatsby default starter](https://github.com/MengTo/gatsby-starter-designcode), without complex code and all in [Typescript](https://www.typescriptlang.org/), which will be taught later in the course. Having our own Gatsby starter also ensures that the steps will consistent in the future, avoiding confusion if for example, Gatsby decides to change their template.

## Start your site!

From your Downloads folder, drag and drop to the top portion of VSCode. This will open your project files. Then, start your local environment with the following command in the terminal.

```
gatsby develop

```

Congrats, you've just started your site! If you **Command click** the [http://localhost:8000](http://localhost:8000/), it'll preview your site in your favorite browser.

## Gatsby Site Structure

For any site, you'll need 3 main folders:

- **components**: put all the re-usable elements such as **buttons**, **sections**, **layout** and **styles**. It is best to organize into subfolders for their respective category. That's because you'll most likely end up with hundreds of components. In **components/layout**: you'll find the header and footer as well as the **layout.css**. This is where you can set your global font, links and reset your CSS if needed.
- **pages**: every file here will create a new page automatically. For example, **pricing.tsx** will route to **/pricing.** The only exception is that **index.tsx** will route to the main page.
- **images**: to simplify the implementation of local images, we made a folder at the root, in **/static/images**. These images will automatically be included in the public site using the url **/images/your-image.svg**.

## **Site Title**

You can change the site title by going to **gatsby-config.js** file and edit the title property.

```
// gatsby-config.js

module.exports = {
  siteMetadata: {
	  title: `Design+Code`,
	  description: `Don’t skip design. Learn design and code by building real apps with React and Swift. Complete courses about the best tools.`,
	  author: `@mengto`,
	},
}

```

## Semantic HTML and SEO

When you build a site, it is important to respect the correct structure for your texts, images and buttons. That's because search engines will read your content and index it based on your structure. Some basic rules are:

- Every page needs an **h1** for title.
- Every page needs meta tags specifically for search engines: **title**, **description**, **keywords**, etc.
- Every image needs an **alt** properties to explain what the image is about. This is also great for accessibility.

```
<img src="/images/logos/logo.svg" alt="logo" />
<h1>Design and code React apps</h1>
<p>
  Don’t skip design. Learn design and code by building real apps with
  React and Swift. Complete courses about the best tools.
</p>

```

## Github setup

Using git is essential to work in a team environment. This will create a version control of all the changes packaged in commits and if there are conflicts, you'll be able to compare and modify appropriately.

## Javascript errors

VSCode and React does a good job at telling you if there's something wrong with your code. In VSCode, you'll see a red underline if you forgot to close your brackets or tags for example. Finally, if you try to save and preview with broken code, your site will show the error and at which line number it is situated.

## Homework

- Build another site using another Gatsby starter template.
- Import images and replace the logo with your logo.
- Make the logo link to Home page.
