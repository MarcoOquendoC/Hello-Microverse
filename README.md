# Set up a "Hello Microverse" project

In this project, I set up a "Hello world" repository. The goal here is to master all of the tools and best practices I have learned about in previous steps. I will be using them in all Microverse projects and most likely in my future job as well.

This [link](https://questions.microverse.org/t/configure-linters-for-html-and-css/2009) could be useful. It has two videos following the steps (there is no sound though).

## Steps

1. Create a repository, activate actions workflow, it creates a blank.yml file.
2. Clone repository and make a branch.
3. Create index.html, styles.css files and link index with styles.css
4. It has to be previously installed [node](https://nodejs.org/en/download/) in the computer.
5. In the terminal write the following commands (It could take a while for each one).

   - These are to install and test Stylelint
       
      ``` npm install --save-dev stylelint@13.x stylelint-scss@3.x stylelint-config-standard@21.x stylelint-csstree-validator@1.x ```
      
      ``` npx stylelint "**/*.{css,scss}" ```
       
   - These are to install and test Webhint
   
      ``` npm install --save-dev hint@7.x ```
      
      ``` npx hint . ```
      
   - These are to install and test Lighthouse
   
      ``` npm install -g @lhci/cli@0.7.x ```
      
      ``` lhci autorun --upload.target=temporary-public-storage --collect.staticDistDir=. ```

6. There must be included node_modules folder in the .gitignore file.
7. Stage, commit and push the files to github.
8. Make a pull request and merge when all linters have been aproved.



---
#### Note: this command could be used to autocorrect styles.css

``` npx stylelint "**/*.{css,scss}" --fix ``` 
