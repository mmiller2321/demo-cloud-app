<p align="center"><img src="https://res.cloudinary.com/dtfbvvkyp/image/upload/v1566331377/laravel-logolockup-cmyk-red.svg" width="400"></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/license.svg" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains over 1500 video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the Laravel [Patreon page](https://patreon.com/taylorotwell).

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Cubet Techno Labs](https://cubettech.com)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[British Software Development](https://www.britishsoftware.co)**
- **[Webdock, Fast VPS Hosting](https://www.webdock.io/en)**
- **[DevSquad](https://devsquad.com)**
- [UserInsights](https://userinsights.com)
- [Fragrantica](https://www.fragrantica.com)
- [SOFTonSOFA](https://softonsofa.com/)
- [User10](https://user10.com)
- [Soumettre.fr](https://soumettre.fr/)
- [CodeBrisk](https://codebrisk.com)
- [1Forge](https://1forge.com)
- [TECPRESSO](https://tecpresso.co.jp/)
- [Runtime Converter](http://runtimeconverter.com/)
- [WebL'Agence](https://weblagence.com/)
- [Invoice Ninja](https://www.invoiceninja.com)
- [iMi digital](https://www.imi-digital.de/)
- [Earthlink](https://www.earthlink.ro/)
- [Steadfast Collective](https://steadfastcollective.com/)
- [We Are The Robots Inc.](https://watr.mx/)
- [Understand.io](https://www.understand.io/)
- [Abdel Elrafa](https://abdelelrafa.com)
- [Hyper Host](https://hyper.host)

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-source software licensed under the [MIT license](https://opensource.org/licenses/MIT).

## Heroku Cloud Deployment Instructions
1. Create app in Heroku:
    - Click Create App button from the main page. Give your application a name. Click the Create App button.
    - On the Project page, select the Deploy Tab, and link your application to your GitHub repository (BitBucket is not supported on Heroku). If you are not using GiHub, you can either copy your BitBucket repository to GitHub or use the Heroku CLI, as documented below.
    - On the Project page, select the Settings Tab, click the Add Buildpack button, for PHP click the PHP button, click the Save Changes button.
    - On the Project page, select the Resources Tab, under the Add-ons search for JawsDB MySQL, select JawsDB MySQL from the search list, select the Free plan, click the Provision button. NOTE: If you fail to connect too many times to the database Heroku may lock you out from connecting to your database. If you repeatedly cannot connect to your database and are sure your configuration is correct, then delete your current JawsDB MySQL database Add-on and add a new JawsDB MySQL database.
2. Update your App Configuration as necessary:
    - Update the database configuration parameters in your code.
    - For non-Laravel apps add an empty file (one with just { } as contents) named composer.json to your GitHub repository.
    - You can set the version of PHP using the following entry in your composer.json file: "require": { "php": "^7.1.0" }
    - See Heroku PHP Support located at https://devcenter.heroku.com/articles/php-support
3. Connect MySQL Workbench to the instance of MySQL Database. Run your DDL Script to configure the database.
4. You can deploy your application either thru the Heroku GIT Repository or by using your own GitHub or Bitbucket GIT repository. Follow either steps 5 or 6 below. NOTE: make sure to include all of the hidden files and the vendor folder in your GIT repository (you might need to modify the .gitignore file) and ensure the .env file is included as this is a required file to run a Laravel application. This should also be tested by cloning your GIT repository as a zip file, then deploying the clone files to your local MAMP, and validating that the application functions properly from the cloned repository.
5. To deploy using the Heroku GIT repository use the following steps:
    - Clone the Heroku GIT repository provided by Heroku (go to your App Settings to get the URL).
    - Update your App Configuration as noted above.
    - Push your code from your local repository to the Heroku GIT repository.
    - Test the app: https://[APP NAME].herokuapp.com.
6. To deploy using your GitHub repository and a Build Pipeline use the following steps:
    - Update your App Configuration as noted above and push the changes to your GitHub repository.
    - Create Heroku Pipeline and add your PHP app to it.
    - Go to your Heroku Pipeline and click on your PHP app, select the Deploy menu option, and make sure the Enable Automatic Deploys is enabled from your master branch.
    - Start a Build by performing either of one the following operations:
7. Go to your Heroku Pipeline and click on your PHP app, select the Deploy menu option, and then click the Deploy Branch button.
8. Push a code change to your GitHub repository.
    - Test your app at: https://[APP NAME].herokuapp.com.


## How to host a Laravel project on Heroku (Quick Instructions)
1. After pushing your laravel project to GitHub, deploy the app in Heroku and click your Heroku URL website link. You should see a "Forbidden" error screen which is a good sign. 2. Now we need to create a file named "Procfile in the root directory of your project with "web: vendor/bin/heroku-php-apache2 public/" and make sure it has been pushed to GitHub. 
3. If you go to your Heroku website again you should receive a "500 | Server Error" which is a Laravel error page which also means your project has been deployed successfully. 4. Heroku doesn't work with the Laravel .env file so you need to manually add your variables to Heroku by going to "Deploy" --> Click "Reveal Config Vars". 
5. Add the neccessary variables then try again and you should see your Laravel Home page displayed.  
    - https://just1and0.medium.com/how-to-host-your-laravel-application-for-free-on-heroku-4789688d444b

## Cloud Hosted Websites
- [(Broken) Azure Project Link]().
- [Heroku Project Link](https://demo-cloud-app.herokuapp.com/).
- [(In-Progress) Amazon Web Services Project Link]().
- [(In-Progress) Google Cloud Project Link]().
