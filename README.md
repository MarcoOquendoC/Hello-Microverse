![](https://img.shields.io/badge/Microverse-blueviolet)

# Set up a "Hello Microverse" project

> In this project, I set up a "Hello world" repository. The goal here is to master all of the tools and best practices I have learned about in previous steps. I will be using them in all Microverse projects and most likely in my future job as well.

This [link](https://questions.microverse.org/t/configure-linters-for-html-and-css/2009) is useful. It has two videos following the steps (there is no sound though).


## Built With

- Major languages
	HTML, CSS

- Frameworks
	None

- Technologies used
	Github, Git, VSCode

## Getting Started

### Prerequisites

- knowledge of git
- Knowledge of github



### Setup

- Create a repository, activate actions workflow. It will create a blank.yml file.
- Clone repository and make a branch.
- Create index.html, styles.css files 
- link index.html with styles.css


### Install

- [Git Bash](https://git-scm.com/).
- [node.js](https://nodejs.org/en/download/).
- [Visual Studio Code](https://code.visualstudio.com/Download).


### Usage

- Write the following commands to install [linters](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/clean-code/linters.md) (It could take a while for each one).

   - Install Stylelint
       
      ``` npm install --save-dev stylelint@13.x stylelint-scss@3.x stylelint-config-standard@21.x stylelint-csstree-validator@1.x ```
      
   - Install Webhint

      ``` npm install --save-dev hint@7.x ```

   - Install Lighthouse

      ``` npm install -g @lhci/cli@0.7.x ```

### Run tests

   - Test Stylelint

      ``` npx stylelint "**/*.{css,scss}" ```

   - Test Webhint
       
      ``` npx hint . ```

   - Test Lighthouse

      ``` lhci autorun --upload.target=temporary-public-storage --collect.staticDistDir=. ```

#### Note: this command could be used to autocorrect styles.css

``` npx stylelint "**/*.{css,scss}" --fix ``` 



### Deployment

- There must be included node_modules folder in the .gitignore file.
- Stage, commit and push the files to github.
- Make a pull request and merge when all linters have been aproved.


## Authors

👤 **Marco Vinicio Oquendo**

- GitHub: [@MarcoOquendoC](https://github.com/MarcoOquendoC)
- Twitter: [@marcooquendoc](https://twitter.com/marcooquendoc)
- LinkedIn: [Vinicio Oquendo](https://www.linkedin.com/in/vinicio-oquendo-4a289156/)


## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

Feel free to check the [issues page](../../issues/).

## Show your support

Give a ⭐️ if you like this project!

## Acknowledgments

- The comunity [forum](https://questions.microverse.org/t/configure-linters-for-html-and-css/2009) has some videos to set this up.
- Microverse

## 📝 License

This project is [MIT](https://github.com/microverseinc/readme-template/blob/master/MIT.md) licensed.