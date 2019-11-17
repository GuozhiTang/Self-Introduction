# GuozhiTang_SelfIntro

This repo is simple a static website for my self introduction whose reference is from [RyanFitzgerald/devportfolio](https://github.com/RyanFitzgerald/devportfolio#projects-section).

This application was deployed on github.io: [GuozhiTang_SelfIntro](https://guozhitang.github.io/GuozhiTang_SelfIntro/)


## Images

By default, the template comes with a number of images, some of which can be kept and others which act simply as placeholders and should be switched. The template contains the following:

* Main background (images/lead-bg.jpg) - this is the main background image provided via [Unsplash](https://unsplash.com/). This can be kept or changed easily by replacing `images/lead-bg.jpg` with your new background (recommended size of at least 1920x1080).
* Favicon (/favicon.ico) - this is the favicon used for the page. Similar to the main bg, this can kept or changed easily by replacing the `favicon.ico` with your new one.
* Project image - these are the images associated with the projects under the project section. These are simply placeholders and should either be replaced or removed.


## Experience Section

The experience section creates a vertical timeline with all your relevant experience. The code for the timeline creation can be found within `js/scripts.js` and is an adaptaion of [RyanFitzgerald/vertical-timeline](https://github.com/RyanFitzgerald/vertical-timeline).

The default format is as follows:

```HTML
<div id="experience-timeline">
    <div data-date="September 2015 – September 2016">
        <h3>Employer Name</h3>
        <h4>Job Title</h4>
        <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur in iaculis ex.
        </p>
    </div>
</div>
```

The data attribute `data-date` is what is used to add a date to the associated timeline point. All that is really required is a wrapping div (i.e. `#experience-timeline`) and nested divs to build the timeline. The h3, h4, and p tags are optional and the contents of the div can be styled however you wish.

To add additional section, simply add additional nested divs under the main wrapping div.


To add additional section, simply add additional `.education-block` elements.

## Contact Section

Since the page is static, I opted to use the awesome Formspree to allow for a contact form without the need for anything else. To use it, you must have the page hosted on a server (loading a basic HTML page won't work) where a referrer header is generated. Also, simply add the email to the action. An example is as follows:

```HTML
<form method="POST" action="https://formspree.io/email@email.com">
    <input type="hidden" name="_subject" value="Contact request from personal website" />
    <input type="email" name="_replyto" placeholder="Your email" required>
    <textarea name="message" placeholder="Your message" required></textarea>
    <button type="submit">Send</button>
</form>
```
For more information on configuration of the contact form or dealing with errors, check out [Formspree](https://formspree.io/).

For a quick tutorial about formspree, check out this [tutsplus tutorial](https://webdesign.tutsplus.com/tutorials/quick-tip-add-a-formspree-form-to-your-static-sites--cms-23870) that covers different aspects and features of the form tool.

## Footer Section

The Footer contains an optional copyright where you can place your name as well as an unordered list of all of your social or coding related profiles. By default it contains Github, Stack Overflow, Facebook, Twitter, and Google Plus. You can add or remove them easily and simply use the Font Awesome icon associated with the social profile you wish to use. For a list of all icons, [click here](http://fontawesome.io/icons/).