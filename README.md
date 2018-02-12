# Progressive Content: Full-stack Technical Test
This project is used as a technical test when interviewing potential full-stack web developers for Progressive Content.

## Installation Instructions
This project is designed to use Docker, so that you have a working duplicate of our test environment.

### Prerequisites
You will need the following applications to install and run this project:

1. [Git](https://git-scm.com/downloads)
2. [Docker](https://www.docker.com/get-docker)

### Actual Installation
To install the project, you will need to:

1. From your command line, run:

   ```git clone https://github.com/ProgressiveMediaGroup/fullstack-interview.git```

   This will download a clone of the fullstack-interview project to your machine, into the 'fullstack-interview' sub-folder.


2. From your command line, run:

   ```cd fullstack-interview```

   This will take you into the newly-cloned Git repository.

### Starting the test environment
Run the following from your command line:

```docker-compose up -d```

This will build and start the docker containers required, and will expose WordPress on port 8000. You can access it on [http://localhost:8000](http://localhost:8000)

If it hasn't already done so, it will also create the 'db_data' and 'wordpress' sub-folders. These are mapped volumes used by Docker to maintain file state when they are not running.

You can access all the files for your WordPress instance within the 'wordpress' sub-folder.

### Stopping the test environment
Run the following from your command line:

```docker-compose down```

This will stop all the docker containers, freeing the allocated resources and ports.

This will not delete any of the files within the 'db_data' and 'wordpress' sub-folders.

## Task Instructions
We need you to write a widget for a WordPress site that will contain links to the site owner’s Facebook, Twitter and LinkedIn profiles.

The site owner must be allowed to specify the links for those sites when adding the widget in the WordPress back-end.

The front-end design should fit with the standard WordPress Twenty Seventeen theme and include icons for each of the links

This test should take between 1 and 2 hours, although this is purely a guide.

## Submission Instructions
Please submit a zipped file containing your widget to: [Chris Williams](christopher.williams@progressivecontent.com)

## Troubleshooting

### Docker-Compose version issue

If you receive the following issue, you will need to upgrade your version of Docker to the latest version:

```Version in "./docker-compose.yml" is unsupported. You might be seeing this error because you're using the wrong Compose file version. Either specify a version of "2" (or "2.0") and place your service definitions under the `services` key, or omit the `version` key and place your service definitions at the root of the file to use version 1.
For more on the Compose file format versions, see https://docs.docker.com/compose/compose-file/```
