[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/IJi-El-s)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=14954787&assignment_repo_type=AssignmentRepo)

# Project Overview

we discussed which goal we wanted to take on and decided to go with goal 14. We wanted the storytelling to be short and precise which we hope would make the user interested. The initial goal is to make the user more interested so they click the read more link which links to the UN´s own website, which goes a bit more into to detail for the specially interested. The way we make it interesting is by having a storytelling website which talks about the important parts.

## brainstorming session

We came up with the idea of making it so the storytelling appears when moving down the ocean. The brainstorming session was very short so we both agreed pretty quickly how we wanted to handle this project

## Storyboard

![paper with a storyboard for the website](assets/storyboard.pdf "storyboard") the markings on the sides of the site represents the margin for the `P` elements.

## Instructions

The site is quite easy to navigate since it is only up and down. One scroll downwards will automatically take you to the next section, same goes for scrolling upwards, just make sure to read the text before scrolling. Link to [pages](https://advancedcss2024.github.io/idg1292-2024-oblig3-group07/)

## Techonology 

### Animations

@keyframes cloudGlide {
    0% {
        transform: translateX(-95vw);
    }

    100% {
        transform: translateX(80vw);

    }
}

@keyframes fishSwim {
    0% {
        transform: translateX(60vw);
    }

    100% {
        transform: translateX(-60vw);
    }
}


@keyframes moveWave {
    0% {
        transform: translateY(0);
    }

    50% {
        transform: translateY(1vw);
    }

    100% {
        transform: translateY(0);
    }
}

these are all animations which make the selected element move in certain direction. we did not want everything to move the same which is why we made different types of movement for the different elements.

our script makes it so the `<p>` element appaers when the user has scrolled down the page, we do this by adding **active** to the class which then triggers a css tranformation. here is how we set up the css.

.reveal{
    position: SpeechRecognitionAlternative;
    transform: translateY(50px);
    opacity: 0;
    transition: all 3s ease;
   }
   
.reveal.active{
       transform: translate(0px);
       opacity: 1;
   }


