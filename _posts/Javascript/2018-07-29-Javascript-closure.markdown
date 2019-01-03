---
layout: post
title: "Closure in Javascript and Jquery"
date: '29 July 2018'
body-class: 'inner-page'
category: 'frontend'
description: 'What is closure in Javascript and some example of it in use'
main-image: 'https://images.unsplash.com/photo-1454486837617-ce8e1ba5ebfe?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=056795a1f5eb8b37cdb673c722d0c7cb&auto=format&fit=crop&w=500&q=60'
---
```
function showName(firstName, lastName){
    var nameIntro = "Your name is ";

    // this inner function has access to the outer functions variables, including the parameters
    function makeFullName(){
        return nameIntro + firstName + ' ' + lastName;
    }
    return makeFullName();
}

showName("Micheal", "Jackson"); // Your name is Micheal Jackson
```