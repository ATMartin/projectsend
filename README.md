# ProjectSend

![ProjectSend logo](https://www.projectsend.org/projectsend-logo-new.png)

## About

ProjectSend is a free, clients-oriented, private file sharing web application.

Clients are created and assigned a username and a password.  
Uploaded files can be assigned to specific clients or clients groups.

Other features include auto-expiration of upload, notifications, full logging of actions by users and clients, option to allow clients to also upload files, themes, multiple languages...

Main website: [projectsend.org](https://www.projectsend.org)  
git: [current repository](https://github.com/projectsend/projectsend/)
Support via Patreon: [Patreon](https://www.patreon.com/ignacionelson)
Support via Open Collective: [Open Collective](https://opencollective.com/projectsend)

Feel free to participate!

## IMPORTANT

It is recommended that you download the latest release from the official website.

Downloading a development version directly from the repository might give you unexpected results, such as visible errors, functions that are still not finished, etc.

## Documentation

Docs are maintained at https://projectsend.gitbook.io.
There you will find installation requirements, instructions, tutorials, and troubleshooting information.

## Developing

This fork is packaged with a Docker config to help make running ProjectSend locally even easier. Here's how to get started:

First, make sure you have the necessary tools installed:

- [Git](https://git-scm.com/downloads)
- [Docker](https://docs.docker.com/get-docker/)
- [Composer](https://getcomposer.org/download/)
- [NPM](https://nodejs.org/en/download/)
- [Gulp](https://gulpjs.com/docs/en/getting-started/quick-start)

💡: These tools may be available through package managers like Homebrew, Chocolatey, etc.

### Run ProjectSend on your machine

1. Clone the repository
2. Run `npm install` and `composer update` to install both front- and back-end dependencies.
3. In a dedicated terminal window, run `gulp` to compile the main CSS and JS assets files.
2. In another dedicated terminal window, run `docker-compose up`.
  - This will start three containers: `web`, `db`, and `phpmyadmin`.
  - If you'd rather monitor logs in the Docker Desktop dashboard, you can use `docker-compose start` to run the containers without taking over your terminal.
3. You're ready to go!

- Visit `http://localhost` to begin installation through the included wizard.
- Visit `http://localhost:8080` to access the phpMyAdmin database management tool.

### Troubleshooting

Our Dockerfile should work on most systems, but if you encounter an error you should double-check the log output during `docker-compose up` first.
If the containers are building but you are experiencing Apache errors, you can troubleshoot config files within the `web_1` container at `/etc/apache2/`.

## How to join the project

Questions, ideas?

Send your message to contact@projectsend.org or join us on our [Facebook page](https://www.facebook.com/projectsend/)

## Translations

Thanks. Arigatō. Danke. Gracias. Grazie. Mahadsanid. Salamat po. Merci. אַ דאַנק.

You can download the compiled, translated files for the available languages from [projectsend.org/translations](https://www.projectsend.org/translations/)

If you want to translate ProjectSend in your language or work on an existing translation, please join the project on [Transifex](https://www.transifex.com/projects/p/projectsend)

## License

ProjectSend is licensed under [GNU GPL v2](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)

## Change log

[Available at the official site](http://www.projectsend.org/change-log/)
