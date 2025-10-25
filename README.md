## A Terminal-Style Minimalist Website & Blog

Welcome to `template`, a project designed for those who appreciate the simplicity of the command line. 
This repository provides a terminal-style personal website and blog template with **zero graphical overhead** and a focus on straightforward content creation.

---

## Features

* **Terminal Aesthetic:** A classic command-line interface.
* **Zero-Friction Blogging:** Publish new content simply by writing a **Markdown** file.
* **Automated Content Management:** A GitHub Workflow for handling blog posts.
* **Fast & Light:** With no heavy assets or graphics.

---

## Getting Started

This template is designed for quick deployment, ideally on platforms that integrate with GitHub, such as GitHub Pages.

1.  **Fork or Clone** this repository:
    ```bash
    git clone https://github.com/tucob97/template.git
    cd template
    ```
2.  **Customize** the main HTML and CSS files to personalize your site links and primary content.
3.  **Deploy** the project to your chosen hosting service (e.g., enable GitHub Pages for the repository).

---

## Publishing a New Post

The core comfort of this project is the simplicity of publishing. Follow these steps to put your thoughts online:

1.  Write your post as a markdown file.
2.  Put it into the **`blogpost/`** directory..
4.  **Commit and Push** the update repository to your GitHub repository.

That's it! The automation takes care of the rest.

---

## How It Works (The Automation)

You don't need to manually update post lists or compile files.
The repository leverages **GitHub Workflows** to manage your content pipeline automatically:

1.  **Trigger:** Any push to the repository triggers the workflow.
2.  **Indexing:** The workflow scans the `blogpost/` directory for all `.md` files and compiles their names into the master index file: **`POSTLIST.txt`**. This file acts as the "database" or table of contents for your blog.
3.  **Page Generation:** For every new Markdown file, the workflow automatically generates the corresponding static **HTML page** that renders the content in the terminal style, making it viewable on your website.