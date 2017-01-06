# CSS MEDIA ALL

> A library written in css consisted of media queries to support the responsiveness of webpage.

CMA(Css Media All) makes your webpage responsive, idea behind this library is to make webpage more responsive to differrent screens,
the media queries used in this library is a LIFTOFF from [CSS tricks](https://css-tricks.com/snippets/css/media-queries-for-standard-devices/).


> ### Support
> it is written in vanila CSS and is mostly supported in all major browsers

## Use CMA in your site?

install using npm
```bash
npm install css-media-all --save
```

install using bower
```bash
bower install css-media-all --save
```

clone the git repo

```bash
git clone https://github.com/siddarthvader/CSS-MEDIA-ALL.git
```

Add to your CSS

```bash
import url('css-media-all.css');

p {
    font-size:1rem;// this `rem` unit is now a variable and you can use it the way you want
    padding:0.5rem;
}

```


Add to your html (this is standard setting, in case you forget)

```base
    <meta name="viewport" content="width=device-width, initial-scale=1">
````

>## this is advised that refrain using `rem` in width property, use `%` for width;


## Idea behind it
for years we developers/designers are constantly arguing which is the best unit for css measurements, is it `px` or `em` or `rem` or `vw` or `mm`? nobody has a solid answer to it, because it varies according understanding of developer, but one thing remain unchanged which is rendering of page.

I personally find `rem` to be the best of all, it is relative to the `font-size` of `html` tag, i mean now you have an absolute base unit which is directly dependent on the `font-size` property of `html`, what more can you ask for?

with `rem`, you want to zoom-in your site?
* change the `font-size` of `html` tag?

you want to render your site on mobile viewport but you are not sure about the text size rendering?
* well change the `font-size` of `html` tag?


## Measurements

When it comes to `rem` you have to set the `font-size` of `html` tag, now in this module the default setting goes like this

````bash
| Desktop | Mobile(Portrait) | Mobile(Landscape) | Tab(Portrait) | Tab(Landscape) |
|---------|------------------|-------------------|---------------|----------------|
|  1vw    |       1.5vw      |        1vw        |       1.5vw   |        1vw     |
````

where `vw` is the % of width of view port;

for example:

````bash
    //device width is 1280px
    html{
        font-size:1vw; // meant 12.8px
    }

    p{
        font-size:1.2rem;// (12.8*1.2)
    }
````
