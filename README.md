# xllify-starter

This repo demonstrates using the [xllify-build](https://github.com/marketplace/actions/xllify-build) action to package some simple custom functions from [main.luau](main.luau)

This is a template repo so you can create a copy of it and have a ready to build custom function XLL ready to download in about a minute.

## Experiment building an XLL entirely on GitHub

No need for any Windows development setup. Just a browser (and Microsoft Excel for Windows, if you want to download and run your masterpiece.)

This is not a recommended replacement for a development environment with VS Code or similar, but it's enough to give you the gist without installing anthing.

Some familiarity with the GitHub Actions UI is expected but, briefly:

### Initial build

- Create a repo using this one as a template
- Go to the Actions tab, select **xllify Starter** and click on Run
  - This will build an XLL
- Find the workflow run and observe the build
- When the build completes, you can download the xll - it's there as an attached asset
- Unblock the downloaded file and move it out of your Downloads folder. Desktop is fine. More info: https://support.microsoft.com/en-gb/topic/excel-is-blocking-untrusted-xll-add-ins-by-default-1e3752e2-1177-4444-a807-7b700266a6fb
- Double click the .xll to open Excel
- You'll see a dialog box that the add-in has started
- In a new sheet add `xllify.Demo.Hello()` to a cell

### Make a change

- Edit [main.luau](./main.luau) line 10 and change `"Hello there, "` to `"Bonjour, "` (or whatever you like)
- Repeat the process of building, downloading an running the XLL
- Admire your XLL prowess
