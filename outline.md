# Outline

**These notes are for the presenters.**

For the last two years the Jupyter team has been working on the new Jupyter
frontend: JupyterLab. While JupyterLab does of course allow the use of Jupyter
Notebooks, it goes beyond the classic Jupyter Notebook by providing a flexible
and extensible web application with a set of reusable components. Users can
arrange multiple notebooks, text editors, terminals, output areas, and custom
components using tabs and collapsible sidebars. These components are carefully
designed to enable the user to use them together or separately (for example, a
user can send code from a file to a console with a keystroke, or can pop out an
output from a notebook to work with it alone).

JupyterLab is based on a flexible application plugin system provided by
PhosphorJS that makes it easy to customize existing components or extend it
with new components. For example, users can install or write third-party
plugins to view custom file formats, such as GeoJSON, interact with external
services, such as Dask or Apache Spark, or display their data in effective and
useful ways, such as interactive maps, tables, or plots.

In this tutorial we’ll walk users thought the best way to make use of
JupyterLab, how to transition from the “classic” Jupyter Notebook frontend to
JupyterLab, and how to make the best use of the new powerful features of
JupyterLab.

If you have any question and concern or need help, fell free to speak up. A
helper will come see you, or the speaker will take time to get questions.

This can serve as a quick read through summary of what we talked about (with
links) and a rough timeline if you want to follow up on the video later.

## Overview of JupyterLab

### Introduction (1:30, 20 min)

Today this tutorial will be presented to you by Jason Grout, and Matthias
Bussonnier, two long standing members of the Jupyter Project.

By now you should have installed JupyterLab following the instructions in the
readme. For this tutorial, we are standardizing on a conda-based python
distribution (miniconda or Anaconda). We may not be able to help with
installation issues if you are using a different python distribution.

JupyterLab is still evolving, and we are still refining the usability and user
experience. When trying to do any task in an exercise, please let us know if
something was not intuitive, or what surprised you.

- Introduction to JupyterLab (slides)

- FAQ:
  - Why JupyterLab?
  - Can you get Lab and notebook at the same time: YES
  - No difference in file format; Notebooks files are the same

### Tour of User Interface (Jason, 1:50, 30 min)
- Following outline from https://github.com/jupyterlab/jupyterlab-demo/tree/master/narrative or https://gist.github.com/jasongrout/3039b5909734b1abf4544a8df68a8ace

### Installation and Exercise 1 (Matthias, 2:30, 30 min)

Look into the Exercise 1 folder, and follow the instruction in `Exercise-1.md`
  1. Arranging tabs through dragging
  2. How to author markdown and equations
  3. Collapsible cells
  4. drag cells, inside notebook and between views of files.
  5. Enable scrolling on outputs
  6. creating new view of outputs
  7. javascript rendering restrictions

### BREAK + QA 3:00 (15 min)

Write one good thing on the green sticky note, one bad on the red one.

## Workflows around executing code

### Attaching kernels to multiple documents (Matthias, 3:15, 15 min)

1. Executing code in a markdown file using an attached console.
2. Developing libraries with notebook and Python files attached to same kernel
3. Reloading modules?
4. Create terminal, work with terminal next to code file and console. Maybe using ipython in terminal.
5. Attaching a code console to the same kernel as a notebook.

### Exercise 2 (Matthias, 3:30, 15 min)

- binding multiple documents to the same kernel
  - New Console for Notebook
  - Markdown file + console workflow
  - Python code file + console workflow (notice the completions in the python code file!)
  - Open a notebook in classic notebook, modify, save and reopen in Lab.

## Customizing JupyterLab

### Settings (Matthias, 3:45, 10 min)

  1. Changing editor settings
  2. Changing theme
  3. Json config system overview
  4. Changing keyboard shortcuts

### Exercise 3 (Matthias, 3:55, 10 min)
1. change a keyboard shortcut
  1. Assign existing shortcut to new action.
  2. Assign new Keyboard shortcut to an existing action.
2. add a keyboard shortcut (restart and run all)
3. change an editor setting

## Extensions (Jason, 4:05, 30 min)

1. Everything is an extension - show the package.json
2. Installing/listing/enabling/disabling plugins. `jupyter lab build`
3. `--core-mode`
4. Exercise 5 - writing your own extension

## What's new (Jason, 4:35, 25 min)

JupyterLab 0.34 is out. Changes in 0.33 and 0.34 include:
- No longer in beta
- Workspaces
- Extension manager
- Console show outputs
- Open in new browser tab/Copy Down Link
- Text file completions
- Text editor font size
- Theming improvements
- Many, many upgrades

In the works:
- Real-time collaboration

## Widgets workflows

## JupyterLab in JupyterHub
## Community Sprint day Saturday
## Poster session
## User testing
