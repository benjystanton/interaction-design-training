# Accessibility for designers

A guide to web accessibility best practices for designers.

## Contents

- [Images](#images)
- [Typography](#typography)
- [Colour](#colour)
- [Interaction](#interaction)
- [Forms](#forms)
- [Content](#content)

## Images

### Images of text
Avoid having images of text, especially when it makes up part of the interface. If possible, recreate images using [HTML](http://www.w3schools.com/html/html_intro.asp) and [CSS](http://www.w3schools.com/css/).

In some cases, images that contain text are appropriate. For example a photo of a building or a screenshot of an app might contain some text. If the text is important to the meaning of the image, be sure to include it as alt text somewhere.

[The big problem with sharing text in images](https://blog.ghost.org/text-images/)

### Images should have alt text (alternative text)
Alt text is one of those web jobs that falls through the cracks. Whose responsibility is it? Designers? Developers? Content editors? I suggest that you do everyone a favour and write alt text for any image that you create or supply.

Images that add meaning to the content need to have alt text. Imagine you are explaining the image down the phone to someone who can’t see it.

[Writing effective alt text for images](http://www.webcredible.com/blog/writing-effective-alt-text-images/)

## Typography

### Measure or line length
Long lines of text are hard to read. So are very short lines. As a rule of thumb, I try to keep line length within 45 to 75 characters per line. This is extra tricky when it comes to responsive web design.

[Trent Walton’s trick for managing line length](http://trentwalton.com/2012/06/19/fluid-type/)

### Justified text
Justified text is when all the lines are stretched to fill the entire width of the column. Like in a newspaper. Don’t use justified text. Having ragged (uneven) lines on the right edge helps our eyes when we read. Justified text is harder to read, and these effects can be exaggerated for users who have visual or cognitive access needs.

[Never justify type on the Web](http://designforhackers.com/blog/never-justify-type-on-the-web/)

### Line spacing
Make sure the vertical white space between lines of text is enough so that the taller letters don’t bump into each other. It’s also possible to have too much space. If you’re eye is drawn the gaps between lines instead of the text itself then you probably need to reduce your line spacing a little.

[Line spacing](http://practicaltypography.com/line-spacing.html)

## Colour

### Don’t use colour alone to give meaning
Users who are colour blind can miss out on important information if you don’t consider their needs when designing. For example, if you highlight a required form field with a red outline, this will be invisible to some people.

[Colour accessibility](https://24ways.org/2012/colour-accessibility/)

### Colour contrast
Text must have contrast ratio of at least 4.5:1. Larger text doesn’t need as much contrast. A contrast ratio of at least 3:1 is enough for anything over 18 point.

Good displays like those on Macbook Pros have much higher contrast than most monitors. Test your design on an average, low-res monitor or display, whilst squinting. That should give you a better idea of how some users struggle to read low contrast interface text.

Very light text is overused by designers. We rely on it, because contrast can balance a design. But, if you have to add very light text to a design in order for it to feel balanced then you probably have too much stuff on the page.

[Colour contrast checker](http://webaim.org/resources/contrastchecker/)

## Interaction

### Design a style for keyboard focus
Some users will navigate a website using only a keyboard. But often it’s impossible to tell which elements are currently in focus. Be sure to to give links, buttons and form elements a high contrast focus style.

[Tip: go to GOV.UK and press the tab key a few times](https://www.gov.uk/) to see a good example of this in practice.

## Forms

### Labels
Form elements should always have labels. It’s not enough to use placeholder text as it’s usually very light. It also disappears then users’s select the form field.

### Help text
Add useful instructions to help users to complete the form. If a certain date format or password length is required, let users know. If a field is optional consider removing it, if that’s not possible, mark it as optional.

### Validation errors
Design errors that are easily understood (this includes writing good content too). Make sure they allow users to navigate to the problem and fix it easily.

[The 10 commandments of good form design on the web](http://mono.company/journal/design-practice/the-10-commandments-of-good-form-design-on-the-web/)

## Content

### Avoid technical terms, abbreviations and jargon
Technical terms, abbreviations and jargon can be off putting to all sorts of users:

- users who don’t speak English as a first language (English is a second language for British Sign Language users)
- users who have a low reading age
- newcomers to the topic you are writing about

You can help everyone understand your content better if you use common and simple words.

If you absolutely have to use these words then explain them using the `<abbr>` element or by adding a glossary.

[Stop your team using technical terms and jargon](http://www.disambiguity.com/stop-your-team-using-technical-terms-and-jargon/)

### Readable page titles and hackable urls
Page titles should be descriptive and should match the `<h1>` (main heading) on the page. This helps users to orientate themselves.

Urls should be designed so that users could guess how to navigate their way through a site by editing the website url in the browser address bar.

[Web accessibility & urls](http://simplyaccessible.com/article/web-accessibility-and-urls/)

### Buttons and links should have descriptive labels
Users often scan pages quickly to look for links on a page. This can be done visually or by using screen readers. Don’t use receptive or vague link labels like “read more” or “click here”. They don’t offer any information to the user when taken out of context.

Make sure link and button labels describe what will happen when someone selects them. For example, if they link to a download tell the user the file type and file size.

[Writing content for everyone](https://gds.blog.gov.uk/2016/02/23/writing-content-for-everyone/)

## Conclusion
Everyone benefits from good accessible design. Think about it all of the time. It’s not a separate thing that can be added at the end of a project.

Designers often put up barriers to users with access needs without really meaning to. Don’t be one of those designers.

## Further reading on accessibility
- [Government Digital Service Accessibility](https://accessibility.blog.gov.uk/)
- [WebAIM's WCAG 2.0 Checklist](http://webaim.org/standards/wcag/checklist)
- [Vox Media’s Accessibility Guidelines](http://accessibility.voxmedia.com/)
- [7 Things Every Designer Needs to Know about Accessibility](https://medium.com/salesforce-ux/7-things-every-designer-needs-to-know-about-accessibility-64f105f0881b#.tu5t4zg4m)
