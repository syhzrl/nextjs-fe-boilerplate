This is a static site front end boilerplate with [Next.js](https://nextjs.org/),  [Typescript](https://www.typescriptlang.org/), [Tailwindcss](https://tailwindcss.com/) and [Framer Motion](https://www.framer.com/motion/)

This boilerplate provides predefined file and folder structure to quickly build a static site.

```bash
src
    |__ assets
        |__ fonts
        |__ icons
        |__ images
    |__ components ( global components )
    |__ containers ( this is where you create your screens, e.g: Login Screen )
        |__ components ( each container can have their own components )
	|__ pages
```

Due to how Next.js's routing system works, I prefer to create each screens in the containers folder and render them in the pages folder as so:

```typescript
import React, { FunctionComponent } from 'react';
import HomeScreen from 'containers/home';

const Home: FunctionComponent = () => {
    return (
        <HomeScreen />
    );

};

export default Home;
```

<!--  You dont have to follow this exactly, change up the structure according to your own preferences if needed -->

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Linting

This boilerplate comes with a few predefined linting rules. Feel free to change or remove them as you see fit.

## Deploment

Since this boilerplate utilizes Next.js, the easiest way to deploy is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out their [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.