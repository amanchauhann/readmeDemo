# Email Template Previewer

Dashboard built on top of Shadcn for quick preview for all the stakeholders of 
- Email Templates 
- Common code snippets

It’s the perfect way to keep all stakeholders in the loop, ensuring everyone stays on the same page and aligned.

## Table of Contents
1. [ Features. ](#features)
2. [ Installation. ](#installation)
3. [ For stakeholders. ](#for-stakeholders)
4. [ Contribution. ](#contribution)


## Features
- This project is made in ```Next v14``` with [Shadcn](https://ui.shadcn.com/) UI library.
- On the right, in the ```scrollarea``` you can find the required template.

- Upon navigating inside, different versions of the templates would be displayed that is been wither currently in use or have been in the past.

- On the left, in the ```scrollarea``` you can find the list of available versions of the template.




## Installation
Clone the repository with the following command:

```bash
clone command will be here **
```

Move into the project with following command:

```bash
cd repo name will be here**
```

Install dependencies with the following command: 
```bash
npm install

// if the above command throws error, use:

npm install --legacy-peer-deps
```

Run the project with following command:

```bash
npm run dev
```
<a name="desc"></a>
## For stakeholders

- To check how the modifications would look like click on "Edit on Codepen" to get redirected on codepen on top-right of embedding and start editing.
- The updated code along with preview can be sent across afterwards.

![Edit on codepen](https://github.com/amanchauhann/readmeDemo/assets/44115421/2b72255d-f8ea-47de-8410-c63be5b08a14)

## Contribution

```bash
├── app
├── utils
│   ├── pages.tsx
│   │   ├── **/templates
        ├── **/snippets
├── package.json
├── node_modules
```

### Snippets
To add more snippets.
- Inside pages.tsx in utils, you"ll find two  objects for adding: ```templates``` and ```snippets```
with smilar schemas.
```bash
export const snippets: any = {
  route: {
    heading: "Heading",
    description: "Display description for the entire module.",
    variantHeading: "Versions",
//** there can be more than one variant for each template that is being in use in different contexts.
    variants: [
      {
        id: "this is used for scrolling on different sections the page.",
        title: "Title",
        iframeLink: enter the iframe link for the code,
      },
    ],
  },
}
```
Example:
```bash
export const templates: any = {
  "validate-account": {
    heading: "Account Validation",
    description: "Displaying Template for Account Validation",
    variantHeading: "Versions",
    variants: [
      {
        id: "decentro",
        title: "Decentro",
        iframeLink:
          "https://codepen.io/opxqnlpr-the-looper/embed/gOJgXqW?default-tab=html%2Cresult",
      },
    ],
  },
};
```
- Change the values for the respective keys And a valid route will be created and displayed.
- To check more how route is being created, go to:

```bash
├── config
│   ├── docs.ts
        ├── **/docsConfig
               ├── mainNav
               ├── sidebarNav (routes are being made here)
        ├── **/snippetsConfig
```



### Templates
To add more Templates.
- Inside pages.tsx in utils, you"ll find two  objects for adding: ```templates``` and ```snippets```
with smilar schemas.
```bash
export const templates: any = {
  route: {
    heading: "Heading",
    description: "Display description for the entire module.",
    variantHeading: "Versions",
//** there can be more than one variant for each template that is being in use in different contexts.
    variants: [
      {
        id: "this is used for scrolling on different sections the page.",
        title: "Title",
        iframeLink: enter the iframe link for the code,
      },
    ],
  },
}
```
Example:
```bash
export const templates: any = {
  "validate-account": {
    heading: "Account Validation",
    description: "Displaying Template for Account Validation",
    variantHeading: "Versions",
    variants: [
      {
        id: "decentro",
        title: "Decentro",
        iframeLink:
          "https://codepen.io/opxqnlpr-the-looper/embed/gOJgXqW?default-tab=html%2Cresult",
      },
    ],
  },
};
```
- Change the values for the respective keys And a valid route will be created and displayed.
- To check more how route is being created, go to:

```bash
├── config
│   ├── docs.ts
        ├── **/docsConfig
        ├── **/snippetsConfig
               ├── mainNav
               ├── sidebarNav (routes are being made here)
```


## THANKS
