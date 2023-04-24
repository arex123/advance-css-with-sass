/* clip-path:polygon(x y, x y, x y, x y);  it behave as clockwise direction  */

    clip-path: polygon(0% 0%,100% 0%,100% 80%,0 100%);



/* how to make traingle */

    clip-path: polygon(50% 0,50% 0, 100% 100%, 0 100%);

create a right arrow 

    just go to clipy css website 😒



    /* clip-path: polygon(0% 20%, 60% 20%, 60% 0%, 100% 50%, 60% 100%, 60% 80%, 0% 80%); */



/* below line will create color changing effect from one color to another (#55c57a  -> #28b485) from top left "to right bottom" , and in order to show img we have decreased the color opacity */

    background-image:linear-gradient(to right bottom,#7ed56f44,#28b48547), url(../img/hero.jpg); 



<br>
<br>

<br>


  ## keyFrames , Transfomr, move texts like animation in horizontal manner

below code applies for a text to animate it to move from:<br><br>
 left(-100px) position to original position to 10px right position

 and in start of page loading its opacity will be 0 then after animation its opacity will be 1(visible)

    @keyframes moveTextToLeft{
    0%{
        opacity: 0;
        transform: translateX(-100px);
    }

    80%{
        transform:translate(10px)
    }

    100%{
        opacity: 1;
        transform: translateX(0);
    }
    }

To use above code we will add its name(moveTextToLeft) to that element in css


    .heading-primary-main{
        font-size: 60px;
        font-weight: 400;
        letter-spacing: 35px;
        
        animation-name: moveTextToLeft;
        animation-duration:1s;
    }



    animation-timing-function: ease-out; 


    animation-delay: 3s; /* this will start animation after 3 seconds*/
    animation-iteration-count: 2; /*number of times animation happens*/



## section 2, lec 9

* what pseudo-elements and pseudo-classes are;
* How and why to use the ::after pseudo-element
* How to create a creative hover animation effect using the transition property