###BASIC USAGE.
ImgPos is a jquery plugin that lets you load/view a portion of image in an img tag like a background
image property were you can view a portion of an image.Now with this plugin you can do this in an img tag too, with very little js or using the data attribute form you dont even have to write a single line of js.
###<a href="https://riazxrazor.github.io/imgpos/">Demo</a>

```HTML 

         <!-- JUST INCLUDE THE LATEST JQUERY -->
         <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.12.0/jquery.min.js"></script>
         <!-- INCLUDE THE PLUGN -->
         <script src="js/imgpos.jquery.js"></script>

        // and thats it go on use it no need to write javascript as simple as that
        <img data-img-pos="true" data-posx="630" data-posy="400" data-height="350" data-width="350" height="250" src="img/1.jpg" />

```

### CONFIG OPTIONS.
Those who like me love writting js and conifg a plugin an be in control no need to be gloomy, it has a nice liitle config options taht you can initiate from js too. 

```javascript

            $(function(){
               $('img.pos').imgpos({
               height:250,
               width:250
               });
               
               // all config options and default values
                posx:null, // position x from where to start crop from left
                posy:null, // position y from where to start crop from top
                height:null, // height of the crop image 
                width:null,  // width of the crop image
                originx:0,  // normally the origin is top left corner of an 
                originy:0,  // image 0,0 if you change these posx and posx will start from that positon of image 
                posSize:false // if true use crop image height , width as image height and width
               
            });        

```
###<a href="https://riazxrazor.github.io/imgpos/">Demo</a>

Its a simple plugin yet its powerful. Still have to work on some tiny performance issues. Designers will love it i hope.<br>
Anybody want to work on it or improve it please jump right in.
