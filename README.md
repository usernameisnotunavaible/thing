# Svelte Template

This is a template for ORRHS Web Design and Development students to use when
creating a new Svelte project. This comes with a few built-in packages to help
you get started.

## Built-In Packages

- [Svelte](https://svelte.dev/)
- [SvelteKit](https://kit.svelte.dev/)
- [TailwindCSS](https://tailwindcss.com/)
- [PostCSS](https://postcss.org/)

## Getting Started

### Use This Template

1. To create a new project based on this template from GitHub, click the "Use 
this template" button above.

2. Copy the link that appears.
3. Open WebStorm.
4. Click "Project > New > From Version Control" and paste the link you 
   copied in step.
5. Click "Clone".

### Install Dependencies

Once you've created a project and cloned it to your local machine, open the
project in WebStorm.

WebStorm should then prompt you to install the dependencies. If it doesn't,
you can install them manually using the terminal:

  ```bash
  npm install
```

### Signing Into GitHub in WebStorm Settings

To sign in to GitHub in WebStorm, go to `Preferences > Version Control > GitHub`
and click the "Sign In" button.

### Create A GitHub Repo Using Webstorm Settings

To create a new repo on GitHub using WebStorm, go
to `Preferences > Version Control > GitHub` and click the "Create Repository"
button.

## Start Writing Code / Developing

### Start A Local Server

Once you've created a project, installed dependencies, setup GitHub, you will
need to start the app to get everything running. This is called a local server.

To start a local development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

### Writing Code

To write code for your app, you will need to write code in the `src` directory.
There two main types of code you will write:

- **Components** - These are the building blocks of your app. They are reusable
  pieces of code that you can use to build your app.
- **Pages** - These are the pages of your app. They are the main pages of your
  app that users will see.

#### Components

To create a new component, create a new file in the `src/lib/components`
directory. The file name should be the name of the component. For example, if
you want to create a component called `Button`, you would create a file
called `Button.svelte`.

### Pages

To create a new page, create a new folder in the `src/routes` directory with
the name of your page. Then, create a file inside called `+page.svelte`. It
has to be named `+page.svelte` because SvelteKit uses the `+` to determine what
is a
page.

For example, if you want to create a page called `Home`, you would create a
folder called `Home.svelte` and inside, create a file called `+page.svelte`.

## Adding images from your assets folder

To add an image from your `assets` folder, you can use the `src/lib/assets`
path. For example, if you have an image called `profile-pic.png` in
your `assets`
folder, you can add it to your app like this:

```javascript
import profilePic from '$lib/assets/profile-pic.png';
```

Then you can use it in your HTML like this:

```html
<img src='{profilePic}'
		 alt='Profile picture'>
```

## Adding CSS To A Page or Component

To add CSS to a page or component, you can use the `style` tag. For example, if
you want to add CSS to a component called `Button`, you would add the CSS to
the `Button.svelte` file like this:

```html
<style>
	.button {
		background-color: red;
	}
</style>
```

### Adding CSS To The Whole App In The App.css File

To add CSS to the whole app, you can use the `App.css` file. This file is
located in the `src` directory. You can add CSS to this file like this:

```css
body {
    background-color: red;
}
```

### Adding CSS To A Page or Component Using TailwindCSS

To add CSS to a page or component using TailwindCSS, you can use the `class`
attribute. For example, if you want to add CSS to a component called `Button`,
you would add the CSS to the `Button.svelte` file like this:

```html
<button class='bg-red-500'>Click Me</button>
```

## Build and Deploy on GitHub Pages

### Building Your App

What does "building" mean? It means taking your code and turning it into a
production-ready version of your app. This is what you will deploy to GitHub
Pages. It erases all the development-only code and packages and creates a
smaller and faster version of your app.

To create a production/live version of your app:

```bash
npm run build
```

This will create a `build` directory/folder with a production build of your app.
You can run the newly built app with `npm run start`.

### Deploying to GitHub Pages

To deploy your app to GitHub Pages, you will need to create a new repo on GitHub
and push your code to it. Then you can run the following command to deploy your
app to GitHub Pages.

```bash
npm run deploy
```
