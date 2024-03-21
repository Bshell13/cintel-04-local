# Module 4
## Brandon Shellenberger

### Virtual Environment
```shell
py -m venv .venv
.venv\Scripts\activate
```

### Installing Exteral Libraries
```shell
py -m pip install 'input list of libraries with out quotes'
py -m pip freeze > requirements.txt
```
List of External Libraries<br>
-  altair
-  faicons
-  palmerpenguins
-  pandas
-  pyarrow
-  plotly
-  seaborn
-  shiny
-  shinylive
-  shinywidgets

### Running Shiny Program
```shell
shiny run --reload --launch-browser "name of script file"
```

### Build app to Docs Folder in Repo
```shell
shiny static-assests remove
shinylive export "name of folder" docs
```
This code removes any assets and builds the app in the penguins folder to the docs folder.<br>

### Serve app Locally
```shell
py -m http.server --directory docs --bind localhost 8008
```
Makes sure everything will run correctly before publishing to GitHub Pages.