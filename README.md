# cs312-F2022-lab03-starter

Designed for use with [GitHub Classroom](https://classroom.github.com/), this repository contains the starter files for Lab 2 in Computer Science 312.

## Introduction
You are to build a database using protein data which is based on the database that you built for your previous lab. You are to add a third table to your database of Lab 02 protein data. The details may be found in your lab assignment sheet.

 - Your source code to build your database is to be submitted in the builder file; `src/proteinDB2_build.txt`.

 - Your queries and their results are to be submitted in the file; `writing/queries.md`.

 - Your data files are to be stored in the following directories, with the following names.

```
/src/data/uniprot_n_protein.tab
/src/data/uniprot_s_protein.tab
/src/data/uniprot_sars_protein.tab
/src/data/uniprot_m_protein.tab

```

Note: If you would like to add screenshots to your work, please use the the following code;

```
![graphic](graphic.png)
```

The following html code serves to scale-down your graphic.

```
<img src="graphic.png" alt="drawing" width="200"/>
```

## Learning

If you have not done so already, please read all of the relevant [GitHub Guides](https://guides.github.com/) that explain how to use many of the features that GitHub provides. In particular, please make sure that you have read the following GitHub guides: [Mastering Markdown](https://guides.github.com/features/mastering-markdown/), [Hello World](https://guides.github.com/activities/hello-world/), and [Documenting Your Projects on GitHub](https://guides.github.com/features/wikis/). Each of these guides will help you to understand how to use both [GitHub](http://github.com) and [GitHub Classroom](https://classroom.github.com/).

## Testing your assignment
This assignment uses [Docker](https://www.docker.com) and [GatorGrader tool](https://github.com/GatorEducator/gatorgrader) to check whether your assignment satisfies the minimum submission requirements. First, you need to make sure you have installed the [GatorGrader tool](https://github.com/GatorEducator/gatorgrader) to verify that the minimal content of your reflection document satisfies the Desktop](https://www.docker.com/products/docker-desktop) and have it running. Then, you can use you can use the [GatorGrader requirements specified in the lab assignment sheet. To run the GatorGrader application to start `gradle grade` as a containerized application, using the [DockaGator](https://github.com/GatorEducator/dockagator) Docker image available on [DockerHub](https://cloud.docker.com/u/gatoreducator/repository/docker/gatoreducator/dockagator). First, to ensure that the following command will work correctly, you must create the cache directory by running the command `mkdir $HOME/.dockagator`. Then, to see if your submission satisfies the minimal requirements, you can run the following command in the terminal:

```
docker run --rm --name dockagator \
  -v "$(pwd)":/project \
  -v "$HOME/.dockagator":/root/.local/share \
  gatoreducator/dockagator
```

This command will use `"$(pwd)"` (i.e., the current directory) as the project directory and `"$HOME/.dockagator"` as the cached GatorGrader directory. Please note that both of these directories must exist, although only the project directory must contain something. Generally, the project directory should contain the source code and technical writing of this assignment, as provided to a student through GitHub. Additionally, the cache directory should not contain anything other than directories and programs created by DockaGator, thus ensuring that they are not otherwise overwritten during the completion of the assignment.  If the above `docker run` command does not work correctly on the Windows operating system, you may need to instead run the following command to work around limitations in the terminal window:

```
docker run --rm --name dockagator -v "%cd%:/project" -v "%HomeDrive%%HomePath%/.dockagator:/root/.local/share" gatoreducator/dockagator
```

Please note; in the settings of Docker, your virtual drive must be shared for this command to work in Windows.
