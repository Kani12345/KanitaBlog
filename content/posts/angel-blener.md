+++
authors = ["Kanita"]
title = "Angel Project on Blender"
date = "2024-10-14"
description = "Description of my blender project"
+++


<h1 text-align: center> Making an angel on blender </h1>


<img src="/KanitaBlog/posts/cover_angel_article.png" alt="Angel" width=700>


In our blender class, we had to make a 3D object of our liking on blender using the tools we learned in class. I decided to make the biblically accurate angel for aesthetic reasons and also because I thought it involved a lot of blender features: the use of different textures, a complex use of the shadow editor, the use of several transformers (array and path) as well as the animator. 
The textures used are not made by me, I will put them all at the end of the article. 

## The Process 
### Making of the eye 

To make the eyes, I followed this youtube tutorial: https://www.youtube.com/watch?v=1Nkx2CuaREc&t=542s&ab_channel=NiniaIDigitalArt. 
The eye is composed of two objects: the globe and the iris. 

#### The occular globe 
![globe_oculaire](/KanitaBlog/posts/Globe_oculaire.jpg)
<p style="font-size: 10px; padding: 5px;">(Left: solid view, right: material preview)</p>

(Left: solid view, right: material preview)

I followed the tutorial to shape the eye using the tools provided in blender's edit mode. 
The textures provided allowed me to reproduce a realistic visual aspect of the eye with the apparents veins, as well as this glossy effect. Here is a screen shot of how my [shade editor](/KanitaBlog/posts/Shadow_editor.png) was parametered to obtain this result. 

#### The iris 
![Iris](/KanitaBlog/posts/Iris.png)
The textured effect on the iris was sculpted using the transformer (...)
As for the rendering, an image of an Iris was used without doing much on the shadow editor since there will be the cornea of the occular globe above the iris. 

When combining both the glob and the iris, we obtain a realistic looking eyeball: 
<img src="/KanitaBlog/posts/eyeball.jpg" alt="blanc_oeil" width= 300>

### Making of the rings 
To make the rings that will rotate aroun the eye, we need to make golden rings and manage to put small eyes all around it. 

Making the rings without the eyes is pretty easy. I used a cylinder and the binary modifier to obtain this shape:  

To add the eyes all along the rings, I copied the eye we made previously, reduced its size and used the modifier array to obtain the desired number of eyes. To make them stick the ring, I created a circle of the same shape of the ring as a path and made the eyes follow it. 

As for the golden textures, using a pale yellow color and putting the metallic parameter to its maximum is enough to have the desired effect. 

We finnally obtain a realistic looking ring: 
<img src="/KanitaBlog/posts/couronne_2.png" alt="ring" width= 700>



### Animating the angel 
Since it would be weird for this strange looking aangel to stand still, I animated the main eye and the rings to add some movement.
#### Animating the eye 
I made it have typical rapid eye movements with a twist at the end to make it  a bit unsettling, which is fitting for an odd looking angel.
#### Animating the rings 
I made the rings rotate on themselves and around the eyes to ùake the final result more dynamic. 

### Final Result 
<img src="/KanitaBlog/posts/angel.gif" alt="ring" width= 700>




































### Resources 



Here are the textures I used for the globe: 


<img src="http://localhost:1313/KanitaBlog/posts/blanc_oeil.jpeg" alt="blanc_oeil">


![sclera2](/KanitaBlog/posts/sclera2.jpeg)
![sclera](/KanitaBlog/posts/sclera.png)



This is the texture I used for the iris: 








