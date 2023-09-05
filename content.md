# Load a Grades project with Local Setup

If you choose not to use a cloud IDE like Codespaces or Gitpod, then there are many ways to setup the project locally on your laptop.

As a first step, we recommend that you [download and install Visual Studio Code (VS Code)](https://code.visualstudio.com/download). This is the editor integrated into Codespaces and Gitpod.

Once you've done this, you will need to install Ruby and Rails on your computer using the command line (e.g., `Terminal` on MacOS). Good guides can be found on [Go Rails](https://gorails.com/setup/), and we recommend those. Be sure to choose your operating system and version, then follow the instructions carefully. 

Note that our projects are currently setup with Ruby version 3.2.1, so be sure to install that version:

```
asdf install ruby 3.2.1
asdf global ruby 3.2.1
```

Once you have VSCode installed and Ruby on Rails is working, you can download your repository locally by navigating back to your fork of the repository at `github.com/<your-username>/<project-name>`. 

Click the "Code" drop-down button, click the "Local" tab, and click the "HTTPS" option, then copy the `https://github.com/<your-username>/<project-name>` box to your clipboard:

<!-- ![](/assets/launch-local.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1685989213/launch-local_duclmm.png)
{: .bleed-full }

Back in a command line on your local computer, make a new directory to house your course projects, then move into the directory. This example creates a directory in your `home` on MacOS, but you can choose the location and name:

```
mkdir ~/my-appdev-projects

cd ~/my-appdev-projects
```

In the new directory, run:

```
git clone <URL-copied-above>
```

(The `<URL-copied-above>` should look like `https://github.com/<your-username>/<project-name>`.)

This will create a new folder with the name `<project-name>`. 

Open the project in VSCode by opening VSCode then opening the project folder or by simply running:

```
code <project-name>
```

from the current command line.

Once the project is open in VSCode, run `bin/setup` in the integrated terminal, and you are ready to get to work.
