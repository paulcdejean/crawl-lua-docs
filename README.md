#Overridable:

###ready()

Called when crawl is ready for user input.

###choose_stat_gain()

Return "s" to train strength. "d" to train dexterity. "i" to train intelligence.

###hit_closest()

Called when "tab" is pressed.

#Autopickup:

###clear_autopickup_funcs()

Clears the currently registered autopickup functions.

###add_autopickup_func(function)

Accepts a function in the form of new_func(item, name). If that function returns true then autopickup will pickup an item. If it returns false than autopickup will not pickup an item.

#Crawl:

###crawl.mpr(string)

Prints the string in the place. Very useful!

###crawl.take_note(string)

Takes a note with the string.

###crawl.process_keys(string)

Does stuff as if a player had pressed those keys, sort of.

###crawl.enable_more(boolean)

True is default. If false then --more-- will never show up.

#You:

###you.turns()

Returns the current turn as a number.

###you.floor_items()

I'm not really sure, but if you have a function like: function at_feet() return iter.invent_iterator:new(you.floor_items()) end

Then you can do: for item in at_feet() do stuff done

###you.hunger()

Returns your current hunger level as a number. 7 = stuffed. 6 = very full. 5 = full. 4 = not hungry. 3 = hungry. 2 = very hungry. 1 = almost starving. 0 = starving.

###you.gourmand()

Returns true if you have gourmand, false otherwise.

###you.where()

Returns your current location in string format. For instance "D:13" or "Temple"

###you.god()

Returns the god you currently worship in string format. For instance "Trog"

###you.hp()

Returns two numbers. The first is your current hp. The second is your max hp.

###you.mp()

Returns two numbers. The first is your current mp. The secondi s your max mp.

###you.poisoned()

Returns true if you're poisoned. Returns false if you're not poisoned.

