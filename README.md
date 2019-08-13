# DesignLabUCF.github.io
Main Website for the SENSEable Design Lab.

## Overview
The lab website uses [**Jekyll**](https://jekyllrb.com/) (Simple, blog-aware, static sites generator). The simplest way to edit information on the site is to clone the repository and locally serve the site to generate the static HTML. That static HTML can then be copied over to the 'live' repository **\\web-01\Senseable** on IST servers.

To set up [**Jekyll**](https://jekyllrb.com/) I follow the instructions at [https://jekyllrb.com/docs/installation/ubuntu/](https://jekyllrb.com/docs/installation/ubuntu/) and install it for the *bash for windows client* which is easier than the windows direct installation.

```bash
jekyll serve
```

for production change the <code>URL</code> in the <code>_config.dev</code> to be IST URL.
```bash
JEKYLL_ENV=production jekyll build
```


### Front Page
The front page utilizes <code>index.html</code> as the main driver.
This page utilizes the <code>default</code> layout which you can find in the <code>_layouts</code> folder. The <code>default</code> layout includes <code>head.html</code> and <code>footer.html</code> which takes care of loading the header and footer information uniformly per page. Check those files in the <code>_includes</code> folder if you need to modify anything in the header or footer.

The front page also utilizes a image banner to rotate research images. You can put the new images in the <code>imgs</code> folder and number them <code>00N.JPG</code> or <code>00N.PNG</code>. (Please match the images sizes to what is in the folder.) The code to load the description and new image is found in the <code>_includes</code>  folder and the  <code>slider.html</code> file. You have to copy the <code>div block</code> 


```bash
<div>
   <img data-u="image" src="{{site.url}}/imgs/004.jpg" />
   <div u="thumb">Slide Description 004</div>
</div>
```

### People
(*todo*)

### Publications
(*todo*)

### News Items
(*todo*)
