# Poker-Spin-Go-Basic-Stats-Pack
Custom stats I created for Spin-Go analysis in Poker Tracker4 (postgreSQL)

# Stats:


<a href="https://github.com/erikw425/Poker-Spin-Go-Stats-Pack/blob/master/BB%203H%20EV.pt4stat"><b>BB 3H EV.pt4stat</b> -- Calculates expected amount of chips won from the big blind three handed</a>

<a href="https://github.com/erikw425/Poker-Spin-Go-Stats-Pack/blob/master/BB%203H%20EV_Hand.pt4stat"><b>BB 3H EV_Hand.pt4stat</b> -- Calculates expected amount of chips won per hand from the big blind three handed</a>

<a href="https://github.com/erikw425/Poker-Spin-Go-Stats-Pack/blob/master/BB%203H%20Hands.pt4stat"><b>BB 3H Hands.pt4stat</b> -- Calculates amount of hands played from the big blind three handed</a>

<a href="https://github.com/erikw425/Poker-Spin-Go-Stats-Pack/blob/master/BB%20HU%20EV.pt4stat"><b>BB HU EV.pt4stat</b> -- Calculates expected amount of chips won from the big blind two handed</a>

<a href="https://github.com/erikw425/Poker-Spin-Go-Stats-Pack/blob/master/BB%20HU%20EV_Hand.pt4stat"><b>BB HU EV_Hand.pt4stat</b> -- Calculates expected amount of chips won per hand from the big blind two handed</a>

<a href="https://github.com/erikw425/Poker-Spin-Go-Stats-Pack/blob/master/BB%20HU%20Hands.pt4stat"><b>BB HU Hands.pt4stat</b> -- Calculates the amount of hands played from the big blind two handed</a>

<a href="https://github.com/erikw425/Poker-Spin-Go-Stats-Pack/blob/master/BTN%203H%20EV.pt4stat"><b>BTN 3H EV.pt4stat</b> -- Calculates expected amount of chips won from the button three handed</a>

<a href="https://github.com/erikw425/Poker-Spin-Go-Stats-Pack/blob/master/BTN%203H%20EV_Hand.pt4stat"><b>BTN 3H EV_Hand.pt4stat</b> -- Calculates expected amount of chips won per hand from the button three handed</a>

<a href="https://github.com/erikw425/Poker-Spin-Go-Stats-Pack/blob/master/BTN%203H%20Hands.pt4stat"><b>BTN 3H Hands.pt4stat</b> -- Calculates the amount of hands played from the button three handed</a>

<a href="https://github.com/erikw425/Poker-Spin-Go-Stats-Pack/blob/master/ChipsEV_g.pt4stat"><b>ChipsEV_g.pt4stat</b> -- Calculates expected amount of chips won per tournament</a>

<a href="https://github.com/erikw425/Poker-Spin-Go-Stats-Pack/blob/master/SB%203H%20EV.pt4stat"><b>SB 3H EV.pt4stat</b> -- Calculates expected amount of chips won from the small blind three handed</a>

<a href="https://github.com/erikw425/Poker-Spin-Go-Stats-Pack/blob/master/SB%203H%20EV_Hand.pt4stat"><b>SB 3H EV_Hand.pt4stat</b> -- Calculates expected amount of chips won per hand from the small blind three handed</a>

<a href="https://github.com/erikw425/Poker-Spin-Go-Stats-Pack/blob/master/SB%203H%20Hands.pt4stat"><b>SB 3H Hands.pt4stat</b> -- Calculates the amount of hands played from the small blind three handed</a>

<a href="https://github.com/erikw425/Poker-Spin-Go-Stats-Pack/blob/master/SB%20HU%20EV.pt4stat"><b>SB HU EV.pt4stat</b> -- Calculates expected amount of chips won from</a>

<a href="https://github.com/erikw425/Poker-Spin-Go-Stats-Pack/blob/master/SB%20HU%20EV_Hand.pt4stat"><b>SB HU EV_Hand.pt4stat</b> -- Calculates expected amount of chips won per hand from the small blind two handed</a>

<a href="https://github.com/erikw425/Poker-Spin-Go-Stats-Pack/blob/master/SB%20HU%20Hands.pt4stat"><b>SB HU Hands.pt4stat</b> -- Calculates amount of hands played from the small blind two handed</a>

# Columns:

<b>SB_3H_EV -- Calculates expected amount of chips won from the small blind for three handed play</b>

sum(if[tourney_hand_summary.cnt_players=3 and tourney_hand_player_statistics.position=9, tourney_hand_player_statistics.amt_expected_won, 0])

<b>SB_HU_EV -- Calculates expected amount of chips won from the small blind for two handed play</b>

sum(if[tourney_hand_summary.cnt_players=2 and tourney_hand_player_statistics.position=9, tourney_hand_player_statistics.amt_expected_won, 0])

<b>BB_3H_EV -- Calculates expected amount of chips won from the big blind for three handed play </b>

sum(if[tourney_hand_summary.cnt_players=3 and tourney_hand_player_statistics.position=8, tourney_hand_player_statistics.amt_expected_won, 0])

<b>BB_HU_EV -- Calculates expected amount of chips won from the big blind for two handed play</b>

sum(if[tourney_hand_summary.cnt_players=2 and tourney_hand_player_statistics.position=8, tourney_hand_player_statistics.amt_expected_won, 0])

<b>BTN_3H_EV -- Calculates expected amount of chips won from the button for three handed play</b>

sum(if[tourney_hand_summary.cnt_players=3 and tourney_hand_player_statistics.position=0, tourney_hand_player_statistics.amt_expected_won, 0])
