# Hello! I'm known as RealToughCandy online, but you can call me Candy. 

#### Today, you're going to learn the basics of HTML. Even if you've never seen or used HTML before, that's OK! We're going to go through this together slowly and methodically so you can start using the language's building blocks to start building a simple webpage by the end of this lesson. 

##### Prerequisites: Text editor.
---
---
                                             Let's Get started!
----
---

### Perhaps you've heard of HTML, a basic building block of the web. 
HTML, or Hypertext Markup Language, is a sort of digital skeleton that gives a webpage its structure. From paragraphs, to images, to links, HTML can be found everywhere on the web. 

### Take a look at the following image of HTML's paragraph _element_ and note its anatomy. This is what we'll be learning about in today's lesson.


![html tags](http://wwwcodes.com/HTML-Tutorial/lab-images/hb3.png)

(Image used with permission from: http://wwwcodes.com)

Let’s now go over a few HTML tags in detail. 
### A _tag_ is a special kind of syntax used in HTML, consisting of two angle bracketes with a name or character inside it. This is an example of an HTML _video_ tag: 
```<video>```

To make it useful, we’ll need to add some additional info inside the tag. Let’s start by experimenting with _heading_ tags.

# Heading Tags
---
Heading tags come in six sizes, from ```<h1>``` through ```<h6>```. You use both an opening tag ```<>``` and a closing tag ```</>``` with heading elements, which you will see shortly.  

Use the _heading_ element to emphasize certain bits of text. 

# ```<h1>```I’m important! ```</> ```

## ```<h2>``` I’m pretty important, but not as big as the element above me. ```</h2>```

### ```<h3>``` Hi! I’m getting smaller. ```</h3>```

#### ```<h4>``` This is just a test! ```</h4>```

##### ```<h5>``` Getting smaller as the numbers go higher … ```</h5>```

###### ```<h6>``` This is as small as the headings get. ```</h6>```



# The anchor tag. 
---
An _anchor_ is a tag that brings you to a certain place on the webpage, or another webpage.
An anchor is created using the ```<a>``` tag. 
If you want to create an anchor called _CustomerService_, you simply add this line where you want the anchor to be:

```<a name="CustomerService"></a>``` 


After doing this, you can make a link pointing to the anchor using the normal ```<a href>``` tag, like this:

Click ```<a href="CustomerService"> here </a> to read about our Customer Service policy``` 

The anchor tag, now linking to an external page: 
##### For more information about our customer service here at Amazon, please visit ```<a href= "http:/www.amazon.com/customerservice">``` [Amazon's Customer Service page](http://www.amazon.com/customerservice) ```</a>. ```

#### In summary, to link to an anchor you need to: 
**-Create a link pointing to the anchor**

**-Create the anchor itself.**




# The image tag. 
---
With all this text, let’s add some images. For this, we’ll use the ```<img>``` tag.The ```<img>``` tag defines an image in an HTML page. It has two required attributes: _src_ and _alt_. The _src_ attribute requires the source of the file, while the _alt_ attribute requires a brief text description of the file for screen readers, an assistive technolgoy. 
In action: 
Let’s show a picture of a cute cat. Two things to note: 
 1. Just like with the anchor tag link, our link to our cat needs to be in quotes, either single or double (your choice). 
 2. Unlike _divs_, _headings_, and _anchor_ tags, there is no closing tag with ```<img>```. 
 ```<img src=‘http://www.photos-public-domain.com/wp-content/uploads/2011/01/orange-and-white-cat-closeup.jpg’ alt='cute cat'>```

When opened in a browser, the result is a cute cat: 

![cute cat](http://absfreepic.com/absolutely_free_photos/small_photos/cute-yellow-cat-4272x2848_43158.jpg)




# The video tag. 
---

#### Let’s take a look at the video tag. 

The ```<video>``` tag specifies the presence of a video, like a a movie clip.
There are three supported video formats for the ```<video>``` element: MP4, WebM, and Ogg. 
In action: 
 
 ```javascript 
 <video src='http://clips.vorwaerts-gmbh.de/big_buck_bunny.mp4'> 
 Bummer, your browser does not support embedded videos!
 </video>
 ```
#### Note that there we added an error message if the user’s browser doesn’t support the ```<video>``` tag. 

# Finally, let's look at the _div_ tag. 

 A _div_ is yet another kind of HTML **element**. A div declares a division (or section) in an HTML document and is the generic container for flow content. When you have similar content that can be separated in blocks, use ```<div>```. _Note, there is a similar tag called ```<span>``` that you will see often, but that is used for inline content. More on that in the next lesson._
```
<div>
<h1> I’m a heading! Yay elephants! </h1>
<p> I’m a paragraph that talks about the heading! Elephants came about thousands of years ago... </p>
</div>
```
  
### Congratulations! You completed Lesson 1. There are a lot more things to learn in HTML, but for now, you can start to build a simple web page just by using the material we covered today. 
