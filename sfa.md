// colr
$color-card-one: hsl(31, 77%, 52%);
$color-card-two: hsl(184, 100%, 22%);
$color-card-three: hsl(179, 100%, 13%);
//==== background, headings, buttons
$color-primary: hsl(0, 0%, 95%);
$color-paragraph: hsla(0, 0%, 100%, 0.75);

//============== Font Family

$font-primary: 'Big Shoulders Display', cursive;
$font-seconday: 'Lexend Deca', sans-serif;

//============== Font Weight

$weight-bold: 700;
$weight-light: 400;


//============== Converts Pixels to REM

@function rem($size) {
    $remSize: $size / 16px;
    @return #{$remSize}rem;
  }

// ===================================

//============== Make Content Visible To Only Screen Readers

.sr-only {
    border: 0 !important;
    clip: rect(1px, 1px, 1px, 1px) !important;
    -webkit-clip-path: inset(50%) !important;
            clip-path: inset(50%) !important;
    height: 1px !important;
    margin: -1px !important;
    overflow: hidden !important;
    padding: 0 !important;
    position: absolute !important;
    width: 1px !important;
    white-space: nowrap !important;
  }

//============== CSS Reset

// Box sizing rules 
*,
*::before,
*::after {
  box-sizing: border-box;
}

// Remove default margin and padding
* {
  margin: 0;
  padding: 0;
}

// Set core root defaults 
html:focus-within {
  scroll-behavior: smooth;
}

// Make images easier to work with
img,
picture {
  max-width: 100%;
  display: block;
}

// ===================================

//============== Base

body {
    background-color: $color-primary;
    min-height: 100vh;
    max-width: 100%;
    font-family: $font-seconday;
    color: $color-primary;
}

h2 {
    font-family: $font-primary;
    color: $color-primary;
    font-size: rem(30);
}

p {
    font-family: $-font-seconday;
    color: $-color-paragraph;
    font-size: rem(15);
}


//===================== Main Styling Begins

// 

.card {
    background: red;
    max-width: 500px;
    min-height: 200px;
}
