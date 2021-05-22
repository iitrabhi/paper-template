# paper-template
This is a latex template to write research papers.

## Clean working with windows

On a mac when we use the `-ouput-folder` key in sublime-project, all the build files are written to that output folder. But that does not happen on windows. For windows we need to install Perl and then add a few lines of code to the User setting of LaTeXtools under the `builder-settings` key.

```
"windows" : {
			// See README or third-party documentation
        	"script_commands":
                ["latexmk -pdf -outdir=build -auxdir=build -f  -interaction=nonstopmode -synctex=1 "]
		},
```

Download Perl form [here.](https://strawberryperl.com/)

---

To have a clean build, build with script using the key combination: `ctrl+shift+b`

