---
title: "Choose your Jupyter Notebook themes"
date: 2020-02-09
tags: JupyterNotebook JupyterThemes
categories: DataScience
published: true
---

Jupyter Notebook is a powerful tool to create a document containing codes, visualisations and markdown texts. I use Jupyter Notebook on a daily basis and the white screen that comes as a default setting often causes eye strains. 

While finding a solution for this, I came across a library called, `jupyterthemes`. This library enables you to customise your Jupyter Notebook in themes, fonts, plotting and so on. 

### Installation
This can be installed with pip using the following command.
```python
pip install jupyterthemes
```

### Customising Jupyter Notebook theme
Before customising your notebook theme, you can type the following command to see available themes.
```python
jt -l
```
Then you can select a theme you like to apply.
```python
jt -t chestesrish
```

### Further customisation
This library allows you to customise other features beyond the theme. 
This table shows all the command options you can use for customisation.

cl options|arg| default 
:---|:---:|:---:
Usage help|-h|--
List Themes|-l|--
Theme Name to Install|-t|--
Code Font|-f|--
Code Font-Size|-fs|11
Notebook Font	|-nf|--
Notebook Font Size|-nfs|13
Text/MD Cell Font|-tf|--
Text/MD Cell Fontsize|-tfs|13
Pandas DF Fontsize|-dfs|9
Output Area Fontsize|-ofs|8.5
Mathjax Fontsize (%)|-mathfs|100
Intro Page Margins|-m|auto
Cell Width|-cellw|980
Line Height|-lineh|170
Cursor Width|-cursw|2
Cursor Color|-cursc|--
Alt Prompt Layout|-altp|--
Alt Markdown BG Color|-altmd|--
Alt Output BG Color|-altout|--
Style Vim NBExt*|-vim|	--
Toolbar Visible|-T|--
Name & Logo Visible|-N|--
Kernel Logo Visible|-kl|--
Reset Default Theme|-r|--
Force Default Fonts|-dfonts|--

For myself, I customise font sizes and cell width as well as theme.
```python
jt -t chesterish -fs 10 -tfs 10 -ofs 10 -dfs 10 -cellw 1100
```
Note that the commands work on a terminal and you have to restart your Jupyter Notebook to have these setting enabled.

Check out the [github repository] for more features on customisations. 

### Reference
[dunovank. (2018). <i>jupyterthemes</i>. Github]


[github repository]: https://github.com/dunovank/jupyter-themes/blob/master/README.md
[dunovank. (2018). <i>jupyterthemes</i>. Github]: https://github.com/dunovank/jupyter-themes/blob/master/README.md
