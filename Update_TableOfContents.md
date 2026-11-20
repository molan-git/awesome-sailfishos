# Updating the Table of Contents

This repository uses [doctoc](https://github.com/thlorenz/doctoc) to automatically generate and update the Table of Contents (TOC) in `README.md`.

To update the TOC after adding, removing, or changing headings, follow these steps:

## 1. Clone the repository

    git clone https://github.com/molan-git/awesome-sailfishos.git
    cd awesome-sailfishos

## 2. Install doctoc

    npm install -g doctoc

## 3. Generate the Table of Contents

Run the following command in the repository directory:

    doctoc README.md

Doctoc automatically scans the Markdown headings and updates the TOC between the following markers:

    <!-- START doctoc -->
    ...
    <!-- END doctoc generated TOC please keep comment here to allow auto update -->

**Important:** Keep these markers in the README. Doctoc uses them to identify the section that needs updating.

## 4. Commit and submit the changes

If you don't have write access to the original repository, fork it on GitHub first.

After updating the TOC, commit and push your changes to your fork:

    git add README.md
    git commit -m "Update table of contents"
    git push

Finally, open a Pull Request against the original repository so the changes can be reviewed and merged.

**Note:** Only the generated TOC needs to be updated. Doctoc automatically takes care of the links and heading structure.
