# Q0: Why is this error being thrown?
There is no controller for the Pokemon model.

# Q1: How are the random Pokemon appearing? What is the common factor between all the possible Pokemon that appear? *
The random Pokemon are appearing because in home_controller.rb, there is an "index" method that sets @pokemon to trainerless_pokemon.sample. The common factor between all the possible Pokemon that appear is that they are all chosen from the Pokemons already in the model.

# Question 2a: What does the following line do "<%= button_to "Throw a Pokeball!", capture_path(id: @pokemon), :class => "button medium", :method => :patch %>"? Be specific about what "capture_path(id: @pokemon)" is doing. If you're having trouble, look at the Help section in the README.
The line creates a button with the name "Throw a Pokeball!" and calls the "capture" method on the current pokemon to set the current trainer as the owner of the pokemon. A medium sized button is created, and the method to be used in routes.rb is "patch."


# Question 3: What would you name your own Pokemon?
"Hsiungy"

# Question 4: What did you pass into the redirect_to? If it is a path, what did that path need? If it is not a path, why is it okay not to have a path here?
I passed in the path to trainer, which needed the trainer ID. 

# Question 5: Explain how putting this line "flash[:error] = @pokemon.errors.full_messages.to_sentence" shows error messages on your form.
The flash provides a way to pass temporary primitive types between actions. The error messages that I placed in the flash is exposed to the next action and then cleared out, before redirecting to a display action that can expose the flash to its template.

# Give us feedback on the project and decal below!
The class is straightforward :)

# Extra credit: Link your Heroku deployed app
