# A TodoMVC built with Rails, Turbolinks and boosted with Stimulus

This is a **modest** attempt to create a TodoMVC with Rails, Turbolinks and boost it a bit with Stimulus.
This project was inspired by [this project](https://github.com/nateberkopec/todomvc-turbolinks) : a TodoMVC built with Rails and Turbolinks 3

## The concept behind

The goal of this project was primarily to get more familiar and practice with the new [Stimulus](https://github.com/stimulusjs/stimulus) framework.
The approach taken in this project is to make most of the actions on the todolist client side with Stimulus controller **to get this crisp and fast feeling of client side rendering**.
This Todolist preserves the data in a database within the backend. Each action is therefore linked to a call to the backend to update the content in the database. Those calls are form post submission to keep strong parameters (an alternative could be Ajax post).
As a return from the backend, the page is silently refreshed by Turbolinks. Unless there is a problem persisting the data in the database the refresh is not visible as it is the same as what has already been done by Stimulus controllers.

This is probably not an approach that I would take in production but for this purpose of demo, it does make the job!

## Demo

A live demo is available at: https://todomvc-rails-on-stimulus.herokuapp.com/

As a comparison you can also test the Turbolink 3 only: https://todomvc-turbolinks.herokuapp.com/

## Todo

🚧 WORK IN PROGRESS

* [x] Fix Turbolinks blinks and path change
* [x] We are talking about speed here, score a 100 at Google page speed 💯
* [ ] fix Turbolinks scrolling back to top instead of keeping the current scroll position
* [ ] Add a new todo client side
* [ ] Split the Todo controller in smaller controllers that communicate between each others
* [ ] Add tests

## Disclaimer

This is not intended to be a perfect example of how to use Stimulus, Rails and Turbolinks in a production environment. This is solely an exercise to practice this new Framework and to confirm how well it pairs with Rails and Turbolinks.

## Credits

Lots of inspiration from this great project that got me started
[A Turbolinks 3 TodoMVC](https://github.com/nateberkopec/todomvc-turbolinks)

Many thanks for all Q&A in the Stimulus issues
