#1140-sass README
## What?
A collection of [SASS mixins](http://sass-lang.com/) (specifically, SCSS) to allow you to easily and more-sematically use [1140.gs](http://cssgrid.net/)
## Why?
Because using non-semantic, strictly-presentational grid classes like `<div class="fourcol last">` rubs me the wrong way, and because SASS is *awesome*. 

It rubs [tjschuck](https://github.com/tjschuck) the wrong way too, and [his implementation for 960.gs](https://github.com/tjschuck/960-sass/) made me want something similar.

##How?
    @import "1140";

    div.bottom-section {
      @include container;
    }

    div.bottom-inner {
      @include row;
    }

    div.articles {
      @include column(8);
    }

    div.sidebar {
      @include column(4);
    }

