
var i = 0; // Start Point
var images = []; // Images Array
var time = 1000; // Time Between Switch
var p = 0; //counter of the palys
var next =0
// Image List
images[0] = "https://i.ibb.co/RDkynpX/1-Cropped.jpg";
images[1] = "https://i.ibb.co/2qWTMnC/2-Cropped.jpg";
images[2] = "https://i.ibb.co/pJXx4tz/3-Cropped.jpg";



// Change Image
function changeImg() {
  if (p % 2 == 0){
    document.slide.src = images[i];
  /* Check If Index Is Under Max if less show the next image else start from the bigaining*/
  if (i < images.length - 1) {
    // Add 1 to Index to show the next image
    i++;
  } else {
    // Reset Back To O
    i = 0;
  }
}
  // Run function every x seconds
  setTimeout("changeImg()", time);
}
//add one to the plays counter inj  case the play  boutoun is pressed
function play() {
  p++;
}

//shows the image of the given index 
function showImg(n) {
  document.slide.src = images[n];
}
//show the next or the prev image 
function nextPrevImg(n) {
i=i+n;

if((i <= images.length - 1) && (i >= 0)){
  document.slide.src = images[i]; 
  
}else if(i < 0){
i=images.length - 1;
document.slide.src = images[i];
}else{
i=0;
document.slide.src = images[i];
}
}


document.onkeydown = checkKey; //to take the presed key 

/*this function help us to detect the pressed keys and and act accordingly if should*/ 
function checkKey(e) {
  e = e || window.event;
       if (e.keyCode == '39') {
       nextPrevImg(1);
} else if (e.keyCode == '37') {
       nextPrevImg(-1);
} else if(e.keyCode == '32'){
       play();     
}}


// Run function when page loads
window.onload = changeImg;


//https://codepen.io/hosen-ajbreh/pen/WNeOMMg
