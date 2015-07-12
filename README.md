#Overridable:

###ready()

Called when crawl is ready for user input.

###choose_stat_gain()

Return "s" to train strength. "d" to train dexterity. "i" to train intelligence.

###hit_closest()

Called when "tab" is pressed.

###c_kill_list(???)

Unknown.

###c_interrupt_activity(???)

Unknown.

###ch_stop_running(???)

Unknown.

###ch_start_running(???)

Unknown.

###c_assign_invletter(???)

Unknown.



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

###you.hunger_name()

Returns a string indicating your current level of hunger.

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

###you.race()

Returns a string that is the full name of your choosen race. For instance "Vampire"

###you.mutation(string)

Returns true if you have the provided mutation, and false if you don't have the provided mutation.

###you.num_runes()

Returns the number of runes you've collected.

###you.have_orb()

Returns true if you have the orb of zot ins your posession. False otherwise.

###you.xl()

Returns your current experiance level as a number.

###you.transform()

Returns your current form. For example: "bat" "lich" "dragon"

###you.berserk()

Returns true if you're berserk. False if you're not berserk.

###you.confused()

Returns true if you're confused. False if you're not confused.

###you.silenced()

Returns true if you're silenced. False if you're not silenced.

###you.status()

Not sure.

###you.exhausted()

Returns ture if you're exhuasted. False if you're not exhuasted.

###you.mesmerised()

Returns true if you're mesmerised. False if you're not mesmerised.

###you.piety_rank()

Retruns a number that reflects your piety in some way.

###you.regenerating()

Not sure.

###you.anchored()

Returns true if you're dimensionally anchored by the monster spell.

###you.hasted()

Returns true if you're hasted. False otherwise.

###you.slowed()

Returns true if you're slowed. False otherwise.

###you.caught()

Returns true if you're caught by a net or web or something. False otherwise.

###you.see_cell(x, y)

Not sure but I'd really like to know!

###you.ability_table()

Not sure.

###you.extra_resistant()

Not sure.

###you.teleporting()

Returns true if you're about to teleport. False otherwise.

###you.base_mp()

Not sure.

###you.poison_survival()

Not sure.

###you.mighty()

Returns true if you're mighty. False otherwise.

###you.res_fire()

Returns your current level of fire resistance as a number.

###you.res_cold()

Returns your current level of cold resistance as a number.

###you.flying()

Returns true if you're flying. False otherwise.

###you.constricted()

Returns true if you're constricted. False otherwise.

###you.skill(string)

Returns your current skill level in the provided skill as a number.

###you.corrosion()

Returns a number having to do with your current level of corrosion.

###you.res_shock()

Returns your current level of electricity resistance as a number.

###you.have_rune()

Returns true if you have the provided rune. False otherwise.

###you.silencing()

Different from you.silenced()???

###you.temp_mutation(string)

Not sure.

###you.rooted()

Returns true if you're rooted. False otherwise.

###you.see_cell_no_trans(x,y)

Not sure.

###you.strength()

Returns two numbers. Your current strength and your max strength.

###you.intelligence()

Returns two numbers. Your current intelligence and your max intelligence.

###you.dexterity()

Returns two numbers. Your current dexterity and your max dexterity.

###you.train_skill(string, number)

Not sure.

###you.can_train_skill(???)

Not sure.

###you.base_skill(???)

Not sure.

