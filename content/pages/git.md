---
title: Upload to a git repository
date: Last Modified
permalink: /upload-to-git/index.html
eleventyNavigation:
  key: git
  order: 20
  title: Upload to a git repository
---

It's recommended you use [GitHub](#using-github) or [GitLab](#using-gitlab) to host the code.

::: warning 
*If you are using an online git repository, please ensure that your repository is set to `private`.*
:::

Your final repository should only contain the following three files:

- `index.js`
- `package.json`
- `package-lock.json`

{% image "git-files.png" "Files uploaded to GitHub" %}

## Using GitHub
If you want to use GitHub as your code repository, you will need to: 

1. Create a new repository ([GitHub docs](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository))
1. Upload files to your GitHub repository. You can do this via the [web interface](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository#adding-a-file-to-a-repository-on-github), or [command line](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository#adding-a-file-to-a-repository-using-the-command-line).

### Using GitHub Desktop
Alternately, you can use GitHub Desktop to create a new repository and upload files. ([GitHub docs](https://docs.github.com/en/desktop/installing-and-configuring-github-desktop/overview/getting-started-with-github-desktop))



## Using GitLab
If you want to use GitLab as your code repository, you will need to: 

1. Create a new blank project ([GitLab docs](https://docs.gitlab.com/ee/user/project/working_with_projects.html#create-a-blank-project))
1. Upload files to your GitLab repository. You can do this via the [web interface](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file), or [command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line).
