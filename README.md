# Bescherelle ton code !

Slides are on [slides](http://slides.com/thierrymichel/bescherelle-ton-code#/)

## Demo with ESLint

1. Install linter

    ```js
    npm i -D eslint
    ```

    > Open `package.json`

2. Set config via `.eslintrc.json`
    > Open `.eslintrc.json`
3. Live coding with basic mistakes… (`src/index.js`)

    ```js
    const foo = 'bar'

    /**
     * Affiche message d'info
     *
     * @param {string} msg Message
     * @returns {undefined}
     */
    function info(msg) {
      console.info(msg)
    }

    info(foo)
    ```

    > Show __"problems"__ tab

4. Create `npm script` into `package.json`

    ```json
    "lint": "eslint --ext .js src/ || exit 0",
    ```

5. Open `src/cli.js` and copy/paste `bad.js` 😆

    > Save and close

6. `npm run lint`
7. __BONUS__: add `--fix`

    ```json
    "fix": "eslint --ext .js src/ --fix || exit 0",
    ```

8. Fix the world!

---

Talk @feweb "Debug front-end" conference - March 2017
