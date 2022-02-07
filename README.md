# HTML & CSS3 Course

**NOTE:** If you are running on Windows, you need to initialize npm to create `package.json` file. 
   ```
   npm init -y
   ```

1. Run
   ```
   npm install --save-dev hint@6.x
   ```
   *not sure how to use npm? Read [this](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm).*
2. Copy [.hintrc](.hintrc) to the root directory of your project.
3. **Do not make any changes in config files - they represent style guidelines that you share with your team - which is a group of all Microverse students.**
   - If you think that change is necessary - open a [Pull Request in this repository](../README.md#contributing) and let your code reviewer know about it.
4. Run
   ```
   npx hint .
   ```
5. Fix validation errors.

### [Stylelint](https://stylelint.io/)

A mighty, modern linter that helps you avoid errors and enforce conventions in your styles.

2. Copy [.stylelintrc.json](./.stylelintrc.json) to the root directory of your project.
3. **Do not make any changes in config files - they represent style guidelines that you share with your team - which is a group of all Microverse students.**
   - If you think that change is necessary - open a [Pull Request in this repository](../README.md#contributing) and let your code reviewer know about it.
4. Run `npx stylelint "**/*.{css,scss}"` on the root of your directory of your project.
5. Fix linter errors.
6. **IMPORTANT NOTE**: feel free to research [auto-correct options for Stylelint](https://stylelint.io/user-guide/cli#autofixing-errors) if you get a flood of errors but keep in mind that correcting style errors manually will help you to make a habit of writing a clean code!

## Have you already completed the Sass lessons?

If you completed the Sass lessons you may prefer to work with SCSS files, if that's the case you need to perform
a few modifications to the linter configuration files.

1. In the file `.github/workflows/linters.yml` [line 48](https://github.com/microverseinc/linters-config/blob/master/html-css/.github/workflows/linters.yml#L48) replace `"**/*.{css,scss}"` with `"**/*.scss"`
2. Use `npx stylelint "**/*.scss"` to lint you SCSS files and not the generated CSS

Once you've done the previous steps you can focus on your SCSS files and not in fixing the generated CSS output
every time.
