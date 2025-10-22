# xllify-starter

This repo demonstrates using the [xllify-build](https://github.com/marketplace/actions/xllify-build) action to package some simple custom functions from [main.luau](main.luau)

This is a template repo so you can create a copy of it and have a ready to build custom function XLL ready to download in about a minute (depending on how fast the runner your build lands on is - it can vary.)

Slightly more sophisticated demos are available in the [xllify-demo](https://github.com/acornsoftuk/xllify-demo) repo. You can download a built XLL straight from the releases page.

## Get started, entirely on GitHub

No need for any installation or Windows development setup. Just a browser (and Microsoft Excel for Windows, if you want to download and run your masterpiece.)

This is not a recommended replacement for a development environment, but it's enough to give you the gist without installing anthing.

Some familiarity with the GitHub Actions UI is helpful but, briefly:

### Initial build

- [Use this template to create your own repository](https://github.com/new?template_name=xllify-starter&template_owner=acornsoftuk)
- Go to the Actions tab, select **xllify Starter** and click on Run workflow
  - This will build an XLL
- Find the workflow run and observe the build, should take about 40 seconds - **this'll count towards your free GitHub Actions minutes (consumed at 2x)** 
- When the build completes, click on **Summary** and scroll to the artifacts section. You can download the xll, it's attached!
- Unblock the downloaded file and move it out of your Downloads folder. Desktop is fine. More info: https://support.microsoft.com/en-gb/topic/excel-is-blocking-untrusted-xll-add-ins-by-default-1e3752e2-1177-4444-a807-7b700266a6fb
- Double click the .xll to open in Excel
- You'll see a dialog box that the add-in has started
- In a new sheet add `xllify.Demo.Hello()` to a cell

### Make a change

- Edit [main.luau](./main.luau) line 10 and change `"Hello there, "` to `"Bonjour, "` (or whatever you like)
- Repeat the process of building, downloading an running the XLL
- Admire your XLL prowess
