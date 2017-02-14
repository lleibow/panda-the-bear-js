<!-- 1. Select the element that contains the profile image (hint: look for the class). Change the src attribute so it points to a picture of your choosing instead (hint: use attr()). -->

$('.profile-image').attr('src', 'http://placekitten.com/g/400/400');

<!-- Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing. -->

$('#left-image img').attr('src', 'http://placekitten.com/325/225');

<!-- Select the heading that says "Panda the Bear" and change it to your own name. (hint: use text()) -->

$('.bio-info-name').text("Laura");

<!-- Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector) -->

$('#employment .info-title').html(suitcase).append(' ').append(text1);

<!-- Panda the Bear is lying about their skills! Take the "time travel" skill off the page to satisfy your personal sense of justice. Use your googling and docs-skimming skillz to find a jQuery function that will allow you to remove elements from the DOM. (hint: there are multiple ways of doing this, but the parent() function might be useful when it comes to selecting the right element) -->


$('#time-travel').parent().remove();

<!-- Change the colour of the body. (hint: use css()) -->

$('body').css('background-color', 'black');

<!-- Change the colour used by the highlight class. -->

$('.highlight').css('background-color', 'grey');

<!-- Change the font family of the h1 to 'monospace'. -->

$('h1').css('font-family', 'monospace');

<!-- Find a way to select the round icons in the sidebar and then change their colour. -->

$('.action-icon-bg').css('background-color', 'blue');

<!-- Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself". -->

$('#name').attr('placeholder','I can't see why my having eaten that floor cheese is relevant');

<!-- Change the placeholder attribute of the message field to "state your business". -->

$('#message').attr('placeholder','you are doin a heckin business?');

<!-- Give the name field a "value" attribute of "your nemesis". -->

$('#name').val('Your Nemesis');

<!-- Change the value attribute of the email field to "koalathebear@gmail.com". -->

$('#email').val('koalathebear@gmail.com');

<!-- Change the value of the submit button on the contact form to "En garde!". -->

$('#submit').val('En Garde!');

<!-- We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute). -->

$("#submit").prop('disabled', true);

<!-- That drawing of Pikachu is really cute. Let’s duplicate it using clone() and insert it at the bottom of the .portfolio-container using insertAfter() or appendTo(). -->

$('#right-image img').clone().appendTo( ".portfolio-container" );

<!-- Wow, that was so satisfying I think we should do it 10 more times. Use a for loop to help you do this. -->

for (var i = 0; i<11; i++) {$('#right-image img').clone().appendTo( ".portfolio-container" )}

<!-- Let’s add a message about when the page was last updated. We'll do this by appending a new <li> element to the <ul> in the sidebar (you might need to refresh the page to bring back the list items that we emptied out earlier). -->

$var listItem = document.createElement('li');

$var leftSpan = document.createElement('span');

$var lastUpdated = document.createTextNode('Page last updated on');

$leftSpan.appendChild(lastUpdated);

$listItem.appendChild(leftSpan);

$var d = new Date();

$var rightSpan = document.createElement('span');

$dateNode = document.createTextNode(d);

$rightSpan.appendChild(dateNode);

$listItem.appendChild(rightSpan);
​
$('.bio-info').append(listItem);
[ul.bio-info]
