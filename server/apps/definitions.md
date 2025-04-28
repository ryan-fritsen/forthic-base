My Forthic Word Dictionary
---------------
Default Presets

---------------
My Custom Words (wip)
Requires re-definition in-app

---------------
Common Phrases (wip)

1. Load HTML
    "forthic"   BROWSER-FORTHIC html.RUN-FORTHIC.JS html.RENDER
    - dshajk

2. Load a screen
    : BROWSER-FORTHIC   "browser" LOAD-SCREEN  BROWSER-DATA jinja.RENDER;

2. Load external HTML templates into a dataset of variable names
    : MAIN-DATA    [
    "basic_html-v"    "basic_html-f" LOAD-SCREEN
        ] REC;
    - basic-html-v is the variable. This later gets used as a variable for a Flask template, within Forthic.
    - basic-html-f is the File name, which lives in a "screens" folder.
    - Colloquially you can drop the v and f

3. Old style - Render main.forthic page
    : MAIN-PAGE   MAIN-TEMPLATE MAIN-DATA jinja.RENDER;

4. New Style - Render main.forthic page 
    : MAIN-PAGE   FORTHIC-REACT-v1 UI-FORTHIC <FORTHIC;
    - FORTHIC-REACT-v1
    - UI-FORTHIC
    - <FORTHIC>