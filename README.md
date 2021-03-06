# Intelligo Game - Art & Technology Tohoku 2018 contest
[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors)
[![StackShare](https://img.shields.io/badge/tech-stack-0690fa.svg?style=flat)](https://stackshare.io/tortuvshin/intelligo-game)

Augmented reality game development repository. Special International Prize for the Art & Technology Tohoku 2018 contest.

| [Requirements][] | [Development][] | [Deploy][] | [Built with][] | [Contributors][] | [License][] |
|---|---|---|---|---|---|

## Requirements

- [MongoDB](https://www.mongodb.com/download-center)
- [Node.js 8.0+](http://nodejs.org)
- [Git](https://git-scm.com/download/win)

## Development

Clone repository `git clone https://github.com/tortuvshin/intelligo-game.git`

Install dependencies `npm install`

Start up your game by running node `node app.js`

Web browser [this link](http://localhost:5000) to test the game.

Compile the sass `npm run build-css`

Watch the sass `npm run watch-css`

## Deploy

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

### Deploy to Heroku

<img src="https://upload.wikimedia.org/wikipedia/en/a/a9/Heroku_logo.png" width="200">

- Download and install [Heroku Toolbelt](https://toolbelt.heroku.com/)
- In terminal, run `heroku login` and enter your Heroku credentials
- From *your app* directory run `heroku create`
- Run `heroku addons:create mongolab`.  This will set up the mLab add-on and configure the `DB_URI` environment variable in your Heroku app for you.
- Lastly, do `git push heroku master`.  Done!

**Note:** To install Heroku add-ons your account must be verified.

---

<img src="https://mlab.com/company/img/branding/mLab-logo-onlight.svg" width="200">

- Open [mlab.com](https://mlab.com) website
- Click the yellow **Sign up** button
- Fill in your user information then hit **Create account**
- From the dashboard, click on **:zap:Create new** button
- Select **any** cloud provider (I usually go with AWS)
- Under *Plan* click on **Single-node (development)** tab and select **Sandbox** (it's free)
 - *Leave MongoDB version as is - `2.4.x`*
- Enter *Database name** for your web app
- Then click on **:zap:Create new MongoDB deployment** button
- Now, to access your database you need to create a DB user
- Click to the recently created database
- You should see the following message:
 - *A database user is required to connect to this database.* **Click here** *to create a new one.*
- Click the link and fill in **DB Username** and **DB Password** fields
- Finally, in `.env` instead of `mongodb://localhost:27017/test`, use the following URI with your credentials:
 - `db: 'mongodb://USERNAME:PASSWORD@ds027479.mongolab.com:27479/DATABASE_NAME'`

**Note:** As an alternative to mLab, there is also [Compose](https://www.compose.io/).

## Built with

* [Node.js](https://nodejs.org/en/download/)
* [Express.js](https://expressjs.com/)
* [MongoDB](https://www.mongodb.com/download-center)
* [Tracking.js](https://trackingjs.com/)
* [Three.js](https://threejs.org/)

## Contributors

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore -->
<table>
  <tr>
    <td align="center"><a href="https://github.com/tortuvshin"><img src="https://avatars3.githubusercontent.com/u/9257227?v=4" width="100px;" alt="Turtuvshin Byambaa"/><br /><sub><b>Turtuvshin Byambaa</b></sub></a><br /><a href="#infra-tortuvshin" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/intelligo-systems/intelligo-game/commits?author=tortuvshin" title="Tests">⚠️</a> <a href="https://github.com/intelligo-systems/intelligo-game/commits?author=tortuvshin" title="Code">💻</a></td>
    <td align="center"><a href="https://www.intelligo.systems/"><img src="https://avatars2.githubusercontent.com/u/12738721?v=4" width="100px;" alt="Enkhbayar Doljinsuren"/><br /><sub><b>Enkhbayar Doljinsuren</b></sub></a><br /><a href="#infra-doljko" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/intelligo-systems/intelligo-game/commits?author=doljko" title="Tests">⚠️</a> <a href="https://github.com/intelligo-systems/intelligo-game/commits?author=doljko" title="Code">💻</a></td>
  </tr>
</table>

<!-- ALL-CONTRIBUTORS-LIST:END -->
You may contribute in several ways like creating new features, fixing bugs, improving documentation and examples
or translating any document here to your language. [Find more information in CONTRIBUTING.md](CONTRIBUTING.md).

## License

Intelligo game is open-sourced software licensed under the [MIT](LICENSE).

**[⬆ back to top](#intelligo-game)**

[Requirements]:#requirements
[Development]:#development
[Deploy]:#deploy
[Built with]:#built-with
[Authors]:#authors
[Contributors]:#contributors
[License]:#license
