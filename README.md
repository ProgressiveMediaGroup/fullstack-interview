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

```docker-compose up```

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

The site owner must be allowed to specify their usernames for those sites when adding the widget in the WordPress back-end.

The front-end design of the widget is not important.

This test should take between 1 and 2 hours, although this is purely a guide.

## Submission Instructions
Please submit a zipped file containing your plugin to: [Chris Williams](christopher.williams@progressivecontent.com)
