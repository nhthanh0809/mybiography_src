## My personal biography source code 


This repo is inspired from below links:
1. https://lakemper.eu/blog/getting-started-with-hugo-academic-and-github-pages/
2. https://github.com/smahesh2694/academic-kickstart
3. Academic Kickstart: The Template for [Academic Website Builder](https://github.com/wowchemy/starter-hugo-academic)


## Prerequisites

### I. Installing hugo extended version by downloading it from [Hugo releases website on GitHub](https://github.com/gohugoio/hugo/releases)

#### For window
Download hugo_extended_XXX.0_windows-amd64.zip

#### For Ubuntu
Download hugo_extended_XXX.0_linux-amd64.deb

### II. Installing golang-go

#### For Window

Prefer to https://go.dev/doc/install

#### For Ubuntu
```bash
sudo apt install golang-go
```

## Instruction for building-up 

### Step 1: Clone this repo

```bash
git clone git@github.com:nhthanh0809/mybiography_src.git
```
Note: Please check your git authentication [SSH-key connection](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)

### Step 2: update submodule of Hugo Academic Theme

```bash
cd mybiography_src
git submodule update --init --recursive
```

### Step 3: Building-up static website by hugo

#### For running on local machine
Running command
```bash
hugo server
```
Then open http://localhost:1313 on your browser

#### For running on Github page

Running command for building the static website
```bash
hugo
```
This command will create "public" directory on your repo. \
Please commit all content inside this directory to your github page repo. \

## Note
### 1. Error in displaying your website on github page
Please change "baseurl" line in ./config/_default/config.toml to your website address 
Example:

```
# The URL of your site.
# End your URL with a `/` trailing slash, e.g. `https://example.com/`.
# baseurl = "https://nhthanh0809.github.io/mybiography/"
baseurl = "https://nhthanh0809.github.io/mybiography/"
```



### License
Released under the [MIT](https://github.com/sourcethemes/academic-kickstart/blob/master/LICENSE.md) license.
