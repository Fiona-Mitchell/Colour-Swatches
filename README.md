# Colour-Swatches
Little interactive colour-swatch suggestions, using HTML &amp; CSS


Here's how it turned out: 
<img width="1055" alt="Screen Shot 2020-07-03 at 19 10 41" src="https://user-images.githubusercontent.com/47756305/86490899-f00b3d80-bd60-11ea-900c-2cffe3f256af.png">

Here is how I created the swatch span effect in HTML:
```
<div class="collection-1">
    <div class="swatch1A"></div>
    <div class="swatch1B"></div>
    <div class="swatch1C"></div>
    <div class="swatch1D"></div>
    <div class="swatch1E"></div>
  </div>
```

And the CSS styles to make each div move:
```
.collection-1,{
  float: left;
  width: 20vw;
  padding: 0 20px;
  margin: 30px auto;
  transition: 0.8s;
}


/* SWATCHES SET 1 on HOVER*/
.collection-1:hover{
  transform: rotate(0deg);
  transform-origin: top left;
  transition-duration: 1s;
}

    /* SWATCHES SET 1 on HOVER CHILDREN*/
    .collection-1:hover > div.swatch1A{
      transform: rotate(10deg);
      transform-origin: top left;
      box-shadow: 15px 0px rgba(114, 76, 249, 0.5);
    }

    .collection-1:hover > div.swatch1B{
      transform: rotate(5deg);
      transform-origin: top left;
      box-shadow: 15px 0px rgba(86, 69, 146, 0.5);
    }

    .collection-1:hover > div.swatch1C{
      transform: rotate(0deg);
      transform-origin: top left;
      box-shadow: 15px 0px rgba(202, 125, 149, 0.5);
    }

    .collection-1:hover > div.swatch1D{
      transform: rotate(-5deg);
      transform-origin: top left;
      box-shadow: 15px 0px rgba(248, 150, 216, 0.5);
    }

    .collection-1:hover > div.swatch1E{
      transform: rotate(-10deg);
      transform-origin: top left;
      box-shadow: 15px 0px rgba(237, 246, 125, 0.5);
}
```
