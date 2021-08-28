---
layout: descrip
title: Onomatic
description:
img: /assets/img/3.jpg
importance: 2
category:
---

Onomatic is a tool that utilizes sound to teach language. Deriving from onomatopoeia, the formation of a word through the phonetic imitation of the sound it makes, this system focuses on listening and speaking tools to help users learn.

Each language class comes with lessons tailored toward specific scenarios. A lesson comes with a set of cards. The card can vocalize the new word, an example sentence, part of speech, etc. in both the native and target languages. To support the sound, a visual aid is also provided in the form of an image depicting said word on the card. Likewise, the importance of word formation is also emphasized and used to help the user remember words long term. Memory devices linking the language back to their own native language, user-generated memory, roots of words, and similar words are examples of information that can be stored for each specific card or phrase.

On each card, you can hear the word, hear a sentence with the word, and toggle back and forth between languages. Users can also create their own lessons, with all of the same features available to them. Additionally, users can jot down notes on the word or memory devices, either by recording their cues or typing them. Users create accounts to track progress on their favorite sets and follow lesson plans.

If comparing Onomatic to existing systems, this application takes existing elements from Duolingo and Quizlet, such as flashcards and language learning. However, it adds additional features tailored towards introductory language learners focusing on vocabulary. Onomatic will also provide a core feature allowing for users to record their own audio for phrases, sentences, definitions, and more. Each user-created audio recording will come with information about where the speaker comes from and what type of accent or dialect is used by the speaker. 

Eventually, a question and answer type interface will be integrated into the website. The focus of the interface will be elicitations with other users. For example, one user could ask for someone to say a specific phrase or sentence in a certain dialect or accent, and other users could reply with a recording of their own voice.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/1.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/3.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/5.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/5.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal it's glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/6.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/11.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/" target="_blank">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/6.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/11.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
```
