# Global Variables

## global.plot
In UT/DR global.plot is a `float` used to determine where in the plot the game is in, 0 being the start. 

### Example Usage
```js
if (global.plot < 12)
    global.plot = 12;
```
## global.flag
global.flag is an `array` used for pretty much anything that can happen. From decisions to storing specific values flags can be extremly diverse with their usage.


### Example Usage

```js
if (global.flag[23])
    global.flag[920]++
```

<details>
<summary>All Flags in UNDERTALE</summary>

The following data is sourced from [tomat.dev](https://tomat.dev/undertale/flags)

Volatile values are flags that are changed often at runtime, so not easy to manually set. 

Bool values are true/false conditions. 

Range values can be any number. 

Counter values increment as the condition is met.

<table>
    <tbody><tr>
        <th>Flag</th>
        <th>Name</th>
        <th>Type</th>
        <th>Comments</th>
    </tr>
    <tr>
        <td>1..3</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>4</td>
        <td>undyne_trigger_override</td>
        <td>debug bool</td>
        <td>
            When 1, upon encountering Undyne, she will treat you as if you killed no monsters, even if you killed one.
        </td>
    </tr>
    <tr>
        <td>5</td>
        <td>fun</td>
        <td>range</td>
        <td>Chosen randomly when you start a new run, set to 0 after specific events.</td>
    </tr>
    <tr>
        <td>6</td>
        <td>hardmode</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>7</td>
        <td>true_pacifist</td>
        <td>bool</td>
        <td>Post-Asriel fight status.</td>
    </tr>
    <tr>
        <td>8</td>
        <td>disable_random_encounters</td>
        <td>bool</td>
        <td>Receive Undyne's letter or kill Mettaton Neo. Needs confirmation if it works when set manually.</td>
    </tr>
    <tr>
        <td>9</td>
        <td>unaccessed</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>10</td>
        <td>spared_last</td>
        <td>volatile bool</td>
        <td></td>
    </tr>
    <tr>
        <td>11</td>
        <td>escaped_last</td>
        <td>volatile bool</td>
        <td></td>
    </tr>
    <tr>
        <td>12</td>
        <td>killed_last</td>
        <td>volatile bool</td>
        <td></td>
    </tr>
    <tr>
        <td>13</td>
        <td>bored_last</td>
        <td>volatile bool</td>
        <td>Let the battle take too long. Occurs only in the ruins.</td>
    </tr>
    <tr>
        <td>14</td>
        <td>status_dummy</td>
        <td>range</td>
        <td>
            0 if you run away from the Dummy; 1 if you kill it; 2 if you talk to it, 3 if you bore it. The Mad Dummy's
            dialogue will be affected.
        </td>
    </tr>
    <tr>
        <td>15</td>
        <td>in_battle</td>
        <td>volatile bool</td>
        <td></td>
    </tr>
    <tr>
        <td>16</td>
        <td>type_heart_transition</td>
        <td>volatile bool</td>
        <td>Occurs when triggering "quick" battles (i.e. Undyne's spears, lasers).</td>
    </tr>
    <tr>
        <td>17..18</td>
        <td>unaccessed</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>19</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>20</td>
        <td>animation_index</td>
        <td>volatile range</td>
        <td></td>
    </tr>
    <tr>
        <td>21</td>
        <td>cooked_noodles</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>22</td>
        <td>name_color</td>
        <td>range</td>
        <td>
            Set when you talk to the frog in the ruins. When sparing monsters: 0 for yellow names, 1 for white, 2 for
            pink. Also a small easter egg in the trash area if not equal to 0.
        </td>
    </tr>
    <tr>
        <td>23</td>
        <td>spared</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>24</td>
        <td>escaped</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>25</td>
        <td>dialogues_skipped</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>26</td>
        <td>murderlevel_override</td>
        <td>debug range</td>
        <td>If set to anything other than 0, overrides the calculated murder level.</td>
    </tr>
    <tr>
        <td>27</td>
        <td>spared_specific</td>
        <td>bool</td>
        <td>
            If you spare specific opponents, certain events that occur with a high murder level won't happen. Similar to
            a "redemption" flag. If you spare any of those monsters, the game is less desolated.
        </td>
    </tr>
    <tr>
        <td>28</td>
        <td>fast_text_skip</td>
        <td>debug bool</td>
        <td>Keeping C pressed during dialogue will quickly skip sentences.</td>
    </tr>
    <tr>
        <td>29</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>30</td>
        <td>tutorial_froggit_encountered</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>31</td>
        <td>pushed_rock_1</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>32</td>
        <td>pushed_rock_2</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>33</td>
        <td>pushed_rock_3</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>34</td>
        <td>candy_taken</td>
        <td>range</td>
        <td></td>
    </tr>
    <tr>
        <td>35</td>
        <td>pushed_rock_4</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>36</td>
        <td>spared_napstablook</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>37</td>
        <td>waited_toriel</td>
        <td>bool</td>
        <td>Wait for Toriel to call you when she asks to stay in a room.</td>
    </tr>
    <tr>
        <td>38..39</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>40</td>
        <td>greeted_toriel</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>41</td>
        <td>flirted_toriel</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>42</td>
        <td>call_mom_toriel</td>
        <td>bool</td>
        <td>In combination with flirted_toriel above, affects a few dialogues.</td>
    </tr>
    <tr>
        <td>43</td>
        <td>ruins_switches_pressed</td>
        <td>counter</td>
        <td>When greater than 25, changes the displayed text upon pressing a switch.</td>
    </tr>
    <tr>
        <td>44</td>
        <td>disobeyed_toriel</td>
        <td>counter</td>
        <td>Try to exit the ruins without asking Toriel about it first.</td>
    </tr>
    <tr>
        <td>45</td>
        <td>status_toriel</td>
        <td>range</td>
        <td>
            0 when you enter Toriel's house for the first time, 1 when you try to leave the ruins, 3 when you fight
            Toriel, 4 if you kill her, 5 if you spare her.
        </td>
    </tr>
    <tr>
        <td>46</td>
        <td>choice_flavor</td>
        <td>range</td>
        <td></td>
    </tr>
    <tr>
        <td>47</td>
        <td>status_creepy_tundra</td>
        <td>range</td>
        <td>Plays the creepy soundscape and shows Sans' shadow in the foreground.</td>
    </tr>
    <tr>
        <td>48..49</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>50</td>
        <td>know_water_sausage</td>
        <td>bool</td>
        <td>Read about water sausages in Toriel's room. Makes you recognize the plant in Toriel's living room.</td>
    </tr>
    <tr>
        <td>51</td>
        <td>wrong_switches_pressed</td>
        <td>counter</td>
        <td>After a while, gives you a hint about which switch to press.</td>
    </tr>
    <tr>
        <td>52</td>
        <td>status_doggo</td>
        <td>range</td>
        <td>1 if you kill Doggo, 2 if you throw him a stick and spare him.</td>
    </tr>
    <tr>
        <td>53</td>
        <td>status_dogcouple</td>
        <td>range</td>
        <td>1 if you kill Dogamy and/or Dogaressa, 2 if you damage them first and then throw a stick.</td>
    </tr>
    <tr>
        <td>54</td>
        <td>status_greaterdog</td>
        <td>range</td>
        <td>1 if you kill Greater Dog, 2 if you throw him a stick and spare him, 3 if you ignore him repeatedly.</td>
    </tr>
    <tr>
        <td>55</td>
        <td>status_lesserdog</td>
        <td>range</td>
        <td>
            1 if you kill Lesser Dog, 2 if you pet him until his neck extends at max. If 2, room_ruins6 will be filled
            with broken dog structures.
        </td>
    </tr>
    <tr>
        <td>56</td>
        <td>status_snowman</td>
        <td>range</td>
        <td>
            1 if you get a Snowman Piece from the snowman in room_tundra6A, 2 if you get another piece after disposing
            of the first one, 4 if you use the Snowman Piece in front of the him, 5 if you talk to the him when the flag
            is 4.
        </td>
    </tr>
    <tr>
        <td>57</td>
        <td>status_snowdrake</td>
        <td>range</td>
        <td>
            1 if you laugh at Snowdrake's joke; 2 if you kill him, all future instances of Snowdrake with Chilldrakes.
        </td>
    </tr>
    <tr>
        <td>58</td>
        <td>choice_harder_puzzle</td>
        <td>range</td>
        <td></td>
    </tr>
    <tr>
        <td>59</td>
        <td>spider_donations_total</td>
        <td>range</td>
        <td></td>
    </tr>
    <tr>
        <td>60</td>
        <td>nicecream_donations_total</td>
        <td>range</td>
        <td></td>
    </tr>
    <tr>
        <td>61</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>62</td>
        <td>choice_ate_left_spaghetti</td>
        <td>range</td>
        <td></td>
    </tr>
    <tr>
        <td>63</td>
        <td>xoxo_resets</td>
        <td>counter</td>
        <td>
            Affects the dialogue with Sans after the puzzle. Slightly different result if equals to 0 and M1 under the
            Sans category in undertale.ini is greater than 1.
        </td>
    </tr>
    <tr>
        <td>64</td>
        <td>toggled_snow_switch</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>65</td>
        <td>got_snowpoff_gold</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>66</td>
        <td>flirted_papyrus_fight</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>67</td>
        <td>status_papyrus</td>
        <td>range</td>
        <td>
            -1..-3: be defeated by Papyrus, affects the notes he leaves you in the garage. 0 if you spare Papyrus, 1 if
            you kill him.
        </td>
    </tr>
    <tr>
        <td>68</td>
        <td>fought_papyrus</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>69</td>
        <td>bpants_alt_dialogue</td>
        <td>debug bool</td>
        <td>Very slightly changes the dialogue with Burgerpants.</td>
    </tr>
    <tr>
        <td>70</td>
        <td>progress_tundra_battles</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>71</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>72</td>
        <td>status_inn</td>
        <td>range</td>
        <td>1 if you stay a night, 2 if you stay a night with less than 80 gold and the flag set to 0.</td>
    </tr>
    <tr>
        <td>73</td>
        <td>stayed_inn</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>74</td>
        <td>betrayed_gyftrot</td>
        <td></td>
        <td>Set if you "betray" Gyftrot by putting a present after removing some gifts off him. Unaccessed</td>
    </tr>
    <tr>
        <td>75</td>
        <td>armor_papyrus_inquiry</td>
        <td>range</td>
        <td>
            Equals to the id of the armor you're wearing upon the first call. The combination of these affects the
            dialogue you get in Papyrus' second phone call.
        </td>
    </tr>
    <tr>
        <td>76</td>
        <td>choice_papyrus_inquiry</td>
        <td>range</td>
        <td>0 if you tell Papyrus you are wearing the armor he specified, 1 otherwise.</td>
    </tr>
    <tr>
        <td>77</td>
        <td>armor_undyne_saw</td>
        <td>range</td>
        <td>Equals to the id of the armor Undyne saw you wear.</td>
    </tr>
    <tr>
        <td>78</td>
        <td>strong_tough_glove</td>
        <td>volatile bool</td>
        <td>Use a punchcard in battle while wearing the Tough Glove, increases attack.</td>
    </tr>
    <tr>
        <td>79</td>
        <td>nicecream_business</td>
        <td>bool</td>
        <td>
            8 if you buy a nicecream in room_tundra8. Upon the second encounter, will affect Nicecream Guy's mood and
            determine whether he'll start dispensing punchcards.
        </td>
    </tr>
    <tr>
        <td>80</td>
        <td>punchcards_bought</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>81</td>
        <td>status_shyren</td>
        <td>range</td>
        <td>
            1 if you kill Shyren; 2 if you encourage Shyren to the max, affects the Amalgamate's dialogue in the room
            after the True Pacifist ending.
        </td>
    </tr>
    <tr>
        <td>82</td>
        <td>papyrus_sink_event_occurred</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>83</td>
        <td>got_couch_gold</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>84</td>
        <td>unaccessed</td>
        <td></td>
        <td>Would affect the dialogue in room_water_mushroom, but it can't be accessed normally.</td>
    </tr>
    <tr>
        <td>85</td>
        <td>have_umbrella</td>
        <td>volatile bool</td>
        <td></td>
    </tr>
    <tr>
        <td>86</td>
        <td>music_statue_on</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>87</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>88</td>
        <td>dated_papyrus</td>
        <td>counter</td>
        <td>4 is the max, set when you complete the date.</td>
    </tr>
    <tr>
        <td>89</td>
        <td>dated_sans1</td>
        <td>counter</td>
        <td>2 is the max, set when you complete the first date with Sans at Grillbys.</td>
    </tr>
    <tr>
        <td>90</td>
        <td>choice_mkid_umbrella</td>
        <td>range</td>
        <td>
            1 if you meet Monster Kid without an umbrella; 2 if, with flag set to 1, you get an umbrella and talk to
            them; 3 if, with flag set to 2, you dispose of the umbrella and talk to them again.
        </td>
    </tr>
    <tr>
        <td>91</td>
        <td>interacted_garbage_savepoint</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>92</td>
        <td>status_stable</td>
        <td>range</td>
        <td>Would affect the status of the stable. It's cut-out content.</td>
    </tr>
    <tr>
        <td>93</td>
        <td>dated_napstablook</td>
        <td>range</td>
        <td>
            1 if you talk to Napstablook in their house, 3 if you feel like garbage with them, 9 if you refuse to feel like
            garbage.
        </td>
    </tr>
    <tr>
        <td>94</td>
        <td>current_napstablook_song</td>
        <td>volatile range</td>
        <td></td>
    </tr>
    <tr>
        <td>95</td>
        <td>aaron_woshua_event</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>96</td>
        <td>conversation_emblem</td>
        <td>counter</td>
        <td>Gerson's conversation.</td>
    </tr>
    <tr>
        <td>97</td>
        <td>creepy_friend_seen</td>
        <td>bool</td>
        <td>Would prevent the NPC in room_water_prebird from repeating himself. Cut-out content.</td>
    </tr>
    <tr>
        <td>98</td>
        <td>saved_mkid</td>
        <td>range</td>
        <td>
            0 if, when Monster Kid slips and is about fall, you exit the room; 1 if you let Undyne save them; 2 if you
            save them.
        </td>
    </tr>
    <tr>
        <td>99</td>
        <td>undyne_difficulty</td>
        <td>volatile counter</td>
        <td>
            Makes the fight more or less difficult, depending on a few factors (saved Monster Kid, how many times you
            died, etc.).
        </td>
    </tr>
    <tr>
        <td>100</td>
        <td>got_ribbon</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>101</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>102</td>
        <td>got_toyknife</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>103</td>
        <td>got_bscotch_pie</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>104</td>
        <td>got_quiche</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>105</td>
        <td>got_tutu</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>106</td>
        <td>got_ballet_shoes</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>107</td>
        <td>got_artifact</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>108</td>
        <td>got_spacefood</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>109</td>
        <td>got_instant_noodles</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>110</td>
        <td>got_frying_pan</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>111</td>
        <td>got_apron</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>112</td>
        <td>got_glamburger_trashcan</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>113</td>
        <td>got_gold_trashcan</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>114</td>
        <td>got_dagger</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>115</td>
        <td>got_locket</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>116..129</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>130</td>
        <td>spared_froggit</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>131</td>
        <td>spared_whimsun</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>132</td>
        <td>spared_moldsmal</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>133</td>
        <td>spared_loox</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>134</td>
        <td>spared_vegetoid</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>135</td>
        <td>spared_migosp</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>136</td>
        <td>spared_snowdrake</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>137</td>
        <td>spared_icecap</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>138</td>
        <td>spared_gyftrot</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>139</td>
        <td>spared_doggo</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>140</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>141</td>
        <td>spared_lesserdog</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>142</td>
        <td>spared_greatdog</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>143</td>
        <td>spared_aaron</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>144</td>
        <td>spared_moldsmalx</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>145</td>
        <td>spared_woshua</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>146</td>
        <td>spared_temmie</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>147</td>
        <td>spared_maddummy</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>148</td>
        <td>spared_vulkin</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>149</td>
        <td>spared_tsunderplane</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>150</td>
        <td>spared_pyrope</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>151</td>
        <td>spared_finalfroggit</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>152</td>
        <td>spared_whimsalot</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>153</td>
        <td>spared_astigmatism</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>154</td>
        <td>spared_madjick</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>155</td>
        <td>spared_finalknight</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>156</td>
        <td>spared_endogeny</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>157..190</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>191</td>
        <td>conversation_toriel_pacifist</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>192</td>
        <td>conversation_sans_pacifist</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>193</td>
        <td>conversation_undyne_pacifist</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>194</td>
        <td>unlock_napsta_pacifist</td>
        <td>bool</td>
        <td>Talk to Undyne until it invites you to go talk to Napstablook. They will be in their courtyard.</td>
    </tr>
    <tr>
        <td>195</td>
        <td>conversation_papyrus_pacifist</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>196</td>
        <td>conversation_alphys_pacifist</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>197</td>
        <td>conversation_asgore_pacifist</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>198</td>
        <td>conversation_mettaton_pacifist</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>199</td>
        <td>conversation_napstablook_pacifist</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>200</td>
        <td>kills_area_pointer</td>
        <td>range</td>
        <td>Assigned when moving between areas. Points at the area-specific kill counter.</td>
    </tr>
    <tr>
        <td>201</td>
        <td>kills</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>202</td>
        <td>kills_ruins</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>203</td>
        <td>kills_tundra</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>204</td>
        <td>kills_water</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>205</td>
        <td>kills_hotland</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>206..220</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>221</td>
        <td>genocide_ruins</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>222</td>
        <td>genocide_tundra</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>223</td>
        <td>genocide_water</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>224</td>
        <td>genocide_hotland</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>225</td>
        <td>genocide_core</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>226..249</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>250</td>
        <td>nicecream_business2</td>
        <td>volatile range</td>
        <td>Nicecream Guy's outlook of his business will depend on your interactions with him.</td>
    </tr>
    <tr>
        <td>251</td>
        <td>killed_undyne_ex</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>252</td>
        <td>killed_glad_dummy</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>253</td>
        <td>killed_snowman</td>
        <td>counter</td>
        <td>Take pieces of the snowman to kill him.</td>
    </tr>
    <tr>
        <td>254</td>
        <td>interacted_crosswords</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>255</td>
        <td>robbed_snowdin</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>256</td>
        <td>robbed_core</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>257..259</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>260</td>
        <td>used_recovery_item</td>
        <td>bool</td>
        <td>Affects the neutral ending.</td>
    </tr>
    <tr>
        <td>261</td>
        <td>interacted_fakedog</td>
        <td>bool</td>
        <td>Interact with the fake dog in the dev room.</td>
    </tr>
    <tr>
        <td>262</td>
        <td>delivered_seatea</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>263</td>
        <td>delivered_cinnabun</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>264</td>
        <td>delivered_hotdog</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>265</td>
        <td>tem_sell_parameter1</td>
        <td>range</td>
        <td></td>
    </tr>
    <tr>
        <td>266</td>
        <td>tem_sell_parameter2</td>
        <td>range</td>
        <td></td>
    </tr>
    <tr>
        <td>267</td>
        <td>status_hotel</td>
        <td>range</td>
        <td>1 the first time you stay at the hotel, 2 if you stay at the hotel again.</td>
    </tr>
    <tr>
        <td>268</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>269</td>
        <td>allergy_tem_talked</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>270</td>
        <td>glowshrooms_on</td>
        <td>bool</td>
        <td>Doesn't seem to have any effect, set when you turn 4 glowshrooms on in the mushrooms path puzzle.</td>
    </tr>
    <tr>
        <td>271</td>
        <td>fighting_sans</td>
        <td>volatile bool</td>
        <td></td>
    </tr>
    <tr>
        <td>272</td>
        <td>geeettttttt_dunked_on</td>
        <td>volatile bool</td>
        <td></td>
    </tr>
    <tr>
        <td>273..274</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>275</td>
        <td>tundra_stick_broken</td>
        <td>range</td>
        <td>1 when you walk past the stick, 2 when you walk further ahead.</td>
    </tr>
    <tr>
        <td>276</td>
        <td>temmie_college_paid</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>277</td>
        <td>fun_call_occurred</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>278</td>
        <td>completed_tile_puzzle</td>
        <td>bool</td>
        <td>Affects a dialogue with Papyrus on the phone.</td>
    </tr>
    <tr>
        <td>279</td>
        <td>interacted_clamgirl</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>280</td>
        <td>conversation_elderpuzzles</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>281</td>
        <td>status_sosorry</td>
        <td>range</td>
        <td>1 if you kill So Sorry, 2 if you spare him.</td>
    </tr>
    <tr>
        <td>282</td>
        <td>encountered_glyde</td>
        <td>bool</td>
        <td>Encounter Glyde.</td>
    </tr>
    <tr>
        <td>283</td>
        <td>check_papyrus_kitchen_again</td>
        <td>bool</td>
        <td>
            After the date, go in Papyrus' kitchen. Prevents Glyde from appearing and affects the dialogue with Papyrus
            on the phone.
        </td>
    </tr>
    <tr>
        <td>284</td>
        <td>undyne_spears_anger</td>
        <td>bool</td>
        <td>When Undyne throws her 100th spear, be in room_water8.</td>
    </tr>
    <tr>
        <td>285</td>
        <td>unaccessed</td>
        <td>volatile range</td>
        <td>Something to do with the spear tile generation, but is unaccessed.</td>
    </tr>
    <tr>
        <td>286</td>
        <td>conversation_toriel_sms</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>287</td>
        <td>conversation_sms_parameters</td>
        <td>volatile range</td>
        <td>Unclear specifics, but has to do with the amount of SMS you'll receive.</td>
    </tr>
    <tr>
        <td>288</td>
        <td>failed_defusing</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>289</td>
        <td>stepped_green_tile</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>290..299</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>300..311</td>
        <td>dimensional_box_A</td>
        <td>range</td>
        <td>Equals to the id of the stored item. Used in storage scripts.</td>
    </tr>
    <tr>
        <td>312..323</td>
        <td>dimensional_box_B</td>
        <td>range</td>
        <td></td>
    </tr>
    <tr>
        <td>324..349</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>350</td>
        <td>status_undyne</td>
        <td>range</td>
        <td>1 if you kill Undyne, 2 if you spare her, but don't give water to Undyne in Hotland.</td>
    </tr>
    <tr>
        <td>351</td>
        <td>undyne_hp_left</td>
        <td>range</td>
        <td>Equals to the HP Undyne died with. Unaccessed.</td>
    </tr>
    <tr>
        <td>352</td>
        <td>fought_undyne</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>353</td>
        <td>poured_water_ground</td>
        <td>counter</td>
        <td>Affects the dialogue with Clamguy, creates a puddle after a while.</td>
    </tr>
    <tr>
        <td>354</td>
        <td>conversation_papyrus_calls</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>355</td>
        <td>choice_maddummy</td>
        <td>range</td>
        <td>0 if you don't interact with the Mad Dummy; 1 if you punch it; 2 if you don't.</td>
    </tr>
    <tr>
        <td>356</td>
        <td>completed_piano_puzzle</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>357</td>
        <td>progress_water_battles</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>358</td>
        <td>progress_water2_battles</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>359</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>360..364</td>
        <td>rain_parameters</td>
        <td>volatile range</td>
        <td>Seems to affect the rain's rendering.</td>
    </tr>
    <tr>
        <td>365</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>366</td>
        <td>have_water</td>
        <td>volatile bool</td>
        <td></td>
    </tr>
    <tr>
        <td>367</td>
        <td>disable_alphys_calls</td>
        <td>bool</td>
        <td>Reach the lab in a genocide run.</td>
    </tr>
    <tr>
        <td>368</td>
        <td>disable_alphys_statuses</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>369</td>
        <td>conversation_alphys_statuses</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>370</td>
        <td>quick_battle</td>
        <td>bool</td>
        <td>Enter a quick battle (i.e. lasers, spears).</td>
    </tr>
    <tr>
        <td>371</td>
        <td>laser1_off</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>372</td>
        <td>laser2_on</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>373</td>
        <td>laser2_off</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>374</td>
        <td>completed_shoot_puzzle1</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>375</td>
        <td>completed_shoot_puzzle2</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>376</td>
        <td>conveyor_puzzle_variable</td>
        <td>volatile range</td>
        <td>Unclear, seems to be used as a position variable. Doesn't seem important.</td>
    </tr>
    <tr>
        <td>377</td>
        <td>failed_jetpack_segment</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>378</td>
        <td>hot_dogs_money_spent</td>
        <td>range</td>
        <td></td>
    </tr>
    <tr>
        <td>379</td>
        <td>conversation_hotdogs</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>380</td>
        <td>headdogs</td>
        <td>counter</td>
        <td>Buy a hot dog with no space in your inventory.</td>
    </tr>
    <tr>
        <td>381</td>
        <td>reached_headdogs_limit</td>
        <td>bool</td>
        <td>Buy a hot dog with 30 hot dogs on your head.</td>
    </tr>
    <tr>
        <td>382</td>
        <td>muffet_bribe_price</td>
        <td>range</td>
        <td>Various values, depending on your performance, gold, etc.</td>
    </tr>
    <tr>
        <td>383</td>
        <td>muffet_bribe_money_spent</td>
        <td>range</td>
        <td>Total bribes.</td>
    </tr>
    <tr>
        <td>384</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>385</td>
        <td>status_yellow_button</td>
        <td>range</td>
        <td>1 if yellow button available, 2 if yellow button pressed.</td>
    </tr>
    <tr>
        <td>386</td>
        <td>reset_bridgeseed_puzzle</td>
        <td>range</td>
        <td>Unclear specifics, but seems unimportant.</td>
    </tr>
    <tr>
        <td>387</td>
        <td>won_ball_game</td>
        <td>bool</td>
        <td>Win the ball game in an extremely short time.</td>
    </tr>
    <tr>
        <td>388</td>
        <td>fall_animation_parameters</td>
        <td>range</td>
        <td>Something to do with the fall animation. Not worth looking into.</td>
    </tr>
    <tr>
        <td>389</td>
        <td>dated_undyne</td>
        <td>range</td>
        <td>4 after you head outside of the flaming house.</td>
    </tr>
    <tr>
        <td>390</td>
        <td>undyne_expression</td>
        <td>volatile range</td>
        <td>Unclear, but it seems to determine the sprite for Undyne's expression.</td>
    </tr>
    <tr>
        <td>391</td>
        <td>choice_meal_grillby</td>
        <td>range</td>
        <td></td>
    </tr>
    <tr>
        <td>392</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>393</td>
        <td>unclear</td>
        <td>volatile range</td>
        <td>Internal to Madjick's battle.</td>
    </tr>
    <tr>
        <td>394</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>395</td>
        <td>bombs_defused</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>396</td>
        <td>fought_muffet</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>397</td>
        <td>killed_muffet</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>398</td>
        <td>current_elevator_floor</td>
        <td>range</td>
        <td></td>
    </tr>
    <tr>
        <td>399</td>
        <td>completed_shoot_puzzle3</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>400</td>
        <td>completed_shoot_puzzle4</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>401</td>
        <td>asked_papyrus_rg</td>
        <td>bool</td>
        <td>
            Call Papyrus when the Royal Guards are in the room. Slightly affects the dialogue with the guards when you
            spare them.
        </td>
    </tr>
    <tr>
        <td>402</td>
        <td>killed_rg</td>
        <td>bool</td>
        <td>Affects the dialogue during Papyrus' and Undyne's phone call.</td>
    </tr>
    <tr>
        <td>403</td>
        <td>spider_sale_big_spendings</td>
        <td>bool</td>
        <td>Buy a 9999 gold spider bakery sale item. Unaccessed.</td>
    </tr>
    <tr>
        <td>404</td>
        <td>laser3_off</td>
        <td>bool</td>
        <td>Disable the third laser despite of Alphys' phone call.</td>
    </tr>
    <tr>
        <td>405</td>
        <td>conversation_wares</td>
        <td>counter</td>
        <td>Bratty and Catty's conversations.</td>
    </tr>
    <tr>
        <td>406</td>
        <td>conversation_mettaton</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>407</td>
        <td>conversation_alphys</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>408</td>
        <td>progress_hotland_battles</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>409</td>
        <td>got_napstablook_friend_req</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>410..412</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>413</td>
        <td>dated_sans2</td>
        <td>range</td>
        <td>2 after you eat at the restaurant with Sans.</td>
    </tr>
    <tr>
        <td>414</td>
        <td>got_alphys_advice1</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>415</td>
        <td>got_alphys_advice2</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>416</td>
        <td>got_alphys_advice3</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>417</td>
        <td>got_alphys_advice4</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>418..421</td>
        <td>unclear</td>
        <td>volatile range</td>
        <td>
            Pre-castle specific flags, seem to affect whether you can proceed or not and are naturally set as you
            progress.
        </td>
    </tr>
    <tr>
        <td>422</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>423</td>
        <td>progress_core_battles</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>424</td>
        <td>turn_mettaton</td>
        <td>range</td>
        <td>1 if you can turn Mettaton, 2 when you turn Mettaton.</td>
    </tr>
    <tr>
        <td>425</td>
        <td>killed_mettaton</td>
        <td>bool</td>
        <td>1: kill Mettaton.</td>
    </tr>
    <tr>
        <td>426</td>
        <td>progress_core_battles2</td>
        <td>counter</td>
        <td>Incremental values: as you battle unique monsters in the core.</td>
    </tr>
    <tr>
        <td>427..429</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>430</td>
        <td>alphys_expression</td>
        <td>volatile range</td>
        <td>Unclear, but it seems to determine the sprite for Alphy's expression.</td>
    </tr>
    <tr>
        <td>431</td>
        <td>current_final_floor</td>
        <td>bool</td>
        <td>Determines which direction the elevator will go.</td>
    </tr>
    <tr>
        <td>432</td>
        <td>rode_long_elevator</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>433</td>
        <td>unlocked_mettaton_house</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>434</td>
        <td>choice_flamey_challenge</td>
        <td>range</td>
        <td>1 if you remember his name, else 2.</td>
    </tr>
    <tr>
        <td>435</td>
        <td>status_bpants</td>
        <td>range</td>
        <td>1 if you buy something from Burgerpants, 2 if you talk to him afterwards.</td>
    </tr>
    <tr>
        <td>436</td>
        <td>conversation_mtt</td>
        <td>counter</td>
        <td>Burgerpants' MTT conversation.</td>
    </tr>
    <tr>
        <td>437</td>
        <td>conversation_girls</td>
        <td>counter</td>
        <td>Burgerpants' conversation about Bratty and Catty.</td>
    </tr>
    <tr>
        <td>438..439</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>440</td>
        <td>water_taken_amount</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>441</td>
        <td>water_wasted_amount</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>442</td>
        <td>got_gun</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>443</td>
        <td>got_cowboy_hat</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>444</td>
        <td>got_mystery_key</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>445</td>
        <td>got_face_steak</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>446..449</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>450</td>
        <td>progress_early_story</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>451</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>452</td>
        <td>have_castle_key1</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>453</td>
        <td>have_castle_key2</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>454</td>
        <td>unlocked_latchkey</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>455</td>
        <td>early_story_parameter1</td>
        <td>range</td>
        <td>Seem to determine which step of the story to tell next.</td>
    </tr>
    <tr>
        <td>456</td>
        <td>early_story_parameter2</td>
        <td>range</td>
        <td></td>
    </tr>
    <tr>
        <td>457</td>
        <td>told_asgore_ready</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>458</td>
        <td>experience_cosmic_garbage</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>459</td>
        <td>riverman_destination</td>
        <td>volatile range</td>
        <td>1..3 being the destination when talking to the riverman.</td>
    </tr>
    <tr>
        <td>460</td>
        <td>got_tem_village_hint</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>461</td>
        <td>tem_boat_version</td>
        <td>volatile bool</td>
        <td>1: the riverman's boat will be cat-shaped.</td>
    </tr>
    <tr>
        <td>462</td>
        <td>called_already</td>
        <td>range</td>
        <td>
            Allows the second part of the call to occur when calling twice. Every room has two or more conversation
            parts.
        </td>
    </tr>
    <tr>
        <td>463..464</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>465</td>
        <td>papyrus_and_undyne</td>
        <td>bool</td>
        <td>After Undyne's date, calling Papyrus includes Undyne in the conversation.</td>
    </tr>
    <tr>
        <td>466..469</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>470</td>
        <td>conversation_undyne_mad</td>
        <td>bool</td>
        <td>
            Call Papyrus and Undyne in room_fire_lasers1. Just a counter used for this specific call, allowing the third
            part to occur.
        </td>
    </tr>
    <tr>
        <td>471..474</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>475</td>
        <td>killed_flowey</td>
        <td>bool</td>
        <td>Not sure about this one.</td>
    </tr>
    <tr>
        <td>476</td>
        <td>killed_asgore</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>477..479</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>480</td>
        <td>completed_truelab</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>481..492</td>
        <td>truelab_events</td>
        <td>range</td>
        <td>Various values. Only affects what happens in the lab, used to progress through.</td>
    </tr>
    <tr>
        <td>493</td>
        <td>dated_alphys</td>
        <td>range</td>
        <td>12 after you exit the true lab.</td>
    </tr>
    <tr>
        <td>494</td>
        <td>status_undyne_letter</td>
        <td>range</td>
        <td>3 if you receive Undyne's Letter EX.</td>
    </tr>
    <tr>
        <td>495</td>
        <td>popato_chisps_bought</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>496</td>
        <td>conversation_onionsan</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>497</td>
        <td>got_sans_room_key</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>498</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>499</td>
        <td>seen_cast</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>500</td>
        <td>fighting_asriel</td>
        <td>volatile bool</td>
        <td></td>
    </tr>
    <tr>
        <td>501</td>
        <td>conversation_asriel_fight</td>
        <td>counter</td>
        <td></td>
    </tr>
    <tr>
        <td>502</td>
        <td>but_it_refused</td>
        <td>volatile bool</td>
        <td>Flag 500 must be 1. Can't die.</td>
    </tr>
    <tr>
        <td>503</td>
        <td>dreamed_asriel_fight</td>
        <td>volatile bool</td>
        <td></td>
    </tr>
    <tr>
        <td>504</td>
        <td>unused</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>505..508</td>
        <td>saved_lost_soul</td>
        <td>bool</td>
        <td></td>
    </tr>
    <tr>
        <td>509</td>
        <td>toggle_final_beam</td>
        <td>volatile bool</td>
        <td>Sets the HP to decimal values.</td>
    </tr>
    <tr>
        <td>510</td>
        <td>plot_over</td>
        <td>range</td>
        <td>
            2 if you complete the True Pacifist boss fight, 1 if you talk to Asriel in the ruins after the True Pacifist
            boss fight.
        </td>
    </tr>
    <tr>
        <td>511</td>
        <td>conversation_asriel2</td>
        <td>counter</td>
        <td>Progress through the conversation with Asriel in the ruins.</td>
    </tr>
    <tr>
        <td>512</td>
        <td>choice_left_toriel</td>
        <td>bool</td>
        <td>Determines the type of the final scene in the bedroom.</td>
    </tr>
</tbody></table>
</details>

<details>
<summary>All Flags in DELTARUNE</summary>

The following data is sourced from [Tenna Save Editor](https://github.com/tennaproject/tenna-editor/blob/main/src/data/flags.ts)

Volatile values are flags that are changed often at runtime, so not easy to manually set. 

Bool values are true/false conditions. 

Number values can be any number. 

Map values map to certain specific values as outlined in their description.

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th>Flag</th>
      <th>Name</th>
      <th>Type</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>6</td>
      <td>Disable text skip - TEXT_SKIP_DISABLED</td>
      <td>volatile <br> bool</td>
      <td>Volatile. Prevents you from skipping text in some cutscenes. <br></td>
    </tr>
    <tr>
      <td>7</td>
      <td>Disable Dark World menu - DARK_WORLD_MENU_DISABLED</td>
      <td>bool</td>
      <td>Prevents you from opening the Dark World menu and affects music when leaving shops. <br></td>
    </tr>
    <tr>
      <td>8</td>
      <td>Simplify VFX - SIMPLIFIED_VFX_ENABLED</td>
      <td>bool</td>
      <td>Set from the Dark World menu. <br></td>
    </tr>
    <tr>
      <td>9</td>
      <td>Battle music - BATTLE_MUSIC_STATE</td>
      <td>map</td>
      <td>Volatile. Allows or prevents the game from playing Rude Buster at the start of an encounter. <br>0 = Default state<br>1 = In battle<br>2 = Starting boss music<br></td>
    </tr>
    <tr>
      <td>10</td>
      <td>Wrist Protector - WRIST_PROTECTOR_ENABLED</td>
      <td>bool</td>
      <td>Whether you have the Wrist Protector. Enabled by default since the Chapter 1&2 release. <br></td>
    </tr>
    <tr>
      <td>11</td>
      <td>Auto-run - AUTO_RUN_ENABLED</td>
      <td>bool</td>
      <td>Whether you have enabled auto-run. <br></td>
    </tr>
    <tr>
      <td>12</td>
      <td>Disable screen shake - SCREEN_SHAKE_DISABLED</td>
      <td>bool</td>
      <td>Keeps the game screen from shaking. Intended to be set from the Dark World menu. <br></td>
    </tr>
    <tr>
      <td>13</td>
      <td>Old attack controls - OLD_ATTACK_CONTROLS_ENABLED</td>
      <td>bool</td>
      <td>Use Z, X, and C, not just Z, to time attacks. <br></td>
    </tr>
    <tr>
      <td>14</td>
      <td>Remember battle selection - BATTLE_MENU_SELECTION_REMEMBERED</td>
      <td>bool</td>
      <td>Prevents the game from resetting your selection to "FIGHT" each turn. <br></td>
    </tr>
    <tr>
      <td>15</td>
      <td>Sound effect volume - SOUND_VOLUME</td>
      <td>number</td>
      <td>Volume of sound effects. <br></td>
    </tr>
    <tr>
      <td>16</td>
      <td>Music volume - MUSIC_VOLUME</td>
      <td>number</td>
      <td>Volume of music. <br></td>
    </tr>
    <tr>
      <td>17</td>
      <td>Master audio volume - AUDIO_VOLUME</td>
      <td>number</td>
      <td>Volume of all audio. <br></td>
    </tr>
    <tr>
      <td>20</td>
      <td>Other text command - OTHER_TEXT_COMMAND</td>
      <td>volatile <br> number</td>
      <td>Volatile. Controls how some characters' overworld sprites interact with their dialogue, among other things. <br></td>
    </tr>
    <tr>
      <td>21</td>
      <td>Door freeze timer - DOOR_FREEZE_TIMER</td>
      <td>volatile <br> number</td>
      <td>Volatile. Controls timing of room fades. <br></td>
    </tr>
    <tr>
      <td>22</td>
      <td>Disable X slowing - X_SLOWING_DISABLED</td>
      <td>bool</td>
      <td>Added in 1.08. Pressing Z while holding C in combat toggles it. Becomes debug-only in 1.09. <br></td>
    </tr>
    <tr>
      <td>23</td>
      <td>Climb unlocked - CAN_CLIMB</td>
      <td>bool</td>
      <td>Whether you can climb walls using the Claimb Claws. <br></td>
    </tr>
    <tr>
      <td>29</td>
      <td>Susie shows eyes - SUSIE_SHOW_EYES</td>
      <td>bool</td>
      <td>Makes Susie show her eyes at the end of Chapter 1. Ignored in Chapter 2; she shows her eyes anyway. <br></td>
    </tr>
    <tr>
      <td>30</td>
      <td>Ralsei hat state - RALSEI_HAT_STATE</td>
      <td>map</td>
      <td>Controls Ralsei's face selection. Ignored in Chapter 2; he's hatless anyway. <br>0 = Hat<br>1 = Hood<br>2 = Hatless<br></td>
    </tr>
    <tr>
      <td>31</td>
      <td>Disable loud steps - LOUD_STEPS_DISABLED</td>
      <td>bool</td>
      <td>Stops the echoing step sound found in the ?????? area, Great Door field, and Jevil's room. <br></td>
    </tr>
    <tr>
      <td>32</td>
      <td>Hide equip comments - EQUIP_COMMENTS_HIDDEN</td>
      <td>bool</td>
      <td>Prevents Susie and Ralsei from commenting on items you give them when in room_man. <br></td>
    </tr>
    <tr>
      <td>33</td>
      <td>Choice time taken - CHOICE_TIME_TAKEN</td>
      <td>volatile <br> number</td>
      <td>Volatile. The time, in frames, you take to make a choice. Used by Sans. <br></td>
    </tr>
    <tr>
      <td>34</td>
      <td>Party ACTs disabled - PARTY_ACTS_DISABLED</td>
      <td>bool</td>
      <td>Initialized to 1, reset to 0 when unlocking S-Action and R-Action. <br></td>
    </tr>
    <tr>
      <td>35</td>
      <td>Game over mode - GAME_OVER_MODE</td>
      <td>map</td>
      <td>Controls what the game does on game over. Usually 0. <br>0 = Normal Game Over<br>1 = Party Dojo<br>2 = Immediate respawn?<br></td>
    </tr>
    <tr>
      <td>36</td>
      <td>Dojo failure - DOJO_FAILURE</td>
      <td>bool</td>
      <td>Set when losing Party Dojo battles (i.e. when flag 35 is 1). Affects prize and dialogue. <br></td>
    </tr>
    <tr>
      <td>37</td>
      <td>Dojo battle active - DOJO_ACTIVE</td>
      <td>bool</td>
      <td>Alters battle win text and prevents you from gaining money outside of prizes. <br></td>
    </tr>
    <tr>
      <td>38</td>
      <td>Hide battle-end message - BATTLE_END_MESSAGE_DISABLED</td>
      <td>bool</td>
      <td>Disables the battle end message. Used for SnowGraving Berdly and Party Dojo. <br></td>
    </tr>
    <tr>
      <td>39</td>
      <td>Dojo aborted - DOJO_BATTLE_ABORTED</td>
      <td>bool</td>
      <td>Something to do with immediately ending Party Dojo battles, also used in the Jackenstein fight. <br></td>
    </tr>
    <tr>
      <td>40</td>
      <td>Violences - VIOLENCE_COUNT</td>
      <td>number</td>
      <td>Total number of enemies defeated through FIGHTing. Can be reduced by obtaining forgiveness from Rudinn or Hathy. <br></td>
    </tr>
    <tr>
      <td>41</td>
      <td>Spares - SPARE_COUNT</td>
      <td>number</td>
      <td>Total number of enemies SPAREd. Unaccessed. <br></td>
    </tr>
    <tr>
      <td>42</td>
      <td>Pacifies - PACIFY_COUNT</td>
      <td>number</td>
      <td>Total number of enemies Pacify/Sleep Mist-ed. Unaccessed. <br></td>
    </tr>
    <tr>
      <td>43</td>
      <td>Susie auto-violences - UNCONTROLLED_SUSIE_VIOLENCE_COUNT</td>
      <td>number</td>
      <td>Violences committed by Susie while not under player control. In SURVEY_PROGRAM and Chapter 1&2 it's never set due to a bug. It is possible to get the Chapter 1 Overthrow ending even if this is 1. <br></td>
    </tr>
    <tr>
      <td>44</td>
      <td>Kills - KILL_COUNT</td>
      <td>number</td>
      <td>Total number of enemies you killed. Includes SnowGrave and killing Pipis. <br></td>
    </tr>
    <tr>
      <td>45</td>
      <td>Freezes - FREEZE_COUNT</td>
      <td>number</td>
      <td>Total number of enemies you froze. <br></td>
    </tr>
    <tr>
      <td>49</td>
      <td>Last battle TP - LAST_ENCOUNTER_TP</td>
      <td>number</td>
      <td>Amount of TP gained in last encounter, used for Tenna's scoring system. <br></td>
    </tr>
    <tr>
      <td>50</td>
      <td>Last battle result - LAST_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Volatile. Contains what you did in the last encounter. For multiple enemies, priority is Violence > Spare > Pacify > IceShock. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>51</td>
      <td>Enemy 1 result - LAST_ENEMY_1_OUTCOME</td>
      <td>map</td>
      <td>Volatile. What you did to the top monster in the last encounter. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>52</td>
      <td>Enemy 2 result - LAST_ENEMY_2_OUTCOME</td>
      <td>map</td>
      <td>Volatile. What you did to the middle monster in the last encounter. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>53</td>
      <td>Enemy 3 result - LAST_ENEMY_3_OUTCOME</td>
      <td>map</td>
      <td>Volatile. What you did to the bottom monster in the last encounter. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>54</td>
      <td>Battle-result pointer - ENCOUNTER_RESULT_FLAG_ID</td>
      <td>volatile <br> number</td>
      <td>Volatile. Contains a numerical value representing the current encounter, which is used to permanently store the outcome of that encounter in a flag. <br></td>
    </tr>
    <tr>
      <td>55</td>
      <td>Frozen enemy X - FROZEN_ENEMY_X</td>
      <td>volatile <br> number</td>
      <td>Volatile. Used to return enemies to the correct spot in the overworld when frozen. <br></td>
    </tr>
    <tr>
      <td>56</td>
      <td>Frozen enemy Y - FROZEN_ENEMY_Y</td>
      <td>volatile <br> number</td>
      <td>Volatile. Used to return enemies to the correct spot in the overworld when frozen. <br></td>
    </tr>
    <tr>
      <td>60</td>
      <td>Dojo next encounter - DOJO_NEXT_ENCOUNTER</td>
      <td>map</td>
      <td>Volatile. Used to chain encounters for the Party Dojo All Stars challenge. <br>0 = Default state<br>90 = Werewires<br>91 = Smorgasbord<br>92 = Tasques + Maus<br>93 = Swatchlings<br>94 = Werewerewires<br></td>
    </tr>
    <tr>
      <td>61</td>
      <td>Recruiting disabled - RECRUITING_DISABLED</td>
      <td>bool</td>
      <td>Prevents you from recruiting enemies in Party Dojo battles. <br></td>
    </tr>
    <tr>
      <td>62</td>
      <td>Non-narrative intro - NON_NARRATIVE_BATTLE_INTRO</td>
      <td>bool</td>
      <td>Used when Noelle enters her first battle and when Susie wants to demonstrate UltimateHeal to not use the normal battle introduction typer. <br></td>
    </tr>
    <tr>
      <td>63</td>
      <td>Last enemy violenced - LAST_ENEMY_WAS_VIOLENCED</td>
      <td>volatile <br> bool</td>
      <td>Volatile. Triggers "You/Noelle became stronger" when violencing enemies. <br></td>
    </tr>
    <tr>
      <td>64</td>
      <td>Storage capacity - STORAGE_CAPACITY</td>
      <td>number</td>
      <td>The amount of items you can keep in your pockets. Always 24 in Chapters 2 and 3, 36 in Chapter 4, code exists to set it to 48 in Chapter 6 and later. <br></td>
    </tr>
    <tr>
      <td>65</td>
      <td>Level-ups - LEVEL_UP_COUNT_CH2</td>
      <td>number</td>
      <td>The number of times you have leveled up by violently defeating an encounter. Used for certain increases that only occur every 2, 4, or 10 encounters. <br></td>
    </tr>
    <tr>
      <td>66</td>
      <td>AT/Magic gains - AT_MAGIC_GAIN_COUNT_CH2</td>
      <td>number</td>
      <td>The number of times your AT and Magic have increased due to leveling up (every ten encounters). Used to prevent overly increasing them when sealing the fountain. <br></td>
    </tr>
    <tr>
      <td>100</td>
      <td>Got Glowshard - OBTAINED_GLOWSHARD</td>
      <td>bool</td>
      <td>Whether you obtained the Glowshard. Prevents it from re-appearing. <br></td>
    </tr>
    <tr>
      <td>101</td>
      <td>First candy tree - DARK_CANDY_TREE_1_TAKEN</td>
      <td>map</td>
      <td>How much Dark Candy you've taken from the first Dark Candy tree. <br>0 = None<br>1 = One candy<br>2 = Both candies<br></td>
    </tr>
    <tr>
      <td>102</td>
      <td>Second candy tree - DARK_CANDY_TREE_2_TAKEN</td>
      <td>map</td>
      <td>How much Dark Candy you've taken from the second Dark Candy tree. <br>0 = None<br>1 = One candy<br>2 = Both candies<br></td>
    </tr>
    <tr>
      <td>103</td>
      <td>Got Broken Cake - OBTAINED_BROKEN_CAKE_PIECE</td>
      <td>bool</td>
      <td>Whether you took a piece of the Broken Cake. <br></td>
    </tr>
    <tr>
      <td>104</td>
      <td>Got White Ribbon - OBTAINED_WHITE_RIBBON</td>
      <td>bool</td>
      <td>Whether you got the White Ribbon. <br></td>
    </tr>
    <tr>
      <td>105</td>
      <td>Got Iron Shackle - OBTAINED_IRON_SHACKLE</td>
      <td>bool</td>
      <td>Whether you took the Iron Shackle. <br></td>
    </tr>
    <tr>
      <td>106</td>
      <td>Ate Moss - ATE_MOSS_CH1</td>
      <td>bool</td>
      <td>Whether you ate the moss in Chapter 1. Allows you to obtain the Moss Finder title. <br></td>
    </tr>
    <tr>
      <td>107</td>
      <td>Got the dancer-room Revive Mint - OBTAINED_DANCER_REVIVE_MINT</td>
      <td>bool</td>
      <td>Whether you got the Revive Mint from the Scissor Dancers room. <br></td>
    </tr>
    <tr>
      <td>108</td>
      <td>Got Ragger - OBTAINED_RAGGER</td>
      <td>bool</td>
      <td>Whether you got the Ragger. Affects the Royal Coat Rack's dialogue about it. <br></td>
    </tr>
    <tr>
      <td>109</td>
      <td>Got Dice Brace - OBTAINED_DICE_BRACE</td>
      <td>bool</td>
      <td>Whether you got the Dice Brace. <br></td>
    </tr>
    <tr>
      <td>110</td>
      <td>Got the Bloxer-room money - OBTAINED_BLOXER_ROOM_MONEY</td>
      <td>bool</td>
      <td>Whether you got the 40D$ from that room with Bloxers. <br></td>
    </tr>
    <tr>
      <td>111</td>
      <td>Got Bloxer Mint - UNUSED_BLOXER_ROOM_REVIVE_MINT</td>
      <td>bool</td>
      <td>Whether you got a Revive Mint from that room with Bloxers. Unused because there isn't actually a Revive Mint chest in that room. <br></td>
    </tr>
    <tr>
      <td>112</td>
      <td>Got Jevil reward - OBTAINED_JEVIL_REWARD</td>
      <td>bool</td>
      <td>Whether you got the Jevilstail/Devilsknife from a chest. It appears outside the room if your inventory is full after the battle. <br></td>
    </tr>
    <tr>
      <td>113</td>
      <td>Got Clubswich - OBTAINED_CLUBS_SANDWICH</td>
      <td>bool</td>
      <td>Whether you got the Clubs Sandwich. <br></td>
    </tr>
    <tr>
      <td>114</td>
      <td>Got the Card Castle Revive Mint - OBTAINED_CASTLE_REVIVE_MINT</td>
      <td>bool</td>
      <td>Whether you got the Revive Mint from that chest that appears when you interact with the portraits. <br></td>
    </tr>
    <tr>
      <td>115</td>
      <td>Got Key A - OBTAINED_BROKEN_KEY_A</td>
      <td>bool</td>
      <td>Whether you got the Broken Key A. Also set if you defeat the Knight in Chapter 3 due to an encounterflag reuse. <br></td>
    </tr>
    <tr>
      <td>116</td>
      <td>Got Key B - OBTAINED_BROKEN_KEY_B</td>
      <td>bool</td>
      <td>Whether you got the Broken Key B. <br></td>
    </tr>
    <tr>
      <td>117</td>
      <td>Got Key C - OBTAINED_BROKEN_KEY_C</td>
      <td>bool</td>
      <td>Whether you got the Broken Key C. <br></td>
    </tr>
    <tr>
      <td>118</td>
      <td>Got the first Glow Wrist - OBTAINED_FIRST_GLOW_WRIST</td>
      <td>bool</td>
      <td>Whether you got the first Glow Wrist. <br></td>
    </tr>
    <tr>
      <td>119</td>
      <td>Got Nubert's Fiber Scarf - OBTAINED_NUBERT_TREASURE</td>
      <td>bool</td>
      <td>Whether you got the Fiber Scarf. <br></td>
    </tr>
    <tr>
      <td>120</td>
      <td>Got the second Glow Wrist - OBTAINED_SECOND_GLOW_WRIST</td>
      <td>bool</td>
      <td>Whether you got that other Glow Wrist. <br></td>
    </tr>
    <tr>
      <td>121</td>
      <td>Tenna - TENNA_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Tenna battle. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>122</td>
      <td>Got Tension Bit - OBTAINED_TENSION_BIT</td>
      <td>bool</td>
      <td>Whether you got the Tension Bit. <br></td>
    </tr>
    <tr>
      <td>123</td>
      <td>Got the third Revive Mint - OBTAINED_THIRD_REVIVE_MINT_CH2</td>
      <td>bool</td>
      <td>Whether you got the THIRD Revive Mint. <br></td>
    </tr>
    <tr>
      <td>125</td>
      <td>Revive Dust flag - UNUSED_REVIVE_DUST_FLAG</td>
      <td>number</td>
      <td>Unused. Intended for obtaining the Revive Dust, but overwritten by 137. <br></td>
    </tr>
    <tr>
      <td>126</td>
      <td>Got $20 from the trash can - OBTAINED_TRASH_CAN_20_DOLLARS</td>
      <td>bool</td>
      <td>Whether you got 20D$ from the twenty-dollar trash can. <br></td>
    </tr>
    <tr>
      <td>127</td>
      <td>Got $80 from the trash can - OBTAINED_TRASH_CAN_80_DOLLARS</td>
      <td>bool</td>
      <td>Whether you got 80D$ from the eighty-dollar trash can. <br></td>
    </tr>
    <tr>
      <td>128</td>
      <td>Got a CD Bagel from the trash can - OBTAINED_TRASH_CAN_CD_BAGEL</td>
      <td>bool</td>
      <td>Whether you got a CD Bagel from the CD Bagel trash can. <br></td>
    </tr>
    <tr>
      <td>129</td>
      <td>Got Ragger 2 - OBTAINED_RAGGER_2</td>
      <td>bool</td>
      <td>Whether you got the Ragger2. <br></td>
    </tr>
    <tr>
      <td>130</td>
      <td>Got Bounce Blade - OBTAINED_BOUNCE_BLADE</td>
      <td>bool</td>
      <td>Whether you got the Bounce Blade. <br></td>
    </tr>
    <tr>
      <td>131</td>
      <td>Got the second trash-can $20 - OBTAINED_SECOND_TRASH_CAN_20_DOLLARS</td>
      <td>bool</td>
      <td>Whether you got 20D$ from the other twenty-dollar trash can. <br></td>
    </tr>
    <tr>
      <td>132</td>
      <td>Got the second trash-can CD Bagel - OBTAINED_SECOND_TRASH_CAN_CD_BAGEL</td>
      <td>bool</td>
      <td>Whether you got a CD Bagel from the other CD Bagel trash can. <br></td>
    </tr>
    <tr>
      <td>133</td>
      <td>Got $1 from the chest - OBTAINED_ONE_DOLLAR_CHEST</td>
      <td>bool</td>
      <td>Whether you got the $1 from the one-dollar treasure chest. <br></td>
    </tr>
    <tr>
      <td>134</td>
      <td>Got Pink Ribbon - OBTAINED_PINK_RIBBON</td>
      <td>bool</td>
      <td>Whether you got the Pink Ribbon. <br></td>
    </tr>
    <tr>
      <td>135</td>
      <td>Got the CD Bagel chest - OBTAINED_CD_BAGEL_CHEST</td>
      <td>bool</td>
      <td>Whether you got a CD Bagel from the CD Bagel treasure chest. <br></td>
    </tr>
    <tr>
      <td>136</td>
      <td>Got the secret Dark Candy - OBTAINED_SECRET_DARK_CANDY</td>
      <td>bool</td>
      <td>Whether you got a Dark Candy from the secret Dark Candy location. <br></td>
    </tr>
    <tr>
      <td>137</td>
      <td>Got Revive Dust - OBTAINED_REVIVE_DUST</td>
      <td>bool</td>
      <td>Whether you got the Revive Dust. <br></td>
    </tr>
    <tr>
      <td>138</td>
      <td>Got the fourth Revive Mint - OBTAINED_FOURTH_REVIVE_MINT</td>
      <td>bool</td>
      <td>Whether you got the fourth Revive Mint from a painting. <br></td>
    </tr>
    <tr>
      <td>139</td>
      <td>Got the Mansion Glowshard - OBTAINED_MANSION_GLOWSHARD</td>
      <td>bool</td>
      <td>Whether you got the Glowshard in Queen's Mansion, found by activating all the platters behind the door on the 2F moving vases room. <br></td>
    </tr>
    <tr>
      <td>140</td>
      <td>Got Dark Candy from the trash can - OBTAINED_TRASH_CAN_DARK_CANDY</td>
      <td>bool</td>
      <td>Whether you got a Dark Candy from the Dark Candy trash can. <br></td>
    </tr>
    <tr>
      <td>141</td>
      <td>Got Chain Mail - OBTAINED_CHAIN_MAIL</td>
      <td>bool</td>
      <td>Whether you got the Chain Mail armor. <br></td>
    </tr>
    <tr>
      <td>142</td>
      <td>Got Spamton reward - OBTAINED_SPAMTON_REWARD</td>
      <td>bool</td>
      <td>Whether you got the Dealmaker/Puppet Scarf from a chest. There's one immediately after you beat Spamton, and one back at My Castle Town. <br></td>
    </tr>
    <tr>
      <td>176</td>
      <td>Susie - SOUND_OF_JUSTICE_SUSIE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Susie-only stage of the Sound of Justice Battle, always 2. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>177</td>
      <td>Spawn - TITAN_SPAWN_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Titan Spawn encounter. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>186</td>
      <td>Kris - SOUND_OF_JUSTICE_KRIS_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Kris stage of the Sound of Justice Battle, always 2. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>200</td>
      <td>Ran to Susie at school - RAN_IN_SCHOOL</td>
      <td>bool</td>
      <td>Whether you ran to Susie in the Chapter 1 school scene. Unaccessed. <br></td>
    </tr>
    <tr>
      <td>201</td>
      <td>Solved the eye puzzle - SOLVED_EYE_PUZZLE</td>
      <td>bool</td>
      <td>Whether you solved the eye puzzle in the ?????? area. <br></td>
    </tr>
    <tr>
      <td>202</td>
      <td>Susie approach - DARK_AREA_MOVEMENT_CHOICE</td>
      <td>map</td>
      <td>How you proceeded once finding Susie in the ?????? area. <br>0 = Walked<br>1 = Ran<br>2 = Wrong way<br></td>
    </tr>
    <tr>
      <td>203</td>
      <td>Skipped - SKIPPED_PROPHECY</td>
      <td>bool</td>
      <td>Whether you skipped Ralsei's prophecy. Lancer explains it instead. <br></td>
    </tr>
    <tr>
      <td>204</td>
      <td>Ralsei subject answer - RALSEI_SUBJECT_RESPONSE</td>
      <td>map</td>
      <td>How you answered Ralsei when he said he had no subjects... that is, unused. <br>0 = Default state<br>1 = I'll be your subject<br>2 = Keep dreaming<br></td>
    </tr>
    <tr>
      <td>205</td>
      <td>Outcome - RALSEI_TUTORIAL_OUTCOME</td>
      <td>map</td>
      <td>What happened during Ralsei's tutorial. <br>0 = Skipped tutorial<br>1 = Success<br>2 = Hug Ralsei (in unused version of tutorial)<br>3 = Beat up Ralsei<br>4 = Beat up dummy<br>5 = Continued defending<br>6 = Missed dummy<br></td>
    </tr>
    <tr>
      <td>206</td>
      <td>Learned to run - LEARNED_TO_RUN</td>
      <td>bool</td>
      <td>Set to 1 whether Ralsei explains it or you demonstrate. Just prevents him from asking again. <br></td>
    </tr>
    <tr>
      <td>207</td>
      <td>Manual disposal - MANUAL_DISPOSAL_PROGRESS</td>
      <td>map</td>
      <td>Your progress on being a terrible person. Ralsei gives you a trash can for the manual instead of a stand, in case you ever want to trash it again. <br>0 = Default state<br>1 = Dropped once<br>2 = Dropped twice<br></td>
    </tr>
    <tr>
      <td>208</td>
      <td>Re-convinced Rudinn - RE_CONVINCED_RUDINN</td>
      <td>bool</td>
      <td>Whether you Convinced Rudinn after failing to do. Unused, since it works first try now. <br></td>
    </tr>
    <tr>
      <td>209</td>
      <td>Saw the Field title card - SAW_FIELD_SONG</td>
      <td>bool</td>
      <td>Prevents you from seeing the Field of Hopes and Dreams title every single room. <br></td>
    </tr>
    <tr>
      <td>210</td>
      <td>Lancer dialogue - LANCER_PRE_HATHY_DIALOGUE</td>
      <td>map</td>
      <td>Alters Lancer's dialogue if interacted with prior to the triple Hathy fight. <br>0 = Default state<br>1 = Talked<br>2 = Did not talk<br></td>
    </tr>
    <tr>
      <td>211</td>
      <td>Outcome - C_ROUND_OUTCOME</td>
      <td>map</td>
      <td>What happened to C. Round. Can skip Ralsei telling Susie not to fight. <br>0 = Default state<br>1 = Complimented by Susie<br>2 = Warned<br>3 = Attacked by Kris/Ralsei<br></td>
    </tr>
    <tr>
      <td>212</td>
      <td>Progress - VANDALIZED_BOX_PUZZLE_STATE</td>
      <td>map</td>
      <td>Progress on the vandalized box puzzle. <br>0 = Default state<br>1 = Initiated puzzle<br>2 = Failure (unused)<br></td>
    </tr>
    <tr>
      <td>214</td>
      <td>Team name - TEAM_NAME</td>
      <td>map</td>
      <td>The name of your team. <br>0 = The Guys<br>1 = The $!$? Squad<br>2 = The Lancer Fan Club<br>3 = The Fun Gang<br></td>
    </tr>
    <tr>
      <td>215</td>
      <td>Talked to Jigsaw Joe - TALKED_TO_JIGSAW_JOE</td>
      <td>bool</td>
      <td>Whether you talked to Joe (and were inevitably offered a tutorial). Makes him help with the Warp Door. <br></td>
    </tr>
    <tr>
      <td>216</td>
      <td>Donated to the hole - DONATED_TO_HOLE</td>
      <td>bool</td>
      <td>Whether you put a dollar in the donation hole. <br></td>
    </tr>
    <tr>
      <td>217</td>
      <td>Solved Rouxls's first puzzle - SOLVED_FIRST_ROUXLS_PUZZLE</td>
      <td>bool</td>
      <td>Whether you solved Rouxls's first puzzle. <br></td>
    </tr>
    <tr>
      <td>218</td>
      <td>Solved Rouxls's second puzzle - SOLVED_SECOND_ROUXLS_PUZZLE</td>
      <td>bool</td>
      <td>Whether you solved Rouxls's second puzzle. <br></td>
    </tr>
    <tr>
      <td>220</td>
      <td>Head - THRASH_MACHINE_HEAD</td>
      <td>map</td>
      <td>Your Thrash Machine's head. <br>0 = Laser<br>1 = Sword<br>2 = Flame<br>3 = Duck<br>-1 = In design<br></td>
    </tr>
    <tr>
      <td>221</td>
      <td>Body - THRASH_MACHINE_BODY</td>
      <td>map</td>
      <td>Your Thrash Machine's chassis. <br>0 = Plain<br>1 = Wheel<br>2 = Tank<br>3 = Duck<br>-1 = In design<br></td>
    </tr>
    <tr>
      <td>222</td>
      <td>Shoe - THRASH_MACHINE_SHOE</td>
      <td>map</td>
      <td>Your Thrash Machine's... well, there's a lot of variance here. <br>0 = Shoes<br>1 = Wheels<br>2 = Treads<br>3 = Duck<br>-1 = In design<br></td>
    </tr>
    <tr>
      <td>223</td>
      <td>Head color - THRASH_MACHINE_HEAD_COLOR</td>
      <td>color</td>
      <td>Your Thrash Machine's head color. <br></td>
    </tr>
    <tr>
      <td>224</td>
      <td>Body color - THRASH_MACHINE_BODY_COLOR</td>
      <td>color</td>
      <td>Your Thrash Machine's chassis color. <br></td>
    </tr>
    <tr>
      <td>225</td>
      <td>Shoe color - THRASH_MACHINE_SHOE_COLOR</td>
      <td>color</td>
      <td>Your Thrash Machine's shoe color. <br></td>
    </tr>
    <tr>
      <td>226</td>
      <td>Designed the Thrash Machine - MADE_THRASH_MACHINE</td>
      <td>bool</td>
      <td>Whether you designed the Thrash Machine yet. <br></td>
    </tr>
    <tr>
      <td>229</td>
      <td>Lancer dialogue - LANCER_FOLLOW_DIALOGUE_PROGRESS</td>
      <td>map</td>
      <td>How far Lancer has followed you after joining the team. <br>0 = Default state<br>1 = Monogrammed track jackets<br>3 = Just chill with us<br>4 = Stop making fun of me<br>5 = Darkberry Teacakes (unused)<br>6 = A candy tree!<br>7 = My teeth are disintegrating!<br>8 = Does your dad seem happy?<br>9 = I also feel kinda...<br>10 = ...maybe.<br>11 = That's the FOUNTAIN!<br>12 = All we gotta do is crush them.<br>99 = Max value (unused)<br></td>
    </tr>
    <tr>
      <td>231</td>
      <td>Object interactions - JAIL_INTERACTION_COUNT</td>
      <td>number</td>
      <td>The number of times you have interacted with objects while in jail. The cutscene is triggered by talking to Ralsei after 3+ interactions. <br></td>
    </tr>
    <tr>
      <td>232</td>
      <td>Interacted with the salsa stump - INTERACTED_WITH_SALSA</td>
      <td>bool</td>
      <td>Whether you interacted with the salsa stump. NOT what you actually did; that isn't saved. <br></td>
    </tr>
    <tr>
      <td>233</td>
      <td>Asked the Royal Coat Rack about the chest - ASKED_ROYAL_COAT_RACK_ABOUT_CHEST</td>
      <td>bool</td>
      <td>Whether you talked to the Royal Coat Rack before taking the Ragger. Changes their dialogue if you take it without asking. <br></td>
    </tr>
    <tr>
      <td>234</td>
      <td>Solved the Clover suit puzzle - SOLVED_CLOVER_PUZZLE</td>
      <td>bool</td>
      <td>Whether you solved the suits puzzle before the Clover fight. <br></td>
    </tr>
    <tr>
      <td>235</td>
      <td>Clover puzzle barrier - UNUSED_CLOVER_PUZZLE_BARRIER_FLAG</td>
      <td>bool</td>
      <td>Unused barrier flag for the suits puzzle before the Clover fight. <br></td>
    </tr>
    <tr>
      <td>236</td>
      <td>Talked to all Clover faces - TALKED_TO_ALL_CLOVER_HEADS</td>
      <td>bool</td>
      <td>Set when talking to all of Clover before her fight. Alters her dialogue. <br></td>
    </tr>
    <tr>
      <td>237</td>
      <td>Solved - SOLVED_DARK_PUZZLE</td>
      <td>bool</td>
      <td>Whether you solved the puzzle in the darknening room. It does not save if you did it without going in the middle. <br></td>
    </tr>
    <tr>
      <td>238</td>
      <td>Susie's snack - SUSIE_BOUGHT_SNACK</td>
      <td>bool</td>
      <td>Whether Susie and Lancer bought their Hearts Donut yet. <br></td>
    </tr>
    <tr>
      <td>239</td>
      <td>Elevator floor - CARD_CASTLE_ELEVATOR_FLOOR</td>
      <td>map</td>
      <td>Volatile. Tracks the floor you're currently on when in elevators. <br>0 = Basement B1<br>1 = Floor 1F<br>2 = Floor 5F<br>3 = ???? (JEVIL)<br></td>
    </tr>
    <tr>
      <td>240</td>
      <td>Unlocked - CARD_CASTLE_ELEVATOR_UNLOCKED</td>
      <td>bool</td>
      <td>Whether you have unlocked the Card Castle elevator by going to floor 5F. <br></td>
    </tr>
    <tr>
      <td>241</td>
      <td>Progress - JEVIL_PROGRESS</td>
      <td>map</td>
      <td>Your progress with JEVIL. Alters Seam's dialogue. <br>0 = Default state<br>1 = Talked to JEVIL<br>5 = Opened door<br>6 = Fought<br>7 = Spared<br></td>
    </tr>
    <tr>
      <td>242</td>
      <td>Overflow chest - JEVIL_REWARD_CHEST_ITEM</td>
      <td>map</td>
      <td>The item in the chest outside JEVIL's room, if you don't have enough storage space for it. See also flag 112. <br>0 = Default state<br>1 = Devilsknife<br>2 = Jevilstail<br></td>
    </tr>
    <tr>
      <td>243</td>
      <td>Rudinn - RUDINN_DIALOGUE_OUTCOME</td>
      <td>map</td>
      <td>The status of your talking to Rudinn in Card Castle. Special dialogue if set to 3 but you then hurt Rudinns. <br>0 = Default state<br>1 = Apologized<br>2 = Did not apologize<br>3 = Did not need to apologize<br></td>
    </tr>
    <tr>
      <td>244</td>
      <td>Talked to Hathy - TALKED_TO_HATHY</td>
      <td>bool</td>
      <td>Whether you talked to Hathy in Card Castle. Only set if you had two or fewer Hathy kills. <br></td>
    </tr>
    <tr>
      <td>245</td>
      <td>Summoned the Bluh Chest - SUMMONED_BLUH_CHEST</td>
      <td>bool</td>
      <td>Whether you interacted with all four Bluh Paintings, summoning the Bluh Chest. <br></td>
    </tr>
    <tr>
      <td>246</td>
      <td>Checked K. Round - CHECKED_K_ROUND</td>
      <td>bool</td>
      <td>Whether you Checked K. Round the first time, changing its act to Checkers (including in the second fight). <br></td>
    </tr>
    <tr>
      <td>247</td>
      <td>Spared King - SPARED_KING</td>
      <td>bool</td>
      <td>Whether you exhausted King rather than fighting him. <br></td>
    </tr>
    <tr>
      <td>248</td>
      <td>Violent ending - VIOLENT_ENDING_CH1</td>
      <td>bool</td>
      <td>Whether you got the bad (beat people up) ending in Chapter 1. Minor dialogue differences in Castle Town. <br></td>
    </tr>
    <tr>
      <td>249</td>
      <td>Spared Lancer and Susie - SPARED_LANCER</td>
      <td>bool</td>
      <td>Whether you spared Lancer and Susie. <br></td>
    </tr>
    <tr>
      <td>250</td>
      <td>Rematches - THRASH_MACHINE_REMATCH_COUNT</td>
      <td>number</td>
      <td>The number of times you fought Lancer and Susie, thus requiring them to blow up a Thrash Machine. Unique dialogue at 1 and 2. <br></td>
    </tr>
    <tr>
      <td>251</td>
      <td>Warp Door restored - SHORTCUT_DOOR_HELP</td>
      <td>bool</td>
      <td>Whether Jigsaw Joe helped restore the Warp Door. No functional change. <br></td>
    </tr>
    <tr>
      <td>252</td>
      <td>Inspected the beds - INSPECTED_BEDS_CH1</td>
      <td>bool</td>
      <td>Whether you inspected all four beds in Chapter 1, becoming a Bed Inspector. <br></td>
    </tr>
    <tr>
      <td>253</td>
      <td>Traded the Top Cake - TRADED_TOP_CAKE</td>
      <td>bool</td>
      <td>Whether you returned the TopCake, receiving a SpinCake in its place. <br></td>
    </tr>
    <tr>
      <td>254</td>
      <td>Talked to original &ensp;*Starwalker* - TALKED_TO_STARWALKER_CH1</td>
      <td>bool</td>
      <td>Whether you talked to the original Starwalker. That's foresight. <br></td>
    </tr>
    <tr>
      <td>255</td>
      <td>Dialogue progress - RUDY_DIALOGUE_PROGRESS_CH1</td>
      <td>map</td>
      <td>Progress talking with Rudolph Holiday in Chapter 1. <br>0 = Default state<br>1 = Noelle left<br>2 = Talked to Rudy<br></td>
    </tr>
    <tr>
      <td>256</td>
      <td>Talked to Berdly at the hospital window - TALKED_TO_BERDLY_AT_HOSPITAL_WINDOW</td>
      <td>bool</td>
      <td>Whether you talked to Berdly about visiting the hospital window to have something thrown at him. Slightly alters his dialogue about How to Draw Dragons. <br></td>
    </tr>
    <tr>
      <td>257</td>
      <td>Put fingers in the picnic table - PUT_FINGERS_IN_PICNIC_TABLE</td>
      <td>bool</td>
      <td>Whether you tried to put your fingers in the picnic table. <br></td>
    </tr>
    <tr>
      <td>258</td>
      <td>Friendship - ONION_STATUS_CH1</td>
      <td>map</td>
      <td>Onion's status. <br>0 = Default state<br>1 = Talking (volatile)<br>2 = Befriended<br>3 = Rejected<br></td>
    </tr>
    <tr>
      <td>259</td>
      <td>Your name - ONION_PLAYER_NAME</td>
      <td>map</td>
      <td>The name you told Onion was yours. <br>0 = Default state<br>1 = Kris<br>2 = Hippopotamus<br></td>
    </tr>
    <tr>
      <td>260</td>
      <td>Onion's name - ONION_NAME</td>
      <td>map</td>
      <td>The name you told Onion was theirs. <br>0 = Default state<br>1 = Onion<br>2 = Beauty<br>3 = Asriel II<br>4 = Disgusting<br></td>
    </tr>
    <tr>
      <td>261</td>
      <td>Dialogue progress - QC_DIALOGUE_PROGRESS_CH1</td>
      <td>map</td>
      <td>Tracks your talking with QC. <br>0 = Default state<br>1 = Received Hot Chocolate<br>2 = Full inventory<br></td>
    </tr>
    <tr>
      <td>262</td>
      <td>Bouquet quest - BOUQUET_QUEST_PROGRESS_CH1</td>
      <td>map</td>
      <td>Progress toward failing to redeem Toriel and Asgore's relationship in Chapter 1. <br>0 = Default state<br>1 = In flower shop<br>2 = Received bouquet<br>3 = Gave to Toriel<br>4 = Disposed of<br></td>
    </tr>
    <tr>
      <td>263</td>
      <td>Fridge egg - ASGORE_FRIDGE_EGG_STATUS</td>
      <td>map</td>
      <td>The Chapter 1 egg status, with regards to Asgore's fridge. Each stage correlates with an egg quantity in the fridge. <br>0 = (0) Default state<br>1 = (1) Egg dropped/fridge inspected eggless<br>2 = (2) Egg put in fridge<br></td>
    </tr>
    <tr>
      <td>264</td>
      <td>Asgore stairs door side - ASGORE_STAIRS_ENTRY_X</td>
      <td>volatile <br> number</td>
      <td>Volatile. Persists the different door sides when going upstairs in Asgore's fridge via Kris's x-coordinate. <br></td>
    </tr>
    <tr>
      <td>265</td>
      <td>Talked to Catty - TALKED_TO_CATTY_CH1</td>
      <td>bool</td>
      <td>Whether you talked to Catty in Chapter 1. <br></td>
    </tr>
    <tr>
      <td>267</td>
      <td>Toriel talk - UNUSED_TORIEL_DIALOGUE_PROGRESS</td>
      <td>map</td>
      <td>Progress talking to Toriel in an unused variant. <br>0 = Headband<br>1 = Go to bed<br>-10 = Kris...?<br></td>
    </tr>
    <tr>
      <td>268</td>
      <td>Called home from house - CALLED_TORIEL_FROM_HOME</td>
      <td>bool</td>
      <td>Whether you called Toriel's home phone, while at home. Unaccessed. <br></td>
    </tr>
    <tr>
      <td>269</td>
      <td>Talked to Alphys - TALKED_TO_ALPHYS_CH1</td>
      <td>bool</td>
      <td>Whether you met Alphys after school in Chapter 1. Alters her dialogue the morning of Chapter 2. <br></td>
    </tr>
    <tr>
      <td>270</td>
      <td>Talked to Undyne - TALKED_TO_UNDYNE_CH1</td>
      <td>bool</td>
      <td>Whether you met Undyne in Chapter 1. <br></td>
    </tr>
    <tr>
      <td>271</td>
      <td>Burgerpants - BURGERPANTS_DIALOGUE_PROGRESS_CH1</td>
      <td>map</td>
      <td>Progress chatting with BurgerPizzaSodaCandyPants. <br>0 = Default state<br>1 = Mask off<br>2 = Talked<br></td>
    </tr>
    <tr>
      <td>272</td>
      <td>Toriel calls - TORIEL_CALL_COUNT</td>
      <td>number</td>
      <td>The number of times you called Toriel after school. If zero when leaving the school, she calls you instead, incrementing the flag. <br></td>
    </tr>
    <tr>
      <td>273</td>
      <td>Dialogue progress - SANS_DIALOGUE_PROGRESS_CH1</td>
      <td>map</td>
      <td>Progress chatting up the funny bone man in Chapter 1. <br>0 = Default state<br>1 = Talked<br>2 = Invited over<br></td>
    </tr>
    <tr>
      <td>274</td>
      <td>Phone number - SANS_PHONE_PROGRESS</td>
      <td>map</td>
      <td>Your progress toward being called an idiot baby. <br>0 = Default state<br>1 = Received number<br>2 = Called<br></td>
    </tr>
    <tr>
      <td>275</td>
      <td>Idiot baby - IDIOT_BABY_STATUS</td>
      <td>map</td>
      <td>What you are. <br>0 = None<br>1 = Idiot<br>2 = Baby<br>3 = Idiot Baby<br></td>
    </tr>
    <tr>
      <td>276</td>
      <td>Dialogue progress - NOELLE_DIALOGUE_PROGRESS_CH1</td>
      <td>map</td>
      <td>Your progress talking to Noelle outside her house in Chapter 1. If 2, she gives Susie the Light Candy in Chapter 2. <br>0 = Default state<br>1 = Talked<br>2 = Talked about Susie<br></td>
    </tr>
    <tr>
      <td>277</td>
      <td>Returns - HOME_RETURN_COUNT_CH1</td>
      <td>number</td>
      <td>The number of times you have returned home at the end of Chapter 1. Special dialogue at 0, 1, and 7; stops counting at 8. <br></td>
    </tr>
    <tr>
      <td>278</td>
      <td>Used Rudy's sink - USED_RUDY_SINK_CH1</td>
      <td>bool</td>
      <td>Whether you used the sink in Chapter 1 (of the 1&2 demo). Rudy comments on you "loving that sink". <br></td>
    </tr>
    <tr>
      <td>279</td>
      <td>Loaded legacy file - LOADED_LEGACY_FILE</td>
      <td>bool</td>
      <td>Set to 1 while loading a Chapter 1 file (which has different room offsets). If 1 on an old file, you might load into a Chapter 2 room. <br></td>
    </tr>
    <tr>
      <td>280</td>
      <td>Shadow Crystal usage - SHADOW_CRYSTAL_USE_CH1</td>
      <td>map</td>
      <td>Your Shadow Crystal usage in Chapter 1. Unique dialogue if less than 2. <br>0 = Default state<br>1 = Saw toys<br>2 = Not useful<br></td>
    </tr>
    <tr>
      <td>281</td>
      <td>Glass usage without Susie - GLASS_USE_ALONE_CH1</td>
      <td>map</td>
      <td>Your Glass usage without Susie around/in Chapter 1. <br>0 = Default state<br>1 = Saw through hand<br>2 = Not useful (Ch1)<br></td>
    </tr>
    <tr>
      <td>290</td>
      <td>Solved the Dice Brace puzzle - SOLVED_DICE_BRACE_PUZZLE</td>
      <td>bool</td>
      <td>Whether you solved the suits puzzle to obtain Dice Brace. <br></td>
    </tr>
    <tr>
      <td>291</td>
      <td>Forest maze progress - FOREST_MAZE_PROGRESS</td>
      <td>volatile <br> number</td>
      <td>Volatile. Counts the number of correct rooms you've gone through in the maze. Find Susie at 4, done at 9. <br></td>
    </tr>
    <tr>
      <td>292</td>
      <td>Forest maze wrong turns - FOREST_MAZE_FAILURE_COUNT</td>
      <td>volatile <br> number</td>
      <td>Volatile. Counts how much you've taken the wrong choice in the forest maze. Jumps straight to 3 (dead end) if you got lost before or found Susie. <br></td>
    </tr>
    <tr>
      <td>293</td>
      <td>Lancer dead ends - LANCER_DEAD_END_COUNT</td>
      <td>number</td>
      <td>The number of times you found the Lancer dead end. <br></td>
    </tr>
    <tr>
      <td>294</td>
      <td>Susie dead ends - SUSIE_DEAD_END_COUNT</td>
      <td>number</td>
      <td>The number of times you found the Susie dead end. <br></td>
    </tr>
    <tr>
      <td>295</td>
      <td>Talked to Topchef after returning the Top Cake - TALKED_TO_TOPCHEF_AFTER_RETURNING_TOP_CAKE</td>
      <td>bool</td>
      <td>Whether you talked to Topchef in the pacifist end after returning the Topcake. He thinks Susie is Clover's mom. <br></td>
    </tr>
    <tr>
      <td>296</td>
      <td>Visited jail - VISITED_JAIL</td>
      <td>bool</td>
      <td>Whether you visited the jail. No effects in the Chapter 1&2 demo. <br></td>
    </tr>
    <tr>
      <td>300</td>
      <td>Hugged - HUGGED_DUMMY_CH2</td>
      <td>bool</td>
      <td>Whether you hugged the dummy in Chapter 2. Some slight dialogue changes. <br></td>
    </tr>
    <tr>
      <td>301</td>
      <td>King dialogue - KING_JAIL_DIALOGUE_PROGRESS</td>
      <td>map</td>
      <td>Whether you talked to King in jail before visiting Cyber World. <br>0 = Default state<br>1 = Talked<br>2 = Left<br></td>
    </tr>
    <tr>
      <td>302</td>
      <td>Toy delivery - TOY_DELIVER_PROGRESS</td>
      <td>map</td>
      <td>Your progress in delivering Ralsei's first batch of subjects. <br>0 = Default state<br>1 = Ball on head<br>2 = Toys delivered<br></td>
    </tr>
    <tr>
      <td>303</td>
      <td>Saw Alphys and Toriel talk - BEEN_CALLED_NORMAL</td>
      <td>bool</td>
      <td>Whether you saw Alphys and Toriel talking about you. Alters Toriel's dialogue if called. <br></td>
    </tr>
    <tr>
      <td>304</td>
      <td>Susie ate the cake - SUSIE_ATE_CAKE</td>
      <td>bool</td>
      <td>Whether Susie ate Ralsei's entire cake (yet). <br></td>
    </tr>
    <tr>
      <td>305</td>
      <td>Told Toriel about studying - TOLD_MOM_STUDYING</td>
      <td>bool</td>
      <td>Whether you told Toriel you were going to be studying with Susie over the phone, with or without mentioning the trash orb. <br></td>
    </tr>
    <tr>
      <td>306</td>
      <td>Called Toriel with the trash orb - TOLD_MOM_ORB</td>
      <td>bool</td>
      <td>Whether you called Toriel while just around the corner with a trash orb on your head. Also sets flag 305. <br></td>
    </tr>
    <tr>
      <td>307</td>
      <td>Plush recipient - PLUSH_RECIPIENT</td>
      <td>map</td>
      <td>Records who you gave the plush to. In pre-1.08 versions, there's a bug resetting it to 1 before the acid river ride <br>0 = Default state<br>1 = Ralsei<br>2 = Susie<br>3 = Noelle<br>4 = Berdly<br></td>
    </tr>
    <tr>
      <td>308</td>
      <td>Saw the Asgore egg scene - SAW_EGGS_HUSBAND</td>
      <td>bool</td>
      <td>Whether you've seen Asgore make a fool of himself in public. <br></td>
    </tr>
    <tr>
      <td>309</td>
      <td>Quest progress - SPAMTON_QUEST_PROGRESS</td>
      <td>map</td>
      <td>Your progress in learning about the power of NEO. <br>0 = Default state<br>1 = Spared Spamton<br>3 = Purchased KeyGen<br>4 = Used KeyGen<br>5 = Entered basement<br>7 = Disk Loaded<br>8 = Disk inserted<br>9 = Defeated Spamton NEO<br></td>
    </tr>
    <tr>
      <td>310</td>
      <td>First cheese destroyed - FIRST_CHEESE_DESTROYED</td>
      <td>bool</td>
      <td>Whether the first cheese on the left was destroyed. <br></td>
    </tr>
    <tr>
      <td>311</td>
      <td>Triggered first cheese alone - DESTROYED_CHEESE_ALONE</td>
      <td>bool</td>
      <td>Whether you triggered the first cheese without Noelle, prompting slightly different text when interacting with it. <br></td>
    </tr>
    <tr>
      <td>312</td>
      <td>Talked to Seam - TALKED_TO_SEAM_CH2</td>
      <td>bool</td>
      <td>Set when you talk to Seam in Chapter 2, preventing them from repeating themselves. <br></td>
    </tr>
    <tr>
      <td>313</td>
      <td>Got SpinCake (fresh) - OBTAINED_SPINCAKE_CH2</td>
      <td>bool</td>
      <td>Whether you received a fresh Spincake since Chapter 2. <br></td>
    </tr>
    <tr>
      <td>314</td>
      <td>Mr. Society - MR_SOCIETY_LEFT</td>
      <td>bool</td>
      <td>Whether Mr. Society, the bishop, flew up the cliff after being talked to. <br></td>
    </tr>
    <tr>
      <td>315</td>
      <td>Saw the shelter scene - SAW_SHELTER_SCENE</td>
      <td>bool</td>
      <td>Whether Monster Kid and Snowy fled Susie at the bunker. They go home. <br></td>
    </tr>
    <tr>
      <td>316</td>
      <td>Saw hospital scene - SAW_HOSPITAL_SCENE</td>
      <td>bool</td>
      <td>Whether Noelle went home in Chapter 2 yet (yes, either route). <br></td>
    </tr>
    <tr>
      <td>317</td>
      <td>Dogs - POLICE_SCENE_PROGRESS</td>
      <td>map</td>
      <td>Tracks the state of the police station dog scene. <br>0 = Default state<br>1 = Dogs escaped<br>2 = Alarm playing<br></td>
    </tr>
    <tr>
      <td>319</td>
      <td>Ferris wheel scene state - FERRIS_WHEEL_SCENE_PROGRESS</td>
      <td>map</td>
      <td>Tracks progress through the Ferris wheel scene. <br>0 = Default state<br>1 = On Ferris wheel<br>2 = Off Ferris wheel<br>3 = WHAT? WHAT? WHAT?<br></td>
    </tr>
    <tr>
      <td>320</td>
      <td>Saw King and Queen reunite - SAW_KING_QUEEN_REUNION</td>
      <td>bool</td>
      <td>Whether you've seen the touching reunion of King and Queen. <br></td>
    </tr>
    <tr>
      <td>324</td>
      <td>Post-NEO stress response - SPAMTON_STRESS_RESPONSE</td>
      <td>map</td>
      <td>What you said- made Kris say- after fighting Spamton NEO. <br>0 = Default state<br>1 = OK<br>2 = Not OK<br></td>
    </tr>
    <tr>
      <td>325</td>
      <td>Photo - RALSEI_PHOTO_STATE</td>
      <td>map</td>
      <td>The purty picture you took with Ralsei. Affects his title and whether he hugs Kris after Spamton NEO. <br>0 = Default state<br>1 = Hugged<br>2 = Peace sign<br>3 = Rude gesture<br>4 = No pose<br></td>
    </tr>
    <tr>
      <td>326</td>
      <td>Rouxls wearing pirate hat - ROUXLS_PIRATE_HAT</td>
      <td>bool</td>
      <td>Whether Rouxls Kaard is currently wearing a pirate hat. <br></td>
    </tr>
    <tr>
      <td>327</td>
      <td>Seated Head Hathy with Werewerewire - SEATED_HEAD_HATHY_WITH_WEREWEREWIRE</td>
      <td>bool</td>
      <td>Whether you interacted with a Head Hathy or Werewerewire together at the cafe. Alters Werewerewire narration if subsequently moved away from Head Hathy. <br></td>
    </tr>
    <tr>
      <td>329</td>
      <td>Talked to Spamton about the Knight - TALKED_TO_SPAMTON_ABOUT_KNIGHT</td>
      <td>bool</td>
      <td>Whether you talked with Spamton about the Knight, changing his talk option to Friends. <br></td>
    </tr>
    <tr>
      <td>330</td>
      <td>Found the Tasque-maze switch - FOUND_TASQUE_SWITCH</td>
      <td>bool</td>
      <td>Whether you found the switch that controls the faint hint in the Tasque maze. <br></td>
    </tr>
    <tr>
      <td>331</td>
      <td>Saw the Ferris wheel scene - SAW_FERRIS_SCENE</td>
      <td>bool</td>
      <td>Set to 1 after the Ferris wheel scene, even if skipped. <br></td>
    </tr>
    <tr>
      <td>332</td>
      <td>Found the old maze switch - FOUND_MAZE_SWITCH</td>
      <td>bool</td>
      <td>Whether you found the old variant of the Tasque-maze switch. <br></td>
    </tr>
    <tr>
      <td>333</td>
      <td>Solved AGREE2ALL puzzle - SOLVED_AGREE2ALL_PUZZLE</td>
      <td>bool</td>
      <td>Whether you solved the AGREE2ALL puzzle. <br></td>
    </tr>
    <tr>
      <td>335</td>
      <td>Opened the shovel door - SHOVEL_DOOR_OPEN</td>
      <td>bool</td>
      <td>Whether you opened the door to the room filled with 999 shovels. <br></td>
    </tr>
    <tr>
      <td>336</td>
      <td>Susie avoiding Alphys - SUSIE_AVOID_ALPHYS</td>
      <td>bool</td>
      <td>Whether Susie is waiting due east of you rather than come close to Alphys. <br></td>
    </tr>
    <tr>
      <td>337</td>
      <td>Alvin - ALVIN_DIALOGUE_PROGRESS</td>
      <td>map</td>
      <td>Tracks how much you talk to Alvin about his father and the hammer, and whether he mumbles to himself as you leave. <br>0 = Default state<br>1 = Talked once<br>2 = Talked twice<br>3 = Heard mumbling<br></td>
    </tr>
    <tr>
      <td>339</td>
      <td>Found the basement switch - FOUND_BASEMENT_SWITCH</td>
      <td>bool</td>
      <td>Whether you activated the secret backdoor to the mansion's basement. Alter's Hacker's dialogue. <br></td>
    </tr>
    <tr>
      <td>340</td>
      <td>Found the basement shortcut - FOUND_SHORTCUT_OUT</td>
      <td>bool</td>
      <td>Whether you flipped the less-secret switch to connect the basement to the foyer. Also set on entry into the foyer on Snowgrave. <br></td>
    </tr>
    <tr>
      <td>341</td>
      <td>Susie avoiding diner - SUSIE_AVOID_CATTI</td>
      <td>bool</td>
      <td>Whether Susie has told you she isn't going into the diner (Catti's working there!) <br></td>
    </tr>
    <tr>
      <td>342</td>
      <td>Chocolate recipient - CHOCOLATE_RECIPIENT</td>
      <td>map</td>
      <td>Who did you give the Box of Heart-Shaped Chocolates to? <br>0 = Default value<br>1 = Ate alone<br>2 = Shared with Susie<br>3 = Gave to Alphys<br>4 = Returned to Sans<br></td>
    </tr>
    <tr>
      <td>343</td>
      <td>Made the giant high-five - MADE_HIGH_FIVE</td>
      <td>bool</td>
      <td>Whether you pulled the lever to make a giant high-five and progress the swan ride. <br></td>
    </tr>
    <tr>
      <td>344</td>
      <td>Solved first saucer puzzle - SOLVED_FIRST_SAUCER_PUZZLE</td>
      <td>bool</td>
      <td>Looks to be set to 1 when completing the first shell game-style saucer puzzle. <br></td>
    </tr>
    <tr>
      <td>345</td>
      <td>Checked the Berdly toilet statue - SAW_TOILET_STATUE</td>
      <td>bool</td>
      <td>Whether you interacted with the Berdly statue in the toilet. Spawns the NPC outside waiting for the statue to finish in there. <br></td>
    </tr>
    <tr>
      <td>346</td>
      <td>Solved the saucer shortcut - SOLVED_SAUCER_SHORTCUT</td>
      <td>bool</td>
      <td>Whether you've unlocked a shortcut in Mansion by doing a saucer puzzle. I don't know which. <br></td>
    </tr>
    <tr>
      <td>347</td>
      <td>Toilet statue interactions - SEEN_STATUE_COUNT</td>
      <td>number</td>
      <td>The number of times you interacted with the Berdly statue with Noelle with you. She has unique comments up to 8 on how obsessed you are with it. <br></td>
    </tr>
    <tr>
      <td>349</td>
      <td>Froze the chicken - FROZEN_CHICKEN</td>
      <td>bool</td>
      <td>Whether there is a large ice crystal you cannot see into blocking the way. <br></td>
    </tr>
    <tr>
      <td>350</td>
      <td>Werewired Fedora Plugboy - FEDORA_PLUGBOY_WEREWIRED</td>
      <td>bool</td>
      <td>Whether you walked far enough away for the fedora'd Plugboy to get Werewired offscreen. <br></td>
    </tr>
    <tr>
      <td>351</td>
      <td>Queen screen maze hint - UNUSED_CYBER_MAZE_HINT</td>
      <td>bool</td>
      <td>Unused flag for a hint popup in room_dw_cyber_maze_queenscreen. <br></td>
    </tr>
    <tr>
      <td>352</td>
      <td>Solved Viro Dodge - SOLVED_VIROVIROKUN_DODGE</td>
      <td>bool</td>
      <td>Whether you got the key in room_dw_cyber_viro_ring. <br></td>
    </tr>
    <tr>
      <td>353</td>
      <td>Talk Two Crystals - SEAM_TWO_CRYSTALS_DIALOGUE_PROGRESS</td>
      <td>map</td>
      <td>How much you've talked to Seam since obtaining both Shadow Crystals. <br>0 = Default state<br>1 = Gave both<br>2 = Talked about mantle<br></td>
    </tr>
    <tr>
      <td>354</td>
      <td>CD Bagels - CD_BAGELS_PURCHASED</td>
      <td>number</td>
      <td>The number of CD Bagels you purchased from K_K. He stops selling them at six, in case somebody orders 400. <br></td>
    </tr>
    <tr>
      <td>356</td>
      <td>Cared for Lancer - LANCER_CARED_FOR</td>
      <td>bool</td>
      <td>Whether statue-Lancer has been pushed to the table and given his adorable bib. <br></td>
    </tr>
    <tr>
      <td>357</td>
      <td>Recruited - RECRUITED_HACKER</td>
      <td>bool</td>
      <td>Whether you talked to Hacker after collecting all three Blue Checksmarks. <br></td>
    </tr>
    <tr>
      <td>358</td>
      <td>Basement entries - ENTERED_BASEMENT_COUNT</td>
      <td>number</td>
      <td>Tracks how many times you entered the basement alone. Does not go past 1 until you've seen Susie stealing Ralsei's glasses, after which it gets set to 2. <br></td>
    </tr>
    <tr>
      <td>359</td>
      <td>Met Hacker - MET_HACKER</td>
      <td>map</td>
      <td>Whether you talked to Hacker. Note that the 2 state isn't directly used; see flag 357. <br>0 = Default state<br>1 = Talked<br>2 = Recruited<br></td>
    </tr>
    <tr>
      <td>360</td>
      <td>Approached Cheese Maze - APPROACHED_CHEESE_MAZE</td>
      <td>bool</td>
      <td>Whether you've approached the cheese maze, destroying the lone cheese or triggering Noelle dialogue if it's already destroyed. <br></td>
    </tr>
    <tr>
      <td>361</td>
      <td>Did Right Cheese Fight - DID_RIGHT_CHEESE_FIGHT</td>
      <td>bool</td>
      <td>Unused right-cheese encounter flag. <br></td>
    </tr>
    <tr>
      <td>362</td>
      <td>Defeated Mauswheel - MAUSWHEEL_DEFEATED</td>
      <td>bool</td>
      <td>Whether you defeated Mauswheel on the normal route, freeing the Swatchlings. <br></td>
    </tr>
    <tr>
      <td>366</td>
      <td>Released Tasque - TASQUE_RELEASED</td>
      <td>bool</td>
      <td>Makes one particular Tasque persist after leaving the wall screen in Field. <br></td>
    </tr>
    <tr>
      <td>367</td>
      <td>Got Chestmark 1 - OBTAINED_CHESTMARK</td>
      <td>bool</td>
      <td>Whether you got the Blue Checksmark from a treasure chest. <br></td>
    </tr>
    <tr>
      <td>368</td>
      <td>Solved Mice 2 - SOLVED_MICE_2</td>
      <td>map</td>
      <td>Progress on solving the second mice puzzle. <br>0 = Default state<br>1 = Forcefield down<br>0.5 = Mice in hole<br></td>
    </tr>
    <tr>
      <td>369</td>
      <td>Had Noelle see Ralsei and Susie - NOELLE_SAW_RALSEI_AND_SUSIE</td>
      <td>bool</td>
      <td>Whether Noelle gave her one-time dialogue about seeing Ralsei and Susie having fun. <br></td>
    </tr>
    <tr>
      <td>370</td>
      <td>Solved Mansion Traffic - SOLVED_MANSION_TRAFFIC</td>
      <td>bool</td>
      <td>Whether the traffic challenge at the end of floor 1F was completed, opening the room with the backdoor switch. <br></td>
    </tr>
    <tr>
      <td>371</td>
      <td>Fought Tasque Manager - FOUGHT_TASQUE_MANAGER</td>
      <td>bool</td>
      <td>Whether you fought Tasque Manager. <br></td>
    </tr>
    <tr>
      <td>373</td>
      <td>Unlocked East Basement - UNLOCKED_EAST_BASEMENT</td>
      <td>bool</td>
      <td>Whether you disabled the forcefield in the basement with the final boss. Yeah, the teacups. <br></td>
    </tr>
    <tr>
      <td>374</td>
      <td>Gave the mice $20 - MICE_RECEIVED_20_DOLLARS</td>
      <td>bool</td>
      <td>Whether the mice got $20. Alters Mousemillian's dialogue. <br></td>
    </tr>
    <tr>
      <td>375</td>
      <td>Gave the mice $1 - MICE_RECEIVED_1_DOLLAR</td>
      <td>bool</td>
      <td>Whether the mice got $1. Alters Mousemillian's dialogue. <br></td>
    </tr>
    <tr>
      <td>376</td>
      <td>Vase room - SWATCHLING_VASE_ROOM_PROGRESS</td>
      <td>map</td>
      <td>Progress in the room with the Swatchling and the bridges and the unavoidable vase. <br>0 = Default state<br>1 = Swatchling freed<br>2 = Vase spawned<br></td>
    </tr>
    <tr>
      <td>377</td>
      <td>Mouselottery Solved - MOUSE_LOTTERY_RESULT_1</td>
      <td>bool</td>
      <td>Whether the mice have triggered the blue house. <br></td>
    </tr>
    <tr>
      <td>378</td>
      <td>Mouselottery Solved 2 - MOUSE_LOTTERY_RESULT_2</td>
      <td>bool</td>
      <td>Whether the mice have triggered the red house. <br></td>
    </tr>
    <tr>
      <td>379</td>
      <td>Helped Noelle overcome her fear - NOELLE_BEAT_FEAR</td>
      <td>bool</td>
      <td>Whether Noelle stopped being afraid of mice. <br></td>
    </tr>
    <tr>
      <td>380</td>
      <td>Called Mom After Lab - CALLED_MOM_AFTER_LAB</td>
      <td>bool</td>
      <td>Whether you called Toriel after leaving the computer lab. Prevents her from repeating her dialogue. <br></td>
    </tr>
    <tr>
      <td>381</td>
      <td>Had the dog open the door - DOG_OPENED_DOOR</td>
      <td>bool</td>
      <td>Whether the dog, ah, forced open the double door in the bajillion platters room in the mansion. <br></td>
    </tr>
    <tr>
      <td>382</td>
      <td>Completed the dining hall - DINING_HALL_COMPLETE</td>
      <td>bool</td>
      <td>Whether you finished the ultimate dining hall puzzle. <br></td>
    </tr>
    <tr>
      <td>383</td>
      <td>Solved Forcefield 1 - SOLVED_FORCEFIELD_1</td>
      <td>bool</td>
      <td>Whether you successfully activated both switches in the first forcefield puzzle, disabling it forever. <br></td>
    </tr>
    <tr>
      <td>384</td>
      <td>Fought Cheese Maze - FOUGHT_CHEESE_MAZE</td>
      <td>bool</td>
      <td>Whether you touched the cheese maze, triggering an encounter and destroying it. <br></td>
    </tr>
    <tr>
      <td>385</td>
      <td>Balance Pot Status - VASE_BALANCING_OUTCOME</td>
      <td>map</td>
      <td>What happened in the vase-balancing minigame. <br>0 = Default state<br>1 = Dropped pot<br>2 = Success<br></td>
    </tr>
    <tr>
      <td>386</td>
      <td>Visited Spamton - VISITED_SPAMTON</td>
      <td>map</td>
      <td>Prevents you from getting repeat dialogue every single time you visit Spamton's shop. <br>0 = Default state<br>1 = First time in shop<br>2 = Exited<br></td>
    </tr>
    <tr>
      <td>387</td>
      <td>Saw Queen introduce herself to Castle Town - RETURNED_CASTLE_TOWN</td>
      <td>bool</td>
      <td>Whether you've seen Queen introduce herself to Castle Town. <br></td>
    </tr>
    <tr>
      <td>388</td>
      <td>Sealed the Fountain with no recruits - OBTAINED_NO_RECRUITS</td>
      <td>bool</td>
      <td>Whether you sealed the Fountain with no recruits at all, on the normal route anyway. <br></td>
    </tr>
    <tr>
      <td>389</td>
      <td>Fought Bridge Werewire - FOUGHT_BRIDGE_WEREWIRE</td>
      <td>bool</td>
      <td>Whether you fought the Werewire in the acid lake bridge room, unlocking the Revive Dust chest. <br></td>
    </tr>
    <tr>
      <td>390</td>
      <td>Solved Apple Puzzle - SOLVED_APPLE_PUZZLE</td>
      <td>bool</td>
      <td>Whether you unlocked the way to NUBERT'S TREASURE. <br></td>
    </tr>
    <tr>
      <td>391</td>
      <td>Fought First Viro - ENCOUNTERED_FIRST_VIROVIROKUN</td>
      <td>bool</td>
      <td>Tracks whether you've encountered the first Virovirokun. When set, it will fly around in a circle instead of staying still. <br></td>
    </tr>
    <tr>
      <td>392</td>
      <td>3F bookcase shortcut (Snowgrave) - MANSION_THIRD_FLOOR_SHORTCUT_UNLOCKED</td>
      <td>bool</td>
      <td>Unlocks a mansion shortcut early on the Snowgrave Route. <br></td>
    </tr>
    <tr>
      <td>393</td>
      <td>Stole Susie statue - STOLE_SUSIE_STATUE</td>
      <td>bool</td>
      <td>Whether you stole the Susie statue from Noelle's room. <br></td>
    </tr>
    <tr>
      <td>394</td>
      <td>Stole Ice-E statue - STOLE_ICE_E_STATUE</td>
      <td>bool</td>
      <td>Whether you stole the Ice-E statue from Noelle's room. <br></td>
    </tr>
    <tr>
      <td>395</td>
      <td>Opened Side A painting - OPENED_SIDE_A_PAINTING</td>
      <td>bool</td>
      <td>Whether a painting opened a passageway. <br></td>
    </tr>
    <tr>
      <td>396</td>
      <td>Opened Side B painting - OPENED_SIDE_PAINTING_B</td>
      <td>bool</td>
      <td>Whether a painting opened a passageway. <br></td>
    </tr>
    <tr>
      <td>397</td>
      <td>Activated Queen's paintings - ACTIVATED_QUEEN_PAINTINGS</td>
      <td>bool</td>
      <td>Whether Queen warned you not to take your eyes off her paintings, and activated the painting fireballs. <br></td>
    </tr>
    <tr>
      <td>398</td>
      <td>Activated mint painting - ACTIVATED_MINT_PAINTING</td>
      <td>bool</td>
      <td>Whether you activated the Revive Mint painting with a different painting. <br></td>
    </tr>
    <tr>
      <td>399</td>
      <td>Activated the painting exit - ACTIVATED_PAINTING_EXIT</td>
      <td>bool</td>
      <td>Whether you disabled a fire painting blocking the exit by interacting with a different painting. <br></td>
    </tr>
    <tr>
      <td>400</td>
      <td>Vase Intro Status - MANSION_VASE_TUTORIAL_PROGRESS</td>
      <td>map</td>
      <td>Your progress in learning the basics of Queen's Mansion. <br>0 = Default state<br>1 = Learned rules<br>2 = Broke vase<br></td>
    </tr>
    <tr>
      <td>407</td>
      <td>Got Chestmark 2 - OBTAINED_CHESTMARK_2</td>
      <td>bool</td>
      <td>Whether you got the second Chest-Checksmark. <br></td>
    </tr>
    <tr>
      <td>408</td>
      <td>Saw Sweet Cap'n Cakes fly by - SAW_SWEET_CAPN_CAKES_FLYBY</td>
      <td>bool</td>
      <td>Whether you saw Sweet Cap'n Cakes fly by after fighting them. <br></td>
    </tr>
    <tr>
      <td>409</td>
      <td>Inspected Kris's bed - INSPECTED_KRIS_BED</td>
      <td>bool</td>
      <td>Whether you inspected your own bed. Necessary to retain your Bed Inspector title. <br></td>
    </tr>
    <tr>
      <td>410</td>
      <td>Inspected Susie's bed - INSPECTED_SUSIE_BED</td>
      <td>bool</td>
      <td>Whether you inspected Susie's bed. Necessary to retain your Bed Inspector title. <br></td>
    </tr>
    <tr>
      <td>411</td>
      <td>Inspected Lancer's bed - INSPECTED_LANCER_BED</td>
      <td>bool</td>
      <td>Whether you inspected Lancer's bed. Necessary to retain your Bed Inspector title. <br></td>
    </tr>
    <tr>
      <td>412</td>
      <td>Inspected Clover's bed - INSPECTED_CLOVER_BED</td>
      <td>bool</td>
      <td>Whether you inspected Clover's bed. Necessary to retain your Bed Inspector title. Only obtainable on v1.09+ due to a bug. <br></td>
    </tr>
    <tr>
      <td>413</td>
      <td>Inspected Noelle's bed - INSPECTED_NOELLE_BED</td>
      <td>bool</td>
      <td>Whether you inspected Noelle's bed. Necessary to retain your Bed Inspector title. <br></td>
    </tr>
    <tr>
      <td>414</td>
      <td>Earned Bed Inspector - BED_INSPECTOR_CH2</td>
      <td>bool</td>
      <td>Whether you retained your Bed Inspector title. That is, got slightly different Noelle bed dialogue. Only obtainable on v1.09+ due to a bug. <br></td>
    </tr>
    <tr>
      <td>415</td>
      <td>Mice Attack Reason - MICE_ATTACK_REASON</td>
      <td>map</td>
      <td>What you told Noelle about the mice attacking her. The question was, "What do I look like, the girl from the Nutcracker?" <br>0 = Default state<br>1 = They like you<br>2 = Unknown<br>3 = You look like her<br></td>
    </tr>
    <tr>
      <td>416</td>
      <td>Triggered Field Tempsave - TRIGGERED_CYBER_FIELD_TEMP_SAVE</td>
      <td>bool</td>
      <td>Whether you returned to the Cyber Field hub after defeating Sweet Cap'n Cakes and triggered a tempsave. <br></td>
    </tr>
    <tr>
      <td>417</td>
      <td>Triggered Trash Tempsave - TRIGGERED_TRASH_ZONE_TEMP_SAVE</td>
      <td>bool</td>
      <td>Whether you reached Cyber City by falling into the dump and triggered a tempsave. <br></td>
    </tr>
    <tr>
      <td>418</td>
      <td>Got Shoe - OBTAINED_SHOE</td>
      <td>bool</td>
      <td>Whether you got a free sample from Cyber Shoes. Alters Lancer's dialogue and prevents a Mansion tempsave from happening (reused flag). <br></td>
    </tr>
    <tr>
      <td>419</td>
      <td>Tasque Manager Response - TASQUE_MANAGER_RESPONSE</td>
      <td>map</td>
      <td>Whether you got all or most of Tasque Manager's questions correct. She starts with 100% if all, 50% if you miss the last due to her phrasing. <br>0 = Default state<br>1 = All correct<br>2 = Thought alphabetical<br></td>
    </tr>
    <tr>
      <td>420</td>
      <td>Solved the typing puzzle - SOLVED_GIASFCLFEBREBREBEHR_PUZZLE</td>
      <td>bool</td>
      <td>Whether you solved the Giasfclfebrebrebrebehr typing puzzle, earning the third Blue Checksmark. <br></td>
    </tr>
    <tr>
      <td>421</td>
      <td>Noelle Friend - NOELLE_RELATIONSHIP_RESPONSE</td>
      <td>map</td>
      <td>Whether you told Noelle you were "something else." Necessary for Snowgrave. <br>0 = Friends<br>1 = Something else<br></td>
    </tr>
    <tr>
      <td>422</td>
      <td>Talked to Mettaton - TALKED_TO_METTATON_CH2</td>
      <td>bool</td>
      <td>Whether you talked to Mettaton in Chapter 2. They don't repeat themselves. <br></td>
    </tr>
    <tr>
      <td>423</td>
      <td>Stolen Bagels - STOLEN_BAGELS</td>
      <td>number</td>
      <td>How many CD Bagels you stole on the Snowgrave Route (0-4). <br></td>
    </tr>
    <tr>
      <td>424</td>
      <td>Talked to Onion - TALKED_TO_ONION_CH2</td>
      <td>bool</td>
      <td>Whether you talked to Onionsan in Chapter 2. <br></td>
    </tr>
    <tr>
      <td>425</td>
      <td>Missed - ONION_WAS_MISSED</td>
      <td>map</td>
      <td>What you told Onion. <br>0 = Default state<br>1 = Missed<br>2 = Did not miss<br></td>
    </tr>
    <tr>
      <td>426</td>
      <td>Swatchling fight combo - SWATCHLING_COMBO</td>
      <td>map</td>
      <td>Volatile. The current combination of Swatchlings you are fighting. Later ones are harder, generally. <br>0 = ROB<br>1 = BGY<br>2 = ROY<br>3 = BYR<br>4 = RBY<br>5 = BYG<br>6 = RYB<br>7 = BRY<br>8 = YGO<br>-1 = RRB<br></td>
    </tr>
    <tr>
      <td>427</td>
      <td>Unlocked the mint chest - UNLOCKED_MINT_CHEST</td>
      <td>bool</td>
      <td>Whether Virovirokun triggered the hidden path to the Revive Mint chest. <br></td>
    </tr>
    <tr>
      <td>428</td>
      <td>Saw Sweet - SAW_SWEET</td>
      <td>bool</td>
      <td>Whether you saw Sweet right after the first teacup ride. Prevents him from appearing multiple times. <br></td>
    </tr>
    <tr>
      <td>429</td>
      <td>Statue sink - STATUE_SINK_PROGRESS</td>
      <td>number</td>
      <td>The amount by which the statue of Queen has sunk into the acid, in frames, so it persists even if you leave. <br></td>
    </tr>
    <tr>
      <td>430</td>
      <td>Took Asriel's $5 - TOOK_AZZY_MONEY</td>
      <td>bool</td>
      <td>Whether you took five bucks from Asriel's drawer. <br></td>
    </tr>
    <tr>
      <td>431</td>
      <td>Talked to Jigsaw Joe - TALKED_TO_JIGSAW_JOE_CH2</td>
      <td>bool</td>
      <td>Whether you talked to Jigsaw Joe yet in the Party Dojo, which he introduces. <br></td>
    </tr>
    <tr>
      <td>432</td>
      <td>Told To Explore - TOLD_TO_EXPLORE</td>
      <td>bool</td>
      <td>Whether Ralsei told you and Susie to explore the Castle Town yet. <br></td>
    </tr>
    <tr>
      <td>433</td>
      <td>Told to run - TOLD_TO_RUN_CH2</td>
      <td>bool</td>
      <td>Whether Susie reminded you that you can run in this game (if you fail to do so in the chapter). <br></td>
    </tr>
    <tr>
      <td>434</td>
      <td>Heard Spamton explain the deal - HEARD_SPAMTON_DEAL_EXPLANATION</td>
      <td>bool</td>
      <td>Whether Spamton told you about our deal and the machine in the basement. Prevents him from skipping it if you buy KeyGen first. <br></td>
    </tr>
    <tr>
      <td>435</td>
      <td>House Game Winner - HOUSE_GAME_WINNER</td>
      <td>map</td>
      <td>Who won Rouxls's house minigame. <br>0 = Default state<br>1 = Rouxls<br>2 = Kris<br>3 = Draw<br></td>
    </tr>
    <tr>
      <td>436</td>
      <td>Called home during the ending - CALLED_MOM_BUSY</td>
      <td>bool</td>
      <td>Whether you called home during the Chapter 2 end sequence. Unique dialogue the first time, then everyone's too busy to pick it up. <br></td>
    </tr>
    <tr>
      <td>437</td>
      <td>Fave Party Member 2 - FESTIVAL_COMPANION_RESPONSE</td>
      <td>map</td>
      <td>Who you told Susie you would take to the festival in the Chapter 2 end cutscene. Unaccessed. <br>0 = Default state<br>1 = Noelle<br>2 = Ralsei<br>3 = Susie<br>4 = ...<br></td>
    </tr>
    <tr>
      <td>438</td>
      <td>Tutor Viro Location - TUTORIAL_VIROVIROKUN_LOCATION</td>
      <td>map</td>
      <td>Where you fought the tutorial Virovirokun. Persists its ice statue in Snowgrave. <br>0 = Default state<br>1 = Progressed<br>2 = Backtracked<br></td>
    </tr>
    <tr>
      <td>439</td>
      <td>Deposited the egg - DEPOSITED_EGG_CH2</td>
      <td>bool</td>
      <td>Whether you put the egg in the egg basket in Sans's store. <br></td>
    </tr>
    <tr>
      <td>440</td>
      <td>Checked the Ferris wheel poster - INTERACTED_WITH_FERRIS_POSTER</td>
      <td>bool</td>
      <td>Whether you interacted with the Ferris wheel poster with Noelle. One-time event. <br></td>
    </tr>
    <tr>
      <td>441</td>
      <td>Talked to the Dating Shoes Addison - TALKED_TO_DATING_SHOES_ADDISON</td>
      <td>bool</td>
      <td>Whether you talked to the Addison selling Dating Shoes. One-time event. See also flag 421. <br></td>
    </tr>
    <tr>
      <td>442</td>
      <td>Learned the teacup controls - LEARNED_TEACUPS</td>
      <td>bool</td>
      <td>Whether you've taken your first teacup ride and possibly gotten a tutorial on operating it. <br></td>
    </tr>
    <tr>
      <td>443</td>
      <td>Heard Ralsei explain saving - TOLD_SAVE_TOWN</td>
      <td>bool</td>
      <td>Whether Ralsei told you to feel free to SAVE and take a break in Castle Town. <br></td>
    </tr>
    <tr>
      <td>444</td>
      <td>Heard Susie suggest Castle Town - TOLD_VISIT_TOWN</td>
      <td>bool</td>
      <td>Whether Susie told you to go back and check out Castle Town, if you went down south first. <br></td>
    </tr>
    <tr>
      <td>445</td>
      <td>Read the cleaning poster - READ_CLEANING_POSTER</td>
      <td>bool</td>
      <td>Whether you interacted with the poster for Queen Cleaning Agent with Noelle behind you. Interesting dialogue exclusive to non-Snowgrave. <br></td>
    </tr>
    <tr>
      <td>446</td>
      <td>Went Weird Door - WENT_WEIRD_DOOR</td>
      <td>bool</td>
      <td>Whether you brought Noelle all the way back to the gray door. Unique dialogue about its creepiness, but not required for Snowgrave. <br></td>
    </tr>
    <tr>
      <td>447</td>
      <td>Broke Balloon Cheese - BROKE_BALLOON_CHEESE</td>
      <td>bool</td>
      <td>Whether the balloon cheese, found right before the mice basket puzzle, was dropped. <br></td>
    </tr>
    <tr>
      <td>448</td>
      <td>Finished Big Forcefield - FINISHED_BIG_FORCEFIELD</td>
      <td>bool</td>
      <td>Whether you finished and disabled the right-side forcefields in that room where Noelle stands on a button forever. <br></td>
    </tr>
    <tr>
      <td>449</td>
      <td>Triggered the forcefield easter egg - EASTER_EGG_FORCEFIELD</td>
      <td>bool</td>
      <td>Whether you disabled the Easter egg forcefield (with the balloons) by all getting in one teacup. <br></td>
    </tr>
    <tr>
      <td>450</td>
      <td>Teacup easter egg - BALLOON_TEACUP_EASTER_EGG_PROGRESS</td>
      <td>map</td>
      <td>Progress in the balloon-teacup Easter egg. <br>0 = Default state<br>1 = Read sign<br>2 = Rode teacups<br></td>
    </tr>
    <tr>
      <td>451</td>
      <td>Talked to Sans about Papyrus - TALKED_TO_SANS_ABOUT_PAPYRUS</td>
      <td>bool</td>
      <td>Whether you talked to Sans about Papyrus in both chapters 1 and 2; talking in Chapter 2 only isn't saved. <br></td>
    </tr>
    <tr>
      <td>452</td>
      <td>Told Wrongway - TOLD_WRONGWAY</td>
      <td>bool</td>
      <td>Whether Noelle questioned if you were going the right way while backtracking further into the trash zone. <br></td>
    </tr>
    <tr>
      <td>453</td>
      <td>Talked to Spamton behind the basement door - TALKED_TO_SPAMTON_BEHIND_BASEMENT_DOOR</td>
      <td>bool</td>
      <td>Whether you talked to Spamton through the basement door while he was changing forms. He doesn't repeat himself. <br></td>
    </tr>
    <tr>
      <td>454</td>
      <td>Got Dealmaker - OBTAINED_DEALMAKER</td>
      <td>bool</td>
      <td>Whether you spared Spamton NEO. <br></td>
    </tr>
    <tr>
      <td>455</td>
      <td>Ride With Me - RIDE_WITH_ME</td>
      <td>bool</td>
      <td>Whether you said "Noelle will ride with me" on Snowgrave. Unaccessed. <br></td>
    </tr>
    <tr>
      <td>456</td>
      <td>Defeated SnowGrave NEO - DEFEATED_SNOWGRAVE_NEO</td>
      <td>bool</td>
      <td>Whether you defeated Spamton NEO on Snowgrave. <br></td>
    </tr>
    <tr>
      <td>457</td>
      <td>Spared all three - SPARED_BERDLY_ALL_THREE_TIMES</td>
      <td>bool</td>
      <td>Whether you spared Berdly all three times, keeping him from breaking his arm. <br></td>
    </tr>
    <tr>
      <td>458</td>
      <td>Houses hit - HOUSES_HIT</td>
      <td>number</td>
      <td>The number of houses you hit with the swan boat, converted to TP at the start of the Rouxls fight. Maximum 7. <br></td>
    </tr>
    <tr>
      <td>459</td>
      <td>Put the disk in the mannequin - PUT_DISK_MANNEQUIN</td>
      <td>bool</td>
      <td>Whether you tried to put the LoadedDisk into the Mannequin. It doesn't repeat. <br></td>
    </tr>
    <tr>
      <td>460</td>
      <td>Got the Jevil-hole item - OBTAINED_JEVIL_HOLE</td>
      <td>bool</td>
      <td>Whether you got the Jevil item from the Castle Town hole. Accessed, but not necessary. <br></td>
    </tr>
    <tr>
      <td>461</td>
      <td>Used the sink - INTERACTED_WITH_SINK_CH2</td>
      <td>bool</td>
      <td>Whether you interacted with Rudy's sink in Chapter 2. See also flag 278. <br></td>
    </tr>
    <tr>
      <td>462</td>
      <td>Cars hit - CARS_HIT</td>
      <td>number</td>
      <td>The number of cars you hit. If less than 3 and you're otherwise pacifistic enough, you get the Castle Town tiny car. <br></td>
    </tr>
    <tr>
      <td>463</td>
      <td>Read the Cyberpedia - READ_CYBERPEDIA</td>
      <td>bool</td>
      <td>Whether you read Ralsei's editable Cyberpedia entry. <br></td>
    </tr>
    <tr>
      <td>464</td>
      <td>Talked to Swatch about Topchef - TALKED_TO_SWATCH_ABOUT_TOPCHEF</td>
      <td>bool</td>
      <td>Whether you talked to Swatch in the Castle Town Cafe about removing Topchef. Poor man. <br></td>
    </tr>
    <tr>
      <td>465</td>
      <td>Completed the car section - CAR_PART_COMPLETED</td>
      <td>bool</td>
      <td>Whether you completed the car sequence. You can't get the tiny car on Snowgrave, even with all recruits, because of this. <br></td>
    </tr>
    <tr>
      <td>466</td>
      <td>Dropped the junk ball - JUNKBALL_DROPPED</td>
      <td>bool</td>
      <td>Whether you dropped the Ball of Junk at any point. Unaccessed. <br></td>
    </tr>
    <tr>
      <td>467</td>
      <td>Opened Chestmark - CHESTMARK_OPENED</td>
      <td>bool</td>
      <td>Keeps you from opening the Chestmark chest multiple times. <br></td>
    </tr>
    <tr>
      <td>468</td>
      <td>Spamton No Room - SPAMTON_NO_ROOM</td>
      <td>map</td>
      <td>Whether you had no room after defeating Spamton NEO. Spawns the chest. <br>0 = Default state<br>1 = No room Pacifist<br>2 = No room Snowgrave<br></td>
    </tr>
    <tr>
      <td>469</td>
      <td>Saw the no-return tip - CANT_GO_BACK_TIP</td>
      <td>bool</td>
      <td>Whether the save point reminded you that you can't go back to the Cyber World if you overwrite your save in Castle Town. Consider this carefully! <br></td>
    </tr>
    <tr>
      <td>500</td>
      <td>First Rudinn fight count - RUDINN_FIGHT_COUNT</td>
      <td>number</td>
      <td>The number of times you've fought the first Rudinn. Changes its encounter text. <br></td>
    </tr>
    <tr>
      <td>501</td>
      <td>Triple Hathy encounter state - TRIPLE_HATHY_OUTCOME</td>
      <td>map</td>
      <td>Tracks an unused room_field2 encounter state and related dialogue. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>502</td>
      <td>Ponman fight count - PONMAN_FIGHT_COUNT</td>
      <td>number</td>
      <td>The number of times you fought Ponmen. Minor changes to the overworld chasing Ponmen. <br></td>
    </tr>
    <tr>
      <td>503</td>
      <td>Susie complimented Rudinn Ranger - SUSIE_COMPLIMENT_COUNT</td>
      <td>bool</td>
      <td>Whether Susie has attempted to compliment Rudinn Ranger. Free ham sandwich day does not repeat. <br></td>
    </tr>
    <tr>
      <td>504</td>
      <td>Susie flirt attempts on Head Hathy - SUSIE_FLIRT_COUNT</td>
      <td>number</td>
      <td>The number of times you used X-Flirt on Head Hathy. She tries the first time, makes Ralsei try the second, and you take over from the third. <br></td>
    </tr>
    <tr>
      <td>505</td>
      <td>Fought Rabbick - FOUGHT_RABBICK</td>
      <td>bool</td>
      <td>Whether you fought any Rabbicks. If so, they run slower in the forest maze. Also set when you fight Clover. <br></td>
    </tr>
    <tr>
      <td>506</td>
      <td>Fought Bloxer - FOUGHT_BLOXER</td>
      <td>bool</td>
      <td>Whether you fought Bloxer. If so, they don't chase you as diligently. <br></td>
    </tr>
    <tr>
      <td>507</td>
      <td>Fought Rudinn Ranger - FOUGHT_RUDINN_RANGER</td>
      <td>bool</td>
      <td>Whether you fought Rudinn Ranger. If so, they don't chase you at all. <br></td>
    </tr>
    <tr>
      <td>508</td>
      <td>Fought Head Hathy - FOUGHT_HATHYX</td>
      <td>bool</td>
      <td>Whether you fought Head Hathy. If so, they don't chase you at all. <br></td>
    </tr>
    <tr>
      <td>509</td>
      <td>Pippins Ralsei ACT - PIPPINS_BRIBE_ACT_COUNT</td>
      <td>number</td>
      <td>Number of Bribe ACTs used on Pippins. Unique dialogue first time. <br></td>
    </tr>
    <tr>
      <td>510</td>
      <td>Pippins Susie ACT - PIPPINS_CHEAT_ACT_COUNT</td>
      <td>number</td>
      <td>Number of Cheat ACTs used on Pippins. <br></td>
    </tr>
    <tr>
      <td>511</td>
      <td>Used Susie's ACT on Shuttah - USED_S_ACTION_ON_SHUTTAH</td>
      <td>bool</td>
      <td>Whether you've used S-Action during a Shuttah battle. Randomizes flavortext on repeat. <br></td>
    </tr>
    <tr>
      <td>512</td>
      <td>Used Ralsei's ACT on Shuttah - USED_R_ACTION_ON_SHUTTAH</td>
      <td>bool</td>
      <td>Whether you've used R-Action during a Shuttah battle. Reduces flavortext on repeat. <br></td>
    </tr>
    <tr>
      <td>513</td>
      <td>Shuttah Kris photo - SHUTTAH_KRIS_PIC</td>
      <td>bool</td>
      <td>Whether you took a photo of Kris during the Shuttah fight. Alters repeat dialogue. <br></td>
    </tr>
    <tr>
      <td>514</td>
      <td>Shuttah Susie photo - SHUTTAH_SUSIE_PIC</td>
      <td>bool</td>
      <td>Whether you took a photo of Susie during the Shuttah fight. Alters repeat dialogue. <br></td>
    </tr>
    <tr>
      <td>515</td>
      <td>Shuttah Ralsei photo - SHUTTAH_RALSEI_PIC</td>
      <td>bool</td>
      <td>Whether you took a photo of Ralsei during the Shuttah fight. Alters repeat dialogue. <br></td>
    </tr>
    <tr>
      <td>520</td>
      <td>Rudinns beaten up - RUDINN_VIOLENCES</td>
      <td>number</td>
      <td>The number of Rudinns you have beat up. Subtracted from flag 40 if you apologize. <br></td>
    </tr>
    <tr>
      <td>521</td>
      <td>Hathys beaten up - HATHY_VIOLENCES</td>
      <td>number</td>
      <td>The number of Hathys you have beat up. Subtracted from flag 40 if 2 or less and you apologize. <br></td>
    </tr>
    <tr>
      <td>522</td>
      <td>Violence - CLOVER_VIOLENCE</td>
      <td>bool</td>
      <td>Whether you beat up Clover the first time. You can't apologize. <br></td>
    </tr>
    <tr>
      <td>523</td>
      <td>Susie Rudinn whacks - RUDINN_HIT_BY_SUSIE_COUNT</td>
      <td>number</td>
      <td>Intended for Susie beating up Rudinns, but unset. See flag 43. <br></td>
    </tr>
    <tr>
      <td>524</td>
      <td>Susie Hathy whacks - HATHY_HIT_BY_SUSIE_COUNT</td>
      <td>number</td>
      <td>Intended for Susie beating up Hathys, but unset. See flag 43. <br></td>
    </tr>
    <tr>
      <td>525</td>
      <td>Werewire - FIRST_WEREWIRE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the first random Werewire encounter. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>526</td>
      <td>Tasque - FIRST_TASQUE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the first random Tasque encounter, the one that jumps out at you. Then it's reused for like Giga Queen deaths or something, which is a little broken. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>527</td>
      <td>Virovirokun - FIRST_VIROVIROKUN_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the first Virovirokun encounter, the one en route to AGREE2ALL. Also reused for Giga Queen stuff, doing Round 1 hitless causes this to be set to 1. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>528</td>
      <td>Smorgasbord - SECOND_SMORGASBORD_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Smorgasboard 2 encounter. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>529</td>
      <td>First fight - BERDLY_1_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the first Berdly battle. Used to determine if he breaks his arm. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>530</td>
      <td>Poppup - FIRST_POPPUP_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the first Poppup encounter, before you meet Noelle. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>531</td>
      <td>Virovirokun - TUTORIAL_VIROVIROKUN_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Virovirokun that tells Noelle how to battle. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>532</td>
      <td>Ambyu-Lance - AMBYU_LANCE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the first Ambyu-Lance encounter. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>533</td>
      <td>Ambyu-Lance + Virovirokun - ANTIVIRUS_VIROVIROKUN_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Ambyu-Lance + Virovirokun encounter. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>534</td>
      <td>2 Werewires - DOUBLE_WEREWIRE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the double Werewire encounter toward the middle of Cyber City. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>535</td>
      <td>2 Virovirokuns - ERASER_VIROVIROKUN_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the double Virovirokun encounter blocking the way to the Bounce Blade. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>536</td>
      <td>Maus - SINGLE_MAUS_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the single Maus encounter when rubbing the cheese. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>537</td>
      <td>Maus - CHEESE_MAUS_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of Maus encounters when bumping into cheese. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>538</td>
      <td>Poppup + Maus - POPPUP_MAUS_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Poppup and Maus encounter after the last mouse puzzle. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>539</td>
      <td>Tasque - GLOW_WRIST_TASQUE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the second random Tasque encounter, in the room with the Glow Wrist and checksmark. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>540</td>
      <td>Swatchling - FIRST_SWATCHLING_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the first Swatchling encounter when disrespecting the pottery. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>541</td>
      <td>Swatchlings - MULTIPLE_SWATCHLINGS_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the second Swatchling encounter, in the room full of vases. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>542</td>
      <td>Tasque Manager - TASQUE_MANAGER_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Tasque Manager battle. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>543</td>
      <td>Mauswheel - MAUSWHEEL_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Mauswheel battle. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>544</td>
      <td>Swatchlings - RUNNING_SWATCHLINGS_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Swatchlings running after/from vases on 2F. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>545</td>
      <td>Werewires - ACID_WEREWIRE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Werewires on the acid lake. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>546</td>
      <td>Rouxls - ROUXLS_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Rouxls/Thrash Machine battle. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>547</td>
      <td>Werewerewire - WEREWEREWIRE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Werewerewire encounter. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>548</td>
      <td>Queen - QUEEN_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the normal Queen battle. Used to determine if Berdly breaks his arm. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>549</td>
      <td>Spamton - SPAMTON_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the normal Spamton battle. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>550</td>
      <td>Second fight - BERDLY_2_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the second Berdly battle. Used to determine if he breaks his arm. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>551</td>
      <td>GIGA Queen - GIGA_QUEEN_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state saved for the GIGA Queen battle. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>552</td>
      <td>Scripted battles - SCRIPTED_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of various scripted encounters that are non-repeatable anyway (first Werewires and Sweet Cap'n Cakes). <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>553</td>
      <td>3 Ambyu-Lances - TRIPLE_AMBYU_LANCE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the triple Ambyu-Lance encounter on Snowgrave in the big car room. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>554</td>
      <td>Tasque + 2 Virovirokuns - TASQUE_VIROVIROKUN_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the double Virovirokun single Tasque encounter on Snowgrave. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>555</td>
      <td>Maice - SNOWGRAVE_MAICE_1_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the first Maice encounter on Snowgrave (no cheese is involved). <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>556</td>
      <td>Tasques - FLEEING_TASQUE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Snowgrave Tasques that run away from you. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>557</td>
      <td>Pipis encounter - DINING_HALL_PIPIS_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the last Pipis encounter you had in the dining hall. Well, it would. Pipis don't chase you. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>558</td>
      <td>Tasques + Swatchlings - RETURNING_TASQUE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Tasques and Swatchlings found when backtracking to Tasque Manager's room. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>559</td>
      <td>Poppups - TRASH_ZONE_POPPUP_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Poppups found when backtracking to the Trash Zone with Noelle. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>560</td>
      <td>Virovirokun - TRASH_ZONE_VIROVIROKUN_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Virovirokun found when backtracking to the Trash Zone on Snowgrave. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>561</td>
      <td>Werewire - TRASH_ZONE_WEREWIRE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Werewire found when backtracking to the Trash Zone on Snowgrave. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>562</td>
      <td>Ambyu-Lance - ROAD_AMBYU_LANCE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Ambyu-Lance found in the middle of the road on Snowgrave. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>563</td>
      <td>Tasque - ROAD_TASQUE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Tasque found in the middle of the road on Snowgrave. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>564</td>
      <td>Virovirokun - ROAD_VIROVIROKUN_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Virovirokun found in the middle of the road on Snowgrave. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>565</td>
      <td>Werewire - ROAD_WEREWIRE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Werewire found in the middle of the road on Snowgrave. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>566</td>
      <td>Maice - SNOWGRAVE_MAICE_2_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the second Maice encounter on Snowgrave. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>567</td>
      <td>2 Poppups - SNOWGRAVE_DOUBLE_POPPUP_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the double Poppup encounter that hides under a cone on Snowgrave. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>569</td>
      <td>Werewerewire - SNOWGRAVE_WEREWEREWIRE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>That's gotta be the most abbreviated one yet! Tracks the state of Werewerewire on Snowgrave, since it's found elsewhere. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>570</td>
      <td>Ambyu-Lance - ULTIMATE_HEAL_AMBYU_LANCE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Ambyu-Lance encounter where Susie demonstrates UltimateHeal. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>571</td>
      <td>Spamton NEO - SPAMTON_NEO_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>For some reason doesn't use "encounterflag" but tracks the state of Spamton NEO in case that's ever needed later. There are already like 2 flags for him anyway. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>572</td>
      <td>Poppup - VASE_POPPUP_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Poppup under the vase near where Susie and Ralsei leave you. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>580</td>
      <td>2 Shadowguys - BOARD_1_OASIS_SHADOWGUY_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Shadowguy encounter in the room on the left of the oasis in Board 1. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>581</td>
      <td>3 Shadowguys - BOARD_1_BLOCK_ROOM_SHADOWGUY_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Shadowguy encounter in the block-pushing room in Board 1. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>582</td>
      <td>2 Pippins - BOARD_2_SHRINE_PIPPINS_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Pippins encounter in the room on the left of the Kodakoda shrine in Board 2. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>583</td>
      <td>3 Pippins - BOARD_2_CONTROLLER_PIPPINS_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Pippins encounter that Susie runs into using Kris's controller in Board 2. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>584</td>
      <td>Shuttah - BOARD_2_SHUTTAH_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Shuttah boss battle in Board 2. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>585</td>
      <td>Rouxls + Weather Duo - ROUXLS_WEATHER_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Rouxls Kaard throuple battle. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>586</td>
      <td>Zapper + Shuttah - ZAPPER_SHUTTAH_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Zapper + Shuttah encounter later in TV world. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>587</td>
      <td>Watercooler - FIRST_WATERCOOLER_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Watercooler in the C-rank room. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>588</td>
      <td>Watercooler encounter - UNUSED_WATERCOOLER_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Never set, would have tracked the state of a Watercooler encounter in the unused room_dw_b3bs_watercooler. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>589</td>
      <td>Zapper - FIRST_ZAPPER_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Zapper in front of the suspicious door. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>590</td>
      <td>Shadowguy + Shuttah - FIRST_SHADOWGUY_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the first Shadow Guy + Shuttah encounter in TV World. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>591</td>
      <td>Ribbick - FIRST_RIBBICK_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the first Ribbick encounter in TV World. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>592</td>
      <td>Watercooler + Shadowguys - SECOND_WATERCOOLER_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Watercooler encounter in TV World, along with the Shadowguys that drop down in the Susiezilla room. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>593</td>
      <td>Ribbick - SECOND_RIBBICK_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the second Ribbick encounter in TV World. Can turn into disguised rabbicks. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>605</td>
      <td>Recruited Rudinn - RECRUITED_RUDINN</td>
      <td>bool</td>
      <td>Set at the start of Chapter 2. You NEED at least one recruit. <br></td>
    </tr>
    <tr>
      <td>606</td>
      <td>Recruited Hathy - RECRUITED_HATHY</td>
      <td>bool</td>
      <td>Set at the start of Chapter 2. <br></td>
    </tr>
    <tr>
      <td>611</td>
      <td>Recruited Ponman - RECRUITED_PONMAN</td>
      <td>bool</td>
      <td>Set at the start of Chapter 2. <br></td>
    </tr>
    <tr>
      <td>613</td>
      <td>Recruited Rabbick - RECRUITED_RABBICK</td>
      <td>bool</td>
      <td>Set at the start of Chapter 2. <br></td>
    </tr>
    <tr>
      <td>614</td>
      <td>Recruited Bloxer - RECRUITED_BLOXER</td>
      <td>bool</td>
      <td>Set at the start of Chapter 2. <br></td>
    </tr>
    <tr>
      <td>615</td>
      <td>Recruited Jigsawry - RECRUITED_JIGSAW</td>
      <td>bool</td>
      <td>Set at the start of Chapter 2. <br></td>
    </tr>
    <tr>
      <td>620</td>
      <td>Recruited JEVIL - RECRUITED_JEVIL</td>
      <td>bool</td>
      <td>JEVIL recruit flag with recruit info. <br></td>
    </tr>
    <tr>
      <td>622</td>
      <td>Recruited Rudinn Ranger - RECRUITED_RUDINN_RANGER</td>
      <td>bool</td>
      <td>Set at the start of Chapter 2. <br></td>
    </tr>
    <tr>
      <td>623</td>
      <td>Recruited Head Hathy - RECRUITED_HEAD_HATHY</td>
      <td>bool</td>
      <td>Set at the start of Chapter 2. <br></td>
    </tr>
    <tr>
      <td>630</td>
      <td>Recruited Ambyu-Lance - RECRUITED_AMBYU_LANCE</td>
      <td>bool</td>
      <td>Whether you recruited Ambyu-Lance. <br></td>
    </tr>
    <tr>
      <td>631</td>
      <td>Recruited Poppup - RECRUITED_POPPUP</td>
      <td>bool</td>
      <td>Whether you recruited Poppup. <br></td>
    </tr>
    <tr>
      <td>632</td>
      <td>Recruited Tasque - RECRUITED_TASQUE</td>
      <td>bool</td>
      <td>Whether you recruited Tasque. <br></td>
    </tr>
    <tr>
      <td>633</td>
      <td>Recruited Werewire - RECRUITED_WEREWIRE</td>
      <td>bool</td>
      <td>Whether you recruited Plugboy, by which I mean Werewire. <br></td>
    </tr>
    <tr>
      <td>634</td>
      <td>Recruited Maus - RECRUITED_MAUS</td>
      <td>bool</td>
      <td>Whether you recruited Maus. <br></td>
    </tr>
    <tr>
      <td>635</td>
      <td>Recruited Virovirokun - RECRUITED_VIROVIROKUN</td>
      <td>bool</td>
      <td>Whether you recruited Virovirokun. <br></td>
    </tr>
    <tr>
      <td>636</td>
      <td>Recruited Swatchling - RECRUITED_SWATCHLING</td>
      <td>bool</td>
      <td>Whether you recruited Swatchling. <br></td>
    </tr>
    <tr>
      <td>640</td>
      <td>Recruited Werewerewire - RECRUITED_WEREWEREWIRE</td>
      <td>bool</td>
      <td>Whether you recruited Werewerewire. It doesn't appear for the powers combined scene. <br></td>
    </tr>
    <tr>
      <td>642</td>
      <td>Recruited Tasque Manager - RECRUITED_TASQUE_MANAGER</td>
      <td>bool</td>
      <td>Whether you recruited Tasque Manager. <br></td>
    </tr>
    <tr>
      <td>644</td>
      <td>Recruited Mauswheel - RECRUITED_MAUSWHEEL</td>
      <td>bool</td>
      <td>Whether you recruited Mauswheel. <br></td>
    </tr>
    <tr>
      <td>654</td>
      <td>Recruited Shadowguy - RECRUITED_SHADOWGUY</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>655</td>
      <td>Recruited Shuttah - RECRUITED_SHUTTAH</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>656</td>
      <td>Recruited Zapper - RECRUITED_ZAPPER</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>657</td>
      <td>Recruited Ribbick - RECRUITED_RIBBICK</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>658</td>
      <td>Recruited Watercooler - RECRUITED_COOLER</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>659</td>
      <td>Recruited Pippins - RECRUITED_PIPPINS</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>660</td>
      <td>Recruited Elnina - RECRUITED_ELNINA</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>661</td>
      <td>Recruited Lanino - RECRUITED_LANINO</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>662</td>
      <td>Recruited Guei - RECRUITED_GUEI</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>663</td>
      <td>Recruited Balthizard - RECRUITED_BALTHIZARD</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>664</td>
      <td>Recruited Bibliox - RECRUITED_BIBLIOX</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>665</td>
      <td>Recruited Mizzle - RECRUITED_MIZZLE</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>666</td>
      <td>Recruited Wicabel - RECRUITED_WICABEL</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>667</td>
      <td>Recruited Winglade - RECRUITED_WINGLADE</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>668</td>
      <td>Recruited Organikk - RECRUITED_ORGANIKK</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>669</td>
      <td>Recruited Ms. Mizzle - RECRUITED_MISS_MIZZLE</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>670</td>
      <td>Recruited Floradinn - RECRUITED_FLORADINN</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>671</td>
      <td>Recruited Leafling - RECRUITED_LEAFLING</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>672</td>
      <td>Recruited Shi - RECRUITED_SHI</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>673</td>
      <td>Recruited Shinobeetle - RECRUITED_SHINOBEETLE</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>674</td>
      <td>Recruited KawKaw - RECRUITED_KAWKAW</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>675</td>
      <td>Recruited Sheary - RECRUITED_SHEARY</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>676</td>
      <td>Recruited Netskie - RECRUITED_NETSKIE</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>677</td>
      <td>Recruited Terakota - RECRUITED_TERAKOTA</td>
      <td>bool</td>
      <td>Recruit progress. <br></td>
    </tr>
    <tr>
      <td>700</td>
      <td>Completed the church sticker fight - COMPLETED_CHURCH_STICKER_FIGHT</td>
      <td>bool</td>
      <td>Viewed the cutscene of Kris and Susie placing stickers on each other at the church. Unaccessed as of chapter 4. <br></td>
    </tr>
    <tr>
      <td>701</td>
      <td>Completed the diner scene with Susie - COMPLETED_DINER_SCENE_WITH_SUSIE</td>
      <td>bool</td>
      <td>Finished the cutscene of the diner with Susie. <br></td>
    </tr>
    <tr>
      <td>702</td>
      <td>Drew Susie at the diner - DREW_SUSIE_AT_DINER</td>
      <td>bool</td>
      <td>Drew Susie during the diner cutscene. <br></td>
    </tr>
    <tr>
      <td>703</td>
      <td>Wrote in the diner window - WROTE_IN_DINER_CORNER</td>
      <td>bool</td>
      <td>Wrote something in the corner during the diner cutscene. Unaccessed as of chapter 4. <br></td>
    </tr>
    <tr>
      <td>704</td>
      <td>Activated the darkroom wall switch - ACTIVATED_UNUSED_DARKROOM_WALL_SWITCH</td>
      <td>bool</td>
      <td>Activated the switch in the unused room_dw_church_darkroom1_old. <br></td>
    </tr>
    <tr>
      <td>705</td>
      <td>Lit all candles - LIT_ALL_UNUSED_CANDLES</td>
      <td>bool</td>
      <td>Whether all the candles were lit in an unused candle lighting room. <br></td>
    </tr>
    <tr>
      <td>706</td>
      <td>Completed the Castle Town return scene - COMPLETED_CASTLE_TOWN_RETURN_SCENE_CH4</td>
      <td>bool</td>
      <td>Finished the cutscene of returning to Castle Town and greeting Ralsei at the start of chapter 4. <br></td>
    </tr>
    <tr>
      <td>707</td>
      <td>Had Noelle slap Kris - NOELLE_SLAPPED_KRIS_WEIRD_ROUTE</td>
      <td>bool</td>
      <td>Aborted the Weird Route late enough for Noelle to yell and slap you for your "prank". <br></td>
    </tr>
    <tr>
      <td>708</td>
      <td>Took Noelle's watch - KEPT_NOELLE_WATCH_AFTER_CH2</td>
      <td>bool</td>
      <td>Kept Noelle's watch in your equipment or inventory at the end of chapter 2. <br></td>
    </tr>
    <tr>
      <td>709</td>
      <td>Gate - HOLIDAY_GATE_STATE</td>
      <td>bool</td>
      <td>Opened the gate of the Holiday residence. There is a bug where it is set to -1 if you kill a Titan Spawn because the game thinks it's recruitable. <br></td>
    </tr>
    <tr>
      <td>710</td>
      <td>Ralsei's room - SAW_EMPTY_RALSEI_ROOM</td>
      <td>map</td>
      <td>Whether you saw the emptiness of Ralsei's room in Castle Town. <br>0 = Default state<br>1 = Susie ran off, followed by Ralsei<br>2 = Finished the Ralsei room cutscene<br></td>
    </tr>
    <tr>
      <td>711</td>
      <td>Heard Ralsei's plush dialogue - HEARD_RALSEI_PLUSH_DIALOGUE</td>
      <td>bool</td>
      <td>Listened to Ralsei after interacting with his Ralsei plush (obtained in chapter 2) in his room. <br></td>
    </tr>
    <tr>
      <td>712</td>
      <td>Lake sitting - LAKE_SITTING_SCENE_PROGRESS</td>
      <td>map</td>
      <td>Progress in cutscene after sitting down by the lake at the end of chapter 4. Interrupted by getting up. <br>0 = Default state<br>1 = Susie asks if you can hear a song<br>2 = Kris looks at Susie<br>3 = Susie asks if she got something on her face<br>4 = Given the option to say what's on your mind<br>5 = Susie gets up and says they should go<br></td>
    </tr>
    <tr>
      <td>713</td>
      <td>Beach festival reply - LAKE_CONVERSATION_RESPONSE</td>
      <td>map</td>
      <td>Which option you picked when asked to say what's on your mind or nothing at the lake. Unaccessed as of chapter 4. <br>0 = Default state<br>1 = Say what's on your mind<br>2 = Say nothing<br></td>
    </tr>
    <tr>
      <td>714</td>
      <td>Berdly call - BERDLY_PHONE_CALL_PROGRESS</td>
      <td>map</td>
      <td>Progress in the Berdly phone call at Noelle's house. <br>0 = Default state<br>1 = Picked up Noelle's phone<br>2 = Go with Berdly<br>3 = Sing the wrong number song<br></td>
    </tr>
    <tr>
      <td>715</td>
      <td>Asked Alvin about the shelter - ASKED_ALVIN_ABOUT_SHELTER</td>
      <td>bool</td>
      <td>Talked to Alvin and picked "Enter the shelter" after his sermon. <br></td>
    </tr>
    <tr>
      <td>716</td>
      <td>Praised Alvin's sermon - PRAISED_ALVINS_SERMON</td>
      <td>bool</td>
      <td>Talked to Alvin and picked the best option after his sermon. <br></td>
    </tr>
    <tr>
      <td>717</td>
      <td>Asked Alvin about Asgore - ASKED_ALVIN_ABOUT_ASGORE</td>
      <td>bool</td>
      <td>Talked to Alvin and picked "Asgore" after his sermon. <br></td>
    </tr>
    <tr>
      <td>718</td>
      <td>Monster Kid response - MONSTER_KID_CHURCH_RESPONSE</td>
      <td>map</td>
      <td>What you said to Monster Kid after Alvin's sermon. <br>0 = Default state<br>1 = Shelter<br>2 = Susie will not be tamed<br></td>
    </tr>
    <tr>
      <td>719</td>
      <td>Made Alphys's juice - MADE_ALPHYS_JUICE</td>
      <td>bool</td>
      <td>Successfully created Alphys' juice combo at church. <br></td>
    </tr>
    <tr>
      <td>720</td>
      <td>Alphys response - ALPHYS_JUICE_OUTCOME</td>
      <td>map</td>
      <td>Whether you gave Alphys her juice combo… or not. <br>0 = Default state<br>1 = Offer juice<br>2 = Drink juice in front of her<br></td>
    </tr>
    <tr>
      <td>722</td>
      <td>Shelter reason - ALPHYS_SHELTER_REASON</td>
      <td>map</td>
      <td>The reason you gave to Alphys for asking about the shelter. <br>0 = Default state<br>1 = Architectural history research<br>2 = Put hay inside new house for Susie<br></td>
    </tr>
    <tr>
      <td>723</td>
      <td>Undyne response - ALPHYS_UNDYNE_CHURCH_RESPONSE</td>
      <td>map</td>
      <td>Talked to Alphys about Undyne at church. An extra value is available if we gave her Undyne's chocolate in chapter 2. <br>0 = Default state<br>1 = Undyne / She gave you chocolates though<br>2 = It's because of me<br></td>
    </tr>
    <tr>
      <td>726</td>
      <td>Heard Noelle explain the Santas - HEARD_NOELLE_SANTA_EXPLANATION</td>
      <td>bool</td>
      <td>Whether Noelle has explained the Santas. <br></td>
    </tr>
    <tr>
      <td>727</td>
      <td>Heard Noelle's dead-Santa comment - HEARD_NOELLE_DEAD_SANTA_COMMENT</td>
      <td>bool</td>
      <td>Whether Noelle commented on Kris trying to "starve" the Santas. <br></td>
    </tr>
    <tr>
      <td>728</td>
      <td>Saw the treat-launcher scene - SAW_UNUSED_TREAT_LAUNCHER_SCENE</td>
      <td>bool</td>
      <td>Viewed the cutscene of Noelle showing off the unused holiday treat launcher. <br></td>
    </tr>
    <tr>
      <td>730</td>
      <td>Heard Noelle's cactus comment - HEARD_NOELLE_CACTUS_COMMENT</td>
      <td>bool</td>
      <td>Whether Noelle commented on the cactus being called Tsuntsun by Berdly. <br></td>
    </tr>
    <tr>
      <td>731</td>
      <td>Checked Noelle's browsing history - CHECKED_NOELLE_BROWSING_HISTORY</td>
      <td>bool</td>
      <td>Checked Noelle's browsing history with Susie. <br></td>
    </tr>
    <tr>
      <td>732</td>
      <td>Found Cat Petterz 4 - FOUND_CAT_PETTERZ_4</td>
      <td>bool</td>
      <td>Noticed Cat Petterz 4 on Noelle's computer. <br></td>
    </tr>
    <tr>
      <td>733</td>
      <td>Took Noelle's desk pencil - TOOK_NOELLE_DESK_PENCIL</td>
      <td>bool</td>
      <td>Took the pencil from Noelle's homework desk. <br></td>
    </tr>
    <tr>
      <td>734</td>
      <td>Completed Ralsei and Susie's festival talk - COMPLETED_RALSEI_SUSIE_FESTIVAL_TALK</td>
      <td>bool</td>
      <td>Whether you completed the talk between Susie and Ralsei prior to Tenna's introduction in Chapter 3. <br></td>
    </tr>
    <tr>
      <td>736</td>
      <td>Phone line - NOELLE_KITCHEN_PHONE_LINE</td>
      <td>map</td>
      <td>Tracks the current line in the spooky phone call to Kris in Noelle's kitchen. <br>0 = ... dark... fountain... next...<br>1 = ... Susie... must not get... guitar...<br>2 = ... need... soul...<br>3 = Without... soul... Kris... will...<br>4 = ... Susie... guitar... code... stop...<br>5 = ... police... sacrifice... next week...<br>6 = ... church... tonight...<br>7 = ... Kris... dark world... no soul... can't...<br>8 = ...... ...... ......<br></td>
    </tr>
    <tr>
      <td>737</td>
      <td>Soul capture - NOELLE_KITCHEN_SOUL_CAPTURE_PROGRESS</td>
      <td>map</td>
      <td>Tracks the progress in the cutscene of Kris catching the Soul in Noelle's kitchen. <br>0 = Default state<br>1 = Kris caught Soul in kitchen<br>2 = Kris put back Soul in closet<br></td>
    </tr>
    <tr>
      <td>738</td>
      <td>Piano song - NOELLE_KITCHEN_PIANO_SONG</td>
      <td>map</td>
      <td>Tracks the current piano song being played by Kris in Noelle's kitchen. <br>0 = Default state<br>1 = kris_piano_sevenfour<br>2 = kris_piano_quiz<br>3 = kris_piano_lancer_waltz<br>4 = kris_piano_rouxls<br>5 = kris_piano_waitingroom<br>6 = kris_piano_shop<br>7 = kris_piano_last_prophecy<br>8 = kris_piano_prophecy<br>9 = Kris played all songs (unused?)<br></td>
    </tr>
    <tr>
      <td>739</td>
      <td>Present 1 X position - NOELLE_PRESENT_1_X</td>
      <td>number</td>
      <td>X coordinate of the first present in Noelle's present room. <br></td>
    </tr>
    <tr>
      <td>740</td>
      <td>Present 2 X position - NOELLE_PRESENT_2_X</td>
      <td>number</td>
      <td>X coordinate of the second present in Noelle's present room. <br></td>
    </tr>
    <tr>
      <td>741</td>
      <td>Present 3 X position - NOELLE_PRESENT_3_X</td>
      <td>number</td>
      <td>X coordinate of the third present in Noelle's present room. <br></td>
    </tr>
    <tr>
      <td>742</td>
      <td>Mirror - NOELLE_BATHROOM_ASGORE_LINE</td>
      <td>map</td>
      <td>Tracks the current line in the Asgore cutscene in Noelle's bathroom. <br>0 = Default state<br>1 = Dum dee dum...<br>2 = Phew! Cleaning up sure works up an appetite.<br>3 = ... I wonder if the kitchen has any treats for me...<br>4 = ... No. Not now. I can't afford to take a break.<br>5 = Now, more than ever... I need to concentrate.<br>6 = ... to settle this once and for all.<br>7 = ... I've got to go look again.<br></td>
    </tr>
    <tr>
      <td>744</td>
      <td>Showed the family photo to Susie - SHOWED_FAMILY_PHOTO_TO_SUSIE</td>
      <td>bool</td>
      <td>Showed to Susie the old family photo on your fridge. <br></td>
    </tr>
    <tr>
      <td>745</td>
      <td>Showed Asriel's photo to Susie - SHOWED_ASRIEL_PHOTO_TO_SUSIE</td>
      <td>bool</td>
      <td>Showed to Susie the Asriel photo on your fridge. <br></td>
    </tr>
    <tr>
      <td>746</td>
      <td>Opened the dragon-book drawer for Susie - OPENED_DRAGON_BOOK_DRAWER_FOR_SUSIE</td>
      <td>bool</td>
      <td>Opened the drawer containing How To Draw Dragons in front of Susie. <br></td>
    </tr>
    <tr>
      <td>748</td>
      <td>Cleaned Kris's room stain - CLEANED_KRIS_ROOM_STAIN</td>
      <td>bool</td>
      <td>Cleaned up the stain with Susie in Kris's room. <br></td>
    </tr>
    <tr>
      <td>750</td>
      <td>Talked to Berdly at the Librarby - TALKED_TO_BERDLY_AT_LIBRARBY</td>
      <td>bool</td>
      <td>Talked to Berdly at the Librarby. <br></td>
    </tr>
    <tr>
      <td>751</td>
      <td>Discussed study plans - DISCUSSED_PLANS_WITH_BERDLY_AT_LIBRARBY</td>
      <td>bool</td>
      <td>Discussed plans with Berdly at the Librarby. <br></td>
    </tr>
    <tr>
      <td>752</td>
      <td>Introduced Susie - INTRODUCED_SUSIE_TO_RUDY_AFTER_CHURCH</td>
      <td>bool</td>
      <td>Brought Susie to see Rudy at the hospital after church, if we didn't see him at the end of chapter 2 (flag 316). <br></td>
    </tr>
    <tr>
      <td>753</td>
      <td>Brought Susie to Rudy after church - BROUGHT_SUSIE_TO_RUDY_AFTER_CHURCH</td>
      <td>bool</td>
      <td>Brought Susie to see Rudy at the hospital after church, if we did see him at the end of chapter 2 (flag 316). <br></td>
    </tr>
    <tr>
      <td>754</td>
      <td>Used Rudy's sink - USED_RUDY_SINK_CH4</td>
      <td>bool</td>
      <td>Interacted with Rudy's sink in chapter 4, after also doing it in chapter 1 (flag 278) and 2 (flag 461). <br></td>
    </tr>
    <tr>
      <td>755</td>
      <td>Visited Berdly in the hospital - VISITED_BERDLY_IN_HOSPITAL_CH4</td>
      <td>bool</td>
      <td>Visited Berdly's room at the hospital after church if his arm was injured in chapter 2. <br></td>
    </tr>
    <tr>
      <td>756</td>
      <td>Changed Berdly's hospital water bottle - CHANGED_BERDLY_HOSPITAL_WATER_BOTTLE</td>
      <td>bool</td>
      <td>Changed Berdly's water bottle at the hospital during the Weird Route. <br></td>
    </tr>
    <tr>
      <td>757</td>
      <td>Turned up Berdly's hospital heater - TURNED_UP_BERDLY_HOSPITAL_HEATER</td>
      <td>bool</td>
      <td>Turned up the space heater in Berdly's room at the hospital during the Weird Route. <br></td>
    </tr>
    <tr>
      <td>758</td>
      <td>Saw Susie's post-Berdly hallway scene - SAW_SUSIE_POST_BERDLY_VISIT_SCENE</td>
      <td>bool</td>
      <td>Viewed the cutscene of Susie talking to Kris after exiting Berdly's hospital room if his arm was injured in chapter 2. <br></td>
    </tr>
    <tr>
      <td>759</td>
      <td>Hallway visit state - SUSIE_BERDLY_HOSPITAL_WEIRD_ROUTE_PROGRESS</td>
      <td>map</td>
      <td>Tracks Susie talking before and after we enter Berdly's hospital room in the Weird Route. <br>0 = Default state<br>1 = Susie asked if Kris wants to go alone<br>2 = Susie talked to Kris after they come out<br></td>
    </tr>
    <tr>
      <td>760</td>
      <td>Talked to Catty in alley - TALKED_TO_CATTY_IN_ALLEY</td>
      <td>bool</td>
      <td>Talked to Catty in the alley. <br></td>
    </tr>
    <tr>
      <td>761</td>
      <td>Eavesdropped on bunny - EAVESDROPPED_BLUE_BUNNY</td>
      <td>bool</td>
      <td>Eavesdropped on Blue Bunny at the diner. <br></td>
    </tr>
    <tr>
      <td>762</td>
      <td>Talked to Bratty about Catty - TALKED_TO_BRATTY_ABOUT_CATTY</td>
      <td>bool</td>
      <td>Talked to Bratty about Catty at the diner. <br></td>
    </tr>
    <tr>
      <td>763</td>
      <td>Talked to Alphys about milk - TALKED_TO_ALPHYS_CH4</td>
      <td>bool</td>
      <td>Talked to Alphys in Hometown in chapter 4, if we already talked to her in chapter 1 (flag 269). <br></td>
    </tr>
    <tr>
      <td>764</td>
      <td>Asked Alphys to explain - ASKED_ALPHYS_TO_EXPLAIN_CH4</td>
      <td>bool</td>
      <td>Talked to Alphys in Hometown in chapter 4 and asked her to explain herself, if we didn't talk to her in chapter 1 (flag 269). <br></td>
    </tr>
    <tr>
      <td>765</td>
      <td>Saw Susie scare the door kid - SAW_SUSIE_SCARE_DOOR_KID_SCENE</td>
      <td>bool</td>
      <td>Viewed the cutscene of Susie scaring the kid behind one of the knockable doors. <br></td>
    </tr>
    <tr>
      <td>767</td>
      <td>Talked to Catti about Susie in Hometown - TALKED_TO_CATTI_ABOUT_SUSIE_IN_HOMETOWN</td>
      <td>bool</td>
      <td>Talked to Catti about Susie in Hometown. <br></td>
    </tr>
    <tr>
      <td>768</td>
      <td>Checked Gerson's grave with Susie - CHECKED_GERSON_GRAVE_WITH_SUSIE</td>
      <td>bool</td>
      <td>Interacted with Gerson's grave with Susie at the end of chapter 4. <br></td>
    </tr>
    <tr>
      <td>769</td>
      <td>Checked the shelter with Susie - CHECKED_SHELTER_WITH_SUSIE</td>
      <td>bool</td>
      <td>Interacted with the Shelter with Susie at the end of chapter 4. <br></td>
    </tr>
    <tr>
      <td>770</td>
      <td>Alphys's classroom - TRIED_TO_ENTER_SCHOOL_END_CH4</td>
      <td>bool</td>
      <td>Tried to enter the school at the end of chapter 4. <br></td>
    </tr>
    <tr>
      <td>771</td>
      <td>Beach scene - LAKE_CUTSCENE_PROGRESS_CH4</td>
      <td>map</td>
      <td>Tracks the progress of the lake cutscene with Susie in chapter 4. <br>0 = Default state<br>1 = Susie remarks our weird friend is busy today<br>2 = Normal NPC when coming back<br>3 = Viewed the skipping stones cutscene<br></td>
    </tr>
    <tr>
      <td>773</td>
      <td>Checked the lake table before the rain - CHECKED_LAKE_TABLE_BEFORE_RAIN</td>
      <td>bool</td>
      <td>Interacted with the table near the lake with Susie, before it started raining. <br></td>
    </tr>
    <tr>
      <td>774</td>
      <td>Checked the lake table after the rain - CHECKED_LAKE_TABLE_AFTER_RAIN</td>
      <td>bool</td>
      <td>Interacted with the table near the lake with Susie, after it started raining. <br></td>
    </tr>
    <tr>
      <td>775</td>
      <td>Checked Berdly's desk with the eggs - CHECKED_BERDLY_DESK_WITH_EGGS</td>
      <td>bool</td>
      <td>Interacted with Berdly's desk with the egg(s) on it in Alphys' class. <br></td>
    </tr>
    <tr>
      <td>776</td>
      <td>Asked burgerpants to continue - ASKED_BURGERPANTS_TO_CONTINUE</td>
      <td>bool</td>
      <td>Picked 'Hear more' when talking to Burgerpants. <br></td>
    </tr>
    <tr>
      <td>777</td>
      <td>Date progress - BURGERPANTS_DATE_PROGRESS</td>
      <td>map</td>
      <td>Tracks the progress of the Burgerpants date cutscene. <br>0 = Default state<br>1 = Burgerpants got cookies and left<br>2 = Talked to Nice Cream Guy<br></td>
    </tr>
    <tr>
      <td>778</td>
      <td>Face draw cutscene - TORIEL_BLUSHING</td>
      <td>bool</td>
      <td>Whether Toriel is blushing. Used for the end of chapter 4. <br></td>
    </tr>
    <tr>
      <td>779</td>
      <td>Mettaton response - TENNA_METTATON_GIFT_PROGRESS</td>
      <td>map</td>
      <td>Tracks the progress of giving Tenna to Mettaton. <br>0 = Default state<br>1 = Offered to give our TV<br>2 = Gave our TV<br></td>
    </tr>
    <tr>
      <td>780</td>
      <td>Brought Tenna to school - BROUGHT_TENNA_TO_SCHOOL</td>
      <td>bool</td>
      <td>Brought Tenna to school. <br></td>
    </tr>
    <tr>
      <td>782</td>
      <td>Used the Treat Catcher with Susie and Noelle - USED_TREAT_CATCHER_WITH_SUSIE_AND_NOELLE</td>
      <td>bool</td>
      <td>Interacted with the holiday treat catcher with Susie and Noelle at Noelle's house. <br></td>
    </tr>
    <tr>
      <td>783</td>
      <td>Ornament done - ORNAMENT_FINISHED_ROLLING</td>
      <td>bool</td>
      <td>Whether the unused ornament in Noelle's house has finished rolling after falling. <br></td>
    </tr>
    <tr>
      <td>784</td>
      <td>Fan running - NOELLE_FAN_ROTATING</td>
      <td>bool</td>
      <td>Whether the unused rotating fan in Noelle's house is rotating. <br></td>
    </tr>
    <tr>
      <td>785</td>
      <td>Fan frame - NOELLE_FAN_FRAME</td>
      <td>number</td>
      <td>The current frame of the unused rotating fan in Noelle's house. <br></td>
    </tr>
    <tr>
      <td>786</td>
      <td>Talked to Sans at the grill - TALKED_TO_SANS_AT_GRILL</td>
      <td>bool</td>
      <td>Talked to Sans in front of his grill in Hometown. <br></td>
    </tr>
    <tr>
      <td>787</td>
      <td>Piano approach - NOELLE_KITCHEN_PIANO_APPROACH_PROGRESS</td>
      <td>map</td>
      <td>Tracks the progress of the cutscene of Kris walking to the piano in Noelle's kitchen. <br>0 = Default state<br>1 = Entered kitchen again after getting caught<br>2 = Kris walks to the left<br>3 = Kris walks down<br>4 = Kris walks to the right<br></td>
    </tr>
    <tr>
      <td>788</td>
      <td>Saw Lancer's renovated room - SAW_LANCER_ROOM_RENOVATION_SCENE</td>
      <td>bool</td>
      <td>Viewed the cutscene about Lancer's room being renovated. <br></td>
    </tr>
    <tr>
      <td>789</td>
      <td>Talked to King about the Knight - TALKED_TO_KING_ABOUT_KNIGHT</td>
      <td>bool</td>
      <td>Talked to King about the Knight. <br></td>
    </tr>
    <tr>
      <td>790</td>
      <td>Saw Tenna entertain King - SAW_TENNA_ENTERTAIN_KING_SCENE</td>
      <td>bool</td>
      <td>Viewed the cutscene of Tenna entertaining King. <br></td>
    </tr>
    <tr>
      <td>791</td>
      <td>Saw Queen drinking - SAW_QUEEN_DRINKING_SCENE</td>
      <td>bool</td>
      <td>Viewed the cutscene of Queen drinking in front of the giant speakers. <br></td>
    </tr>
    <tr>
      <td>792</td>
      <td>Addison lineup - CASTLE_TOWN_ADDISON_LINEUP</td>
      <td>map</td>
      <td>Current lineup of the Addison booth in Castle Town. <br>0 = Lineup 1<br>1 = Lineup 2<br>2 = Lineup 3<br>3 = Lineup 4<br></td>
    </tr>
    <tr>
      <td>793</td>
      <td>Had Susie carry Lancer - SUSIE_CARRIED_LANCER</td>
      <td>bool</td>
      <td>Whether Susie carried Lancer on her back in Castle Town. <br></td>
    </tr>
    <tr>
      <td>794</td>
      <td>Rain effect state - RAIN_STATE</td>
      <td>map</td>
      <td>Activated when it's raining (mainly to control music and effects). <br>0 = Default state<br>1 = Chapter 4 ending (becomes state 2 after setting some parameters)<br>2 = Rain initialized (overrides other states)<br>3 = Used for certain room transitions (set back to 2 immediately if rain exists in the next room)<br></td>
    </tr>
    <tr>
      <td>795</td>
      <td>Legender prophecy seen - UNUSED_STAIRS_PROPHECY_COUNT</td>
      <td>map</td>
      <td>How many of the two prophecies were seen in the two unused room_dw_church_stairs_topleft and room_dw_church_stairs_topright. <br>0 = Default state<br>1 = Saw one prophecy<br>2 = Saw both prophecies<br></td>
    </tr>
    <tr>
      <td>797</td>
      <td>Checked the shelter panel - CHECKED_SHELTER_PANEL</td>
      <td>bool</td>
      <td>Checked the Shelter's panel. <br></td>
    </tr>
    <tr>
      <td>798</td>
      <td>Egg sign - SANS_SIGN_PROGRESS</td>
      <td>map</td>
      <td>Tracks the progress of the Sans sign shenanigans. <br>0 = Default state<br>1 = Talked to Sans before checking the sign<br>2 = Checked Open sign<br>3 = Talked to Sans when sign says Open<br>4 = Went away and came back<br>5 = Talked to Sans when sign says Clopen<br>6 = Went away and came back<br>7 = Talked to Sans when sign is Sans<br></td>
    </tr>
    <tr>
      <td>799</td>
      <td>Saw the Egg Man in the diner - SAW_EGG_MAN_IN_DINER</td>
      <td>bool</td>
      <td>Saw the Man in the diner, if you got the Egg in chapter 3. <br></td>
    </tr>
    <tr>
      <td>800</td>
      <td>Top-left seat recruit - CAFE_TOP_LEFT_RECRUIT</td>
      <td>map</td>
      <td>The recruit seated in the top-left of the Cafe. Defaults to Jigsawry. <br>1 = Invalid (1)<br>5 = Rudinn<br>6 = Hathy<br>11 = Ponman<br>13 = Rabbick<br>14 = Bloxer<br>15 = Jigsawry<br>20 = JEVIL<br>22 = Rudinn Ranger<br>23 = Head Hathy<br>30 = Ambyu-Lance<br>31 = Poppup<br>32 = Tasque<br>33 = Werewire<br>34 = Maus<br>35 = Virovirokun<br>36 = Swatchling<br>40 = Werewerewire<br>42 = Tasque Manager<br>44 = Mauswheel<br>54 = Shadowguy<br>55 = Shuttah<br>56 = Zapper<br>57 = Ribbick<br>58 = Watercooler<br>59 = Pippins<br>60 = Elnina<br>61 = Lanino<br>62 = Guei<br>63 = Balthizard<br>64 = Bibliox<br>65 = Mizzle<br>66 = Wicabel<br>67 = Winglade<br>68 = Organikk<br>69 = Ms. Mizzle<br>70 = Floradinn<br>71 = Leafling<br>72 = Shi<br>73 = Shinobeetle<br>74 = KawKaw<br>75 = Sheary<br>76 = Netskie<br>77 = Terakota<br></td>
    </tr>
    <tr>
      <td>801</td>
      <td>Top-right seat recruit - CAFE_TOP_RIGHT_RECRUIT</td>
      <td>map</td>
      <td>The recruit seated in the top-right of the Cafe. Defaults to Rudinn. <br>1 = Invalid (1)<br>5 = Rudinn<br>6 = Hathy<br>11 = Ponman<br>13 = Rabbick<br>14 = Bloxer<br>15 = Jigsawry<br>20 = JEVIL<br>22 = Rudinn Ranger<br>23 = Head Hathy<br>30 = Ambyu-Lance<br>31 = Poppup<br>32 = Tasque<br>33 = Werewire<br>34 = Maus<br>35 = Virovirokun<br>36 = Swatchling<br>40 = Werewerewire<br>42 = Tasque Manager<br>44 = Mauswheel<br>54 = Shadowguy<br>55 = Shuttah<br>56 = Zapper<br>57 = Ribbick<br>58 = Watercooler<br>59 = Pippins<br>60 = Elnina<br>61 = Lanino<br>62 = Guei<br>63 = Balthizard<br>64 = Bibliox<br>65 = Mizzle<br>66 = Wicabel<br>67 = Winglade<br>68 = Organikk<br>69 = Ms. Mizzle<br>70 = Floradinn<br>71 = Leafling<br>72 = Shi<br>73 = Shinobeetle<br>74 = KawKaw<br>75 = Sheary<br>76 = Netskie<br>77 = Terakota<br></td>
    </tr>
    <tr>
      <td>802</td>
      <td>Bottom-left seat recruit - CAFE_BOTTOM_LEFT_RECRUIT</td>
      <td>map</td>
      <td>The recruit seated in the bottom-left of the Cafe. Defaults to Hathy. <br>1 = Invalid (1)<br>5 = Rudinn<br>6 = Hathy<br>11 = Ponman<br>13 = Rabbick<br>14 = Bloxer<br>15 = Jigsawry<br>20 = JEVIL<br>22 = Rudinn Ranger<br>23 = Head Hathy<br>30 = Ambyu-Lance<br>31 = Poppup<br>32 = Tasque<br>33 = Werewire<br>34 = Maus<br>35 = Virovirokun<br>36 = Swatchling<br>40 = Werewerewire<br>42 = Tasque Manager<br>44 = Mauswheel<br>54 = Shadowguy<br>55 = Shuttah<br>56 = Zapper<br>57 = Ribbick<br>58 = Watercooler<br>59 = Pippins<br>60 = Elnina<br>61 = Lanino<br>62 = Guei<br>63 = Balthizard<br>64 = Bibliox<br>65 = Mizzle<br>66 = Wicabel<br>67 = Winglade<br>68 = Organikk<br>69 = Ms. Mizzle<br>70 = Floradinn<br>71 = Leafling<br>72 = Shi<br>73 = Shinobeetle<br>74 = KawKaw<br>75 = Sheary<br>76 = Netskie<br>77 = Terakota<br></td>
    </tr>
    <tr>
      <td>803</td>
      <td>Bottom-right seat recruit - CAFE_BOTTOM_RIGHT_RECRUIT</td>
      <td>map</td>
      <td>The recruit seated in the bottom-right of the Cafe. Defaults to Rudinn. <br>1 = Invalid (1)<br>5 = Rudinn<br>6 = Hathy<br>11 = Ponman<br>13 = Rabbick<br>14 = Bloxer<br>15 = Jigsawry<br>20 = JEVIL<br>22 = Rudinn Ranger<br>23 = Head Hathy<br>30 = Ambyu-Lance<br>31 = Poppup<br>32 = Tasque<br>33 = Werewire<br>34 = Maus<br>35 = Virovirokun<br>36 = Swatchling<br>40 = Werewerewire<br>42 = Tasque Manager<br>44 = Mauswheel<br>54 = Shadowguy<br>55 = Shuttah<br>56 = Zapper<br>57 = Ribbick<br>58 = Watercooler<br>59 = Pippins<br>60 = Elnina<br>61 = Lanino<br>62 = Guei<br>63 = Balthizard<br>64 = Bibliox<br>65 = Mizzle<br>66 = Wicabel<br>67 = Winglade<br>68 = Organikk<br>69 = Ms. Mizzle<br>70 = Floradinn<br>71 = Leafling<br>72 = Shi<br>73 = Shinobeetle<br>74 = KawKaw<br>75 = Sheary<br>76 = Netskie<br>77 = Terakota<br></td>
    </tr>
    <tr>
      <td>810</td>
      <td>Completed the grazing challenge - COMPLETED_GRAZING</td>
      <td>bool</td>
      <td>Whether you beat the grazing challenge in the Party Dojo. <br></td>
    </tr>
    <tr>
      <td>811</td>
      <td>Completed the Clover dojo battle - COMPLETED_DOJO_CLOVER</td>
      <td>bool</td>
      <td>Whether you beat Clover's rematch in the Party Dojo. <br></td>
    </tr>
    <tr>
      <td>812</td>
      <td>Completed Tasque Manager Says - COMPLETED_TASQUE_MANAGER_SAYS</td>
      <td>bool</td>
      <td>Whether you beat the "Tasque Manager Says" challenge in the Party Dojo. <br></td>
    </tr>
    <tr>
      <td>813</td>
      <td>Completed All Stars - COMPLETED_ALLSTARS</td>
      <td>bool</td>
      <td>Whether you beat the Ch2 All Stars challenge in the Party Dojo. <br></td>
    </tr>
    <tr>
      <td>814</td>
      <td>Completed Joe's dojo battle - COMPLETED_JOE</td>
      <td>bool</td>
      <td>Whether you defeated Jigsaw Joe in the Party Dojo and took his life savings. <br></td>
    </tr>
    <tr>
      <td>815</td>
      <td>Lanino and Elnina - WEATHER_DUO_DOJO_OUTCOME</td>
      <td>map</td>
      <td>Whether you defeated Lanino & Elnina in the chapter 4 Party/Love Dojo. <br>0 = Default state<br>2 = Won<br></td>
    </tr>
    <tr>
      <td>831</td>
      <td>Heard Toriel's post-church invitation - HEARD_TORIEL_POST_CHURCH_INVITATION</td>
      <td>bool</td>
      <td>Viewed the cutscene of Toriel telling us to come by the church if we need anything. <br></td>
    </tr>
    <tr>
      <td>832</td>
      <td>Took Asriel's money - TOOK_ASRIEL_DRAWER_MONEY_CH4</td>
      <td>bool</td>
      <td>Whether you took five bucks from Asriel's drawer in chapter 4. <br></td>
    </tr>
    <tr>
      <td>833</td>
      <td>Payment refused - DINER_PAYMENT_REFUSED</td>
      <td>bool</td>
      <td>Tried to get diner while not having the money for it. <br></td>
    </tr>
    <tr>
      <td>834</td>
      <td>Splatted next to Ralsei - SPLATTED_NEXT_TO_RALSEI</td>
      <td>bool</td>
      <td>Showed compassion to Ralsei by splatting next to him in the church Dark World. <br></td>
    </tr>
    <tr>
      <td>835</td>
      <td>Checked the First Sanctuary prophecy save point - CHECKED_FIRST_SANCTUARY_PROPHECY_SAVE_POINT</td>
      <td>bool</td>
      <td>Interacted with the save point under the prophecy panel at the start of the First Sanctuary. <br></td>
    </tr>
    <tr>
      <td>836</td>
      <td>Talked to Gerson in his study - TALKED_TO_GERSON_IN_STUDY</td>
      <td>bool</td>
      <td>Talked to Gerson once he's installed in his study. <br></td>
    </tr>
    <tr>
      <td>837</td>
      <td>Asked Gerson about his work before Jackenstein - ASKED_GERSON_ABOUT_HIS_WORK_BEFORE_JACKENSTEIN</td>
      <td>bool</td>
      <td>Asked Gerson in his study what he's doing, before healing Jackenstein. <br></td>
    </tr>
    <tr>
      <td>838</td>
      <td>Asked Gerson about the Knight before Jackenstein - ASKED_GERSON_ABOUT_KNIGHT_BEFORE_JACKENSTEIN</td>
      <td>bool</td>
      <td>Asked Gerson in his study about the Knight, before healing Jackenstein. <br></td>
    </tr>
    <tr>
      <td>841</td>
      <td>Study elixir state - UNUSED_HIDE_STUDY_ELIXIR</td>
      <td>map</td>
      <td>If activated, hides the elixir on the table of Gerson's study. Never set. <br>0 = Default state<br>2 = Hide elixir<br></td>
    </tr>
    <tr>
      <td>844</td>
      <td>Wall notes - SUSIE_COPIED_WALL_NOTES</td>
      <td>bool</td>
      <td>Viewed the cutscene of Susie talking to Gerson and writing down the music notes on the wall. <br></td>
    </tr>
    <tr>
      <td>845</td>
      <td>Knight daydream rest - THOUGHT_ABOUT_KNIGHT</td>
      <td>bool</td>
      <td>Viewed the cutscene of Kris thinking about the Knight. Unaccessed as of chapter 4. <br></td>
    </tr>
    <tr>
      <td>846</td>
      <td>Drip vision rest - THOUGHT_ABOUT_NOELLE_WEIRD_ROUTE</td>
      <td>bool</td>
      <td>Viewed the cutscene of Kris thinking about Noelle in the Weird Route. Unaccessed as of chapter 4. <br></td>
    </tr>
    <tr>
      <td>847</td>
      <td>Sheet music - STUDY_SHEET_MUSIC_PROGRESS</td>
      <td>map</td>
      <td>Tracks the progress of the cutscene of Kris playing the organ/piano and opening the central door in Gerson's study. <br>0 = Default state<br>1 = Used sheet music<br>2 = Kris played piano<br>3 = Unused (relies on unused flag 848)<br></td>
    </tr>
    <tr>
      <td>848</td>
      <td>Organ shadow puzzle - UNUSED_ORGAN_FLAG</td>
      <td>number</td>
      <td>Set by unreachable code, might be related to a cut player-only solve. <br></td>
    </tr>
    <tr>
      <td>849</td>
      <td>Saw Jackenstein's True face - SAW_JACKENSTEIN_TRUE_FACE</td>
      <td>bool</td>
      <td>Saw Jackenstein's True face after defeating him. Unaccessed as of chapter 4. <br></td>
    </tr>
    <tr>
      <td>850</td>
      <td>Sheet music hunt - JACKENSTEIN_CUTSCENE_PROGRESS</td>
      <td>map</td>
      <td>Tracks the progress of the Jackenstein cutscenes. <br>0 = Default state<br>1 = Found both sets of four tones<br>2 = Solved piano puzzle<br>3 = Fell into THE DARK ZONE<br>4 = Jackenstein hit chandelier<br>5 = Susie healed Jackenstein<br>6 = Susie offered Kris to heal again<br>0.5 = Found one set of four tones<br></td>
    </tr>
    <tr>
      <td>851</td>
      <td>Tall bookcase - GERSON_CUTSCENE_PROGRESS</td>
      <td>map</td>
      <td>Tracks the progress of the Gerson cutscenes. <br>0 = Default state<br>1 = Solved secret piano puzzle<br>2 = Fought Gerson<br>3 = Viewed post-battle cutscene<br></td>
    </tr>
    <tr>
      <td>852</td>
      <td>Defeated - DEFEATED_HAMMER_OF_JUSTICE</td>
      <td>bool</td>
      <td>Whether you defeated the Hammer of Justice. <br></td>
    </tr>
    <tr>
      <td>853</td>
      <td>Attempts - HAMMER_OF_JUSTICE_ATTEMPT_COUNT</td>
      <td>number</td>
      <td>Number of times you fought the Hammer of Justice. <br></td>
    </tr>
    <tr>
      <td>854</td>
      <td>Ralsei room apology - RALSEI_DESIRES_RESPONSE</td>
      <td>map</td>
      <td>What you answered to Ralsei asking you if a Darkner should be starting to develop his own desires. Unaccessed as of chapter 4. <br>0 = Default state<br>1 = Please be yourself<br>2 = Of course not<br></td>
    </tr>
    <tr>
      <td>855</td>
      <td>Talked to Seam about the Addisons - TALKED_TO_SEAM_ABOUT_ADDISONS</td>
      <td>bool</td>
      <td>Talked to Seam about taking everything from the Addisons to scare them. <br></td>
    </tr>
    <tr>
      <td>856</td>
      <td>Shadow Crystal - GAVE_KNIGHT_SHADOW_CRYSTAL_TO_SEAM</td>
      <td>bool</td>
      <td>Whether you gave Seam the Knight's Shadow Crystal. <br></td>
    </tr>
    <tr>
      <td>862</td>
      <td>Talked to Rudy about Asgore - TALKED_TO_RUDY_ABOUT_ASGORE</td>
      <td>bool</td>
      <td>Talked to Rudy about Asgore at church. <br></td>
    </tr>
    <tr>
      <td>863</td>
      <td>Got Power Band - OBTAINED_SIDE_CLIMB_POWER_BAND</td>
      <td>bool</td>
      <td>Got the Power Band from the chest in the room with the Mizzle on top. <br></td>
    </tr>
    <tr>
      <td>864</td>
      <td>Stole the ladder for Ralsei - STOLE_LADDER_FOR_RALSEI</td>
      <td>bool</td>
      <td>Stole the ladder in the bookshelf puzzle room to decorate Ralsei's room. <br></td>
    </tr>
    <tr>
      <td>865</td>
      <td>Stole the cushion for Ralsei - STOLE_PILLOW_FOR_RALSEI</td>
      <td>bool</td>
      <td>Stole the pillow in the right piano piece room to decorate Ralsei's room. <br></td>
    </tr>
    <tr>
      <td>866</td>
      <td>Told Ralsei to sit - TOLD_RALSEI_TO_SIT</td>
      <td>bool</td>
      <td>Told Ralsei to park his butt. <br></td>
    </tr>
    <tr>
      <td>867</td>
      <td>Talked to the fire extinguisher - TALKED_TO_FIRE_EXTINGUISHER</td>
      <td>bool</td>
      <td>Talked to the most important Darkner. <br></td>
    </tr>
    <tr>
      <td>868</td>
      <td>Had Gerson recruit the Gueis - GERSON_RECRUITED_GUEIS</td>
      <td>bool</td>
      <td>Whether Gerson recruited the Gueis. <br></td>
    </tr>
    <tr>
      <td>869</td>
      <td>Solved the introductory piano puzzle - SOLVED_INTRO_PIANO_PUZZLE</td>
      <td>bool</td>
      <td>Solved the first piano puzzle. <br></td>
    </tr>
    <tr>
      <td>871</td>
      <td>Opened the dark-maze chest - OPENED_DARK_MAZE_CHEST</td>
      <td>bool</td>
      <td>Opened the empty chest in the dark maze room. <br></td>
    </tr>
    <tr>
      <td>872</td>
      <td>Darker Candy bowl - DARKER_CANDY_BOWL_STATE</td>
      <td>map</td>
      <td>Tracks what you did with the Darker Candy bowl. <br>0 = Default state<br>1 = Took one candy<br>3 = Spilled the bowl<br></td>
    </tr>
    <tr>
      <td>873</td>
      <td>Locked door - CHECKED_LOCKED_CHURCH_DOOR</td>
      <td>bool</td>
      <td>Interacted with the locked church door before Susie got an idea. <br></td>
    </tr>
    <tr>
      <td>874</td>
      <td>Triggered Gerson's silhouette - TRIGGERED_GERSON_SILHOUETTE</td>
      <td>bool</td>
      <td>Triggered the silhouette of Gerson walking away in the intro dark maze room. <br></td>
    </tr>
    <tr>
      <td>875</td>
      <td>Ralsei response - RALSEI_SMILE_RESPONSE</td>
      <td>map</td>
      <td>What you told Ralsei after he told you he was smiling. <br>0 = Default state<br>1 = It's okay not to smile<br>2 = Good. Keep smiling<br></td>
    </tr>
    <tr>
      <td>876</td>
      <td>Blue shelf X - BOOKSHELF_PUZZLE_SHELF_1_X</td>
      <td>number</td>
      <td>X coordinate of the first shelf in the bookshelf puzzle room. <br></td>
    </tr>
    <tr>
      <td>877</td>
      <td>Blue shelf Y - BOOKSHELF_PUZZLE_SHELF_1_Y</td>
      <td>number</td>
      <td>Y coordinate of the first shelf in the bookshelf puzzle room. <br></td>
    </tr>
    <tr>
      <td>878</td>
      <td>Red shelf X - BOOKSHELF_PUZZLE_SHELF_2_X</td>
      <td>number</td>
      <td>X coordinate of the second shelf in the bookshelf puzzle room. <br></td>
    </tr>
    <tr>
      <td>879</td>
      <td>Red shelf Y - BOOKSHELF_PUZZLE_SHELF_2_Y</td>
      <td>number</td>
      <td>Y coordinate of the second shelf in the bookshelf puzzle room. <br></td>
    </tr>
    <tr>
      <td>880</td>
      <td>Green shelf X - BOOKSHELF_PUZZLE_SHELF_3_X</td>
      <td>number</td>
      <td>X coordinate of the third shelf in the bookshelf puzzle room. <br></td>
    </tr>
    <tr>
      <td>881</td>
      <td>Green shelf Y - BOOKSHELF_PUZZLE_SHELF_3_Y</td>
      <td>number</td>
      <td>Y coordinate of the third shelf in the bookshelf puzzle room. <br></td>
    </tr>
    <tr>
      <td>882</td>
      <td>Shelf 1 X - RIGHT_PIANO_PIECE_SHELF_1_X</td>
      <td>number</td>
      <td>X coordinate of the first shelf in the right piano piece room. <br></td>
    </tr>
    <tr>
      <td>883</td>
      <td>Shelf 1 Y - RIGHT_PIANO_PIECE_SHELF_1_Y</td>
      <td>number</td>
      <td>Y coordinate of the first shelf in the right piano piece room. <br></td>
    </tr>
    <tr>
      <td>884</td>
      <td>Shelf 2 X - RIGHT_PIANO_PIECE_SHELF_2_X</td>
      <td>number</td>
      <td>X coordinate of the second shelf in the right piano piece room. <br></td>
    </tr>
    <tr>
      <td>885</td>
      <td>Shelf 2 Y - RIGHT_PIANO_PIECE_SHELF_2_Y</td>
      <td>number</td>
      <td>Y coordinate of the second shelf in the right piano piece room. <br></td>
    </tr>
    <tr>
      <td>886</td>
      <td>Right melody - PIANO_PUZZLE_RIGHT_HINT_STATE</td>
      <td>map</td>
      <td>Revealed the right piano hint for the piano puzzle. <br>0 = Default state<br>1 = Revealed hint<br>-1 = Solved piano puzzle<br></td>
    </tr>
    <tr>
      <td>887</td>
      <td>Left hint - INTRO_PIANO_LEFT_HINT_REVEALED</td>
      <td>bool</td>
      <td>Revealed the left piano hint in the intro piano room. <br></td>
    </tr>
    <tr>
      <td>888</td>
      <td>Right hint - INTRO_PIANO_RIGHT_HINT_REVEALED</td>
      <td>bool</td>
      <td>Revealed the right piano hint in the intro piano room. <br></td>
    </tr>
    <tr>
      <td>889</td>
      <td>Bottom hint - DARK_MAZE_BOTTOM_HINT_REVEALED</td>
      <td>bool</td>
      <td>Revealed the bottom piano hint in the dark maze room. <br></td>
    </tr>
    <tr>
      <td>890</td>
      <td>Top hint - DARK_MAZE_TOP_HINT_REVEALED</td>
      <td>bool</td>
      <td>Revealed the top piano hint in the dark maze room. <br></td>
    </tr>
    <tr>
      <td>891</td>
      <td>Left melody - PIANO_PUZZLE_LEFT_HINT_STATE</td>
      <td>map</td>
      <td>Revealed the left piano hint for the piano puzzle. <br>0 = Default state<br>1 = Revealed hint<br>-1 = Solved piano puzzle<br></td>
    </tr>
    <tr>
      <td>892</td>
      <td>Solved - SOLVED_PIANO_PUZZLE</td>
      <td>bool</td>
      <td>Solved the piano puzzle before Jackenstein. <br></td>
    </tr>
    <tr>
      <td>893</td>
      <td>No-hint attempts - PIANO_PUZZLE_WITHOUT_HINT_ATTEMPTS</td>
      <td>map</td>
      <td>Tried to solve the piano puzzle without hint. <br>0 = Default state<br>1 = Interacted with piano once<br>1.1 = Interacted with piano more than once<br></td>
    </tr>
    <tr>
      <td>894</td>
      <td>Opened the left piano-piece chest - OPENED_LEFT_PIANO_PIECE_CHEST</td>
      <td>bool</td>
      <td>Got the Scarlixir from the chest in the left piano piece room. <br></td>
    </tr>
    <tr>
      <td>895</td>
      <td>Susie conversation - SUSIE_BASEMENT_DIALOGUE_LINE</td>
      <td>map</td>
      <td>Tracks the current line of Susie's dialogue alone in Noelle's basement during the Weird Route. <br>0 = Default state<br>1 = ... Damn, I've moved everything but I can't find anything...<br>2 = ... wonder how Kris's search is going.<br>3 = ... nothing to do but keep looking, I guess.<br></td>
    </tr>
    <tr>
      <td>897</td>
      <td>Incomplete music dialogue - UNUSED_PIANO_HINT_PREVENTION_FLAG</td>
      <td>bool</td>
      <td>Flag never set, but would have prevented use of the piano after getting one of the two hints. <br></td>
    </tr>
    <tr>
      <td>898</td>
      <td>Donation - MONEY_FOUNTAIN_DONATION</td>
      <td>number</td>
      <td>The amount of money you donated to the money fountain. <br></td>
    </tr>
    <tr>
      <td>899</td>
      <td>Holy Watercooler - HOLY_WATERCOOLER_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Holywatercooler encounter. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>900</td>
      <td>Head - VESSEL_HEAD</td>
      <td>map</td>
      <td>The head of your vessel. <br>0 = Bald<br>1 = Kris-like<br>2 = Left lock<br>3 = Middle part<br>4 = Thick hair<br>5 = Loose<br>6 = Balding line<br>7 = Refined<br></td>
    </tr>
    <tr>
      <td>901</td>
      <td>Body - VESSEL_BODY</td>
      <td>map</td>
      <td>The body of your vessel. <br>0 = Long sleeves<br>1 = Short sleeves<br>2 = Baggy sleeves<br>3 = Baggier sleeves<br>4 = Zipper<br>5 = Buttons<br></td>
    </tr>
    <tr>
      <td>902</td>
      <td>Legs - VESSEL_LEGS</td>
      <td>map</td>
      <td>The legs of your vessel. <br>0 = Wider on right<br>1 = Wider on right<br>2 = Wider on right<br>3 = Wider on right<br>4 = Wider on left<br></td>
    </tr>
    <tr>
      <td>903</td>
      <td>What is its favorite food? - VESSEL_FOOD</td>
      <td>map</td>
      <td>Your vessel's favorite food. <br>0 = Sweet<br>1 = Soft<br>2 = Sour<br>3 = Salty<br>4 = Pain<br>5 = Cold<br></td>
    </tr>
    <tr>
      <td>904</td>
      <td>Your favorite blood type? - VESSEL_BLOOD</td>
      <td>map</td>
      <td>Your favorite blood type. <br>0 = A<br>1 = AB<br>2 = B<br>3 = C<br>4 = D<br></td>
    </tr>
    <tr>
      <td>905</td>
      <td>What color does it like most? - VESSEL_COLOR</td>
      <td>map</td>
      <td>Your vessel's favorite color. <br>0 = Red<br>1 = Blue<br>2 = Green<br>3 = Cyan<br></td>
    </tr>
    <tr>
      <td>906</td>
      <td>How do you feel about your creation? (It will not hear.) - VESSEL_FEELING</td>
      <td>map</td>
      <td>How you feel about your vessel. <br>0 = Love<br>1 = Hope<br>2 = Disgust<br>3 = Fear<br></td>
    </tr>
    <tr>
      <td>907</td>
      <td>Have you answered honestly? - VESSEL_HONEST</td>
      <td>bool</td>
      <td>Were you honest about your vessel choices? <br></td>
    </tr>
    <tr>
      <td>908</td>
      <td>You acknowledge the possibility of pain and seizure. - VESSEL_SEIZURE</td>
      <td>bool</td>
      <td>Do you acknowledge the possibility of pain and seizure? <br></td>
    </tr>
    <tr>
      <td>909</td>
      <td>Please give it a gift - VESSEL_GIFT</td>
      <td>map</td>
      <td>The gift you give your vessel. Stored in reverse order. <br>0 = Mind<br>1 = Kindness<br>-3 = Voice<br>-2 = Bravery<br>-1 = Ambition<br></td>
    </tr>
    <tr>
      <td>910</td>
      <td>Room progress - EGG_ROOM_PROGRESS_CH1</td>
      <td>map</td>
      <td>Your progress to finding... him. <br>0 = Default state<br>1 = Entered room<br>2 = Interacted with man<br></td>
    </tr>
    <tr>
      <td>911</td>
      <td>Got the egg - OBTAINED_EGG_CH1</td>
      <td>bool</td>
      <td>Set when entering Chapter 2 if you had or deposited the Chapter 1 egg, but not if you dropped it. Maybe. It checks the key item. <br></td>
    </tr>
    <tr>
      <td>912</td>
      <td>Language - LANGUAGE_NAME</td>
      <td>map</td>
      <td>Language your name was entered in, used to display the correct font even if you change the game language later. <br>0 = English<br>1 = Japanese<br></td>
    </tr>
    <tr>
      <td>913</td>
      <td>Saw man in car - INTERACTED_WITH_MAN_CAR</td>
      <td>bool</td>
      <td>Whether you saw the man wave at you from his car, if flag 910 up there was 2 (even if you refused the offer). <br></td>
    </tr>
    <tr>
      <td>914</td>
      <td>Starting chapter - STARTING_CHAPTER</td>
      <td>number</td>
      <td>The chapter you started your current save file on, is 0 if the file was created on the current chapter. <br></td>
    </tr>
    <tr>
      <td>915</td>
      <td>Progress - SNOWGRAVE_ROUTE_PROGRESS</td>
      <td>map</td>
      <td>Your progress on the Snowgrave Route. This is a big one. <br>0 = Default state<br>1 = Froze tutor Virovirokun<br>2 = Ready for Freeze Ring<br>3 = Got Freeze Ring<br>4 = Passed forcefield<br>5 = Froze mouse puzzle<br>6 = SnowGrave.<br>7 = Entered mansion<br>8 = Rouxls's condition explained<br>9 = Did not see Suselle scene<br>19 = Seen Noelle with Rudy<br>20 = Creeped Noelle out<br>1.5 = Froze Trash Zone enemies<br>1.75 = Froze roadway enemies<br></td>
    </tr>
    <tr>
      <td>916</td>
      <td>Failed - SNOWGRAVE_FAIL</td>
      <td>bool</td>
      <td>Whether you failed the Snowgrave Route at any point, by any action. Reverts practically every effect of the route. <br></td>
    </tr>
    <tr>
      <td>917</td>
      <td>Room progress - EGG_ROOM_PROGRESS_CH2</td>
      <td>map</td>
      <td>Your progress to finding him. Again. <br>0 = Default state<br>1 = Killed by dog<br>2 = Entered egg room<br>3 = Interacted with man<br></td>
    </tr>
    <tr>
      <td>918</td>
      <td>Got the egg - OBTAINED_EGG_CH2</td>
      <td>bool</td>
      <td>Whether you got the Chapter 2 egg, for Temmie's collection. <br></td>
    </tr>
    <tr>
      <td>919</td>
      <td>Times Noelle Leveled - NOELLE_LEVEL_UP_COUNT</td>
      <td>number</td>
      <td>Like flag 65 but for Noelle in particular. Unaccessed. <br></td>
    </tr>
    <tr>
      <td>920</td>
      <td>Got the moss - OBTAINED_MOSS_CH2</td>
      <td>bool</td>
      <td>Whether you got the Moss in Chapter 2 and the Moss Finder title. <br></td>
    </tr>
    <tr>
      <td>921</td>
      <td>Ate moss with Noelle - ATE_MOSS_WITH_NOELLE</td>
      <td>bool</td>
      <td>Whether Noelle was with you when you found the Moss, earning the Moss Neutral title. <br></td>
    </tr>
    <tr>
      <td>922</td>
      <td>Ate moss with Susie - ATE_MOSS_WITH_SUSIE</td>
      <td>bool</td>
      <td>Whether Susie was with you when you found the Moss, earning the Moss Enjoyer title. <br></td>
    </tr>
    <tr>
      <td>923</td>
      <td>Forgot Ring - FAILED_SNOWGRAVE_WITHOUT_THORN_RING</td>
      <td>bool</td>
      <td>Whether you failed the Snowgrave route because of not having the Thorn Ring at Berdly. Unaccessed. <br></td>
    </tr>
    <tr>
      <td>924</td>
      <td>Snowgrave Attempts - SNOWGRAVE_KILL_COMMAND_COUNT</td>
      <td>number</td>
      <td>The number of times you told Noelle to KILL HIM, KILL HIM NOW. (0-4) <br></td>
    </tr>
    <tr>
      <td>925</td>
      <td>IceShock uses - ICESHOCKS</td>
      <td>number</td>
      <td>The number of IceShocks Noelle has used, finishing or not. Each increases her Coldness by 7. <br></td>
    </tr>
    <tr>
      <td>926</td>
      <td>Iceshocked Encounters - ICESHOCKED_ENCOUNTERS</td>
      <td>number</td>
      <td>The number of encounters defeated with IceShock. Unaccessed. <br></td>
    </tr>
    <tr>
      <td>928</td>
      <td>Creepy Steps - CREEPY_STEPS</td>
      <td>number</td>
      <td>The number of steps you take toward Noelle (0-3) after the hospital scene on Snowgrave. Yeah, that's a thing. <br></td>
    </tr>
    <tr>
      <td>930</td>
      <td>Got the egg - OBTAINED_EGG_CH3</td>
      <td>bool</td>
      <td>Whether you got the Chapter 3 egg. <br></td>
    </tr>
    <tr>
      <td>931</td>
      <td>Got the egg - OBTAINED_EGG_CH4</td>
      <td>bool</td>
      <td>Whether you got the Chapter 4 egg. <br></td>
    </tr>
    <tr>
      <td>932</td>
      <td>Damage taken - DAMAGE_TAKEN_COUNT_CH1</td>
      <td>number</td>
      <td>Number of times hit in Chapter 1, used for trophies. <br></td>
    </tr>
    <tr>
      <td>933</td>
      <td>Ice-E pain-scale views - ICE_E_PAIN_SCALE_VIEW_COUNT_CH1</td>
      <td>number</td>
      <td>Number of times you looked at the ICE-E pain scale in Chapter 1, used for trophies. <br></td>
    </tr>
    <tr>
      <td>934</td>
      <td>Damage taken - DAMAGE_TAKEN_COUNT_CH2</td>
      <td>number</td>
      <td>Number of times hit in Chapter 2, used for trophies. <br></td>
    </tr>
    <tr>
      <td>935</td>
      <td>Ice-E pain-scale views - ICE_E_PAIN_SCALE_VIEW_COUNT_CH2</td>
      <td>number</td>
      <td>Number of times you looked at the ICE-E pain scale in Chapter 2, used for trophies. <br></td>
    </tr>
    <tr>
      <td>936</td>
      <td>Damage taken - DAMAGE_TAKEN_COUNT_CH3</td>
      <td>number</td>
      <td>Number of times hit in Chapter 3, used for trophies. <br></td>
    </tr>
    <tr>
      <td>937</td>
      <td>Damage taken - DAMAGE_TAKEN_COUNT_CH4</td>
      <td>number</td>
      <td>Number of times hit in Chapter 4, used for trophies. <br></td>
    </tr>
    <tr>
      <td>938</td>
      <td>Ice-E pain-scale views - ICE_E_PAIN_SCALE_VIEW_COUNT_CH4</td>
      <td>number</td>
      <td>Number of times you looked at the ICE-E pain scale in Chapter 4, used for trophies. <br></td>
    </tr>
    <tr>
      <td>939</td>
      <td>Amount Treasure - TREASURE_CHEST_COUNT</td>
      <td>number</td>
      <td>Number of chests opened, used for trophies. <br></td>
    </tr>
    <tr>
      <td>950</td>
      <td>Shadow failed - SHADOW_FAILED_CH2</td>
      <td>bool</td>
      <td>Whether you used the Shadow Crystal in Chapter 2 and saw nothing. 952 is more interesting. <br></td>
    </tr>
    <tr>
      <td>951</td>
      <td>Glass failed - GLASS_FAILED_CH2</td>
      <td>bool</td>
      <td>Whether you used the Glass in Chapter 2 and saw nothing. 953 and 281 are more interesting. <br></td>
    </tr>
    <tr>
      <td>952</td>
      <td>Shadow Lab - SHADOW_LAB</td>
      <td>bool</td>
      <td>Whether you saw the computer lab using the Shadow Crystal. <br></td>
    </tr>
    <tr>
      <td>953</td>
      <td>Glass Susie Glare - GLASS_SUSIE_GLARE</td>
      <td>bool</td>
      <td>Whether you saw Susie glare at you using the Glass. <br></td>
    </tr>
    <tr>
      <td>954</td>
      <td>Jevil Crystal - GAVE_JEVIL_CRYSTAL</td>
      <td>bool</td>
      <td>Whether you gave Seam JEVIL's Shadow Crystal. <br></td>
    </tr>
    <tr>
      <td>961</td>
      <td>Failed Spam Crystal - FAILED_SPAM_CRYSTAL</td>
      <td>bool</td>
      <td>Whether you got JEVIL's Shadow Crystal but failed to find Spamton's, and told Seam. They seem quite dejected... <br></td>
    </tr>
    <tr>
      <td>1001</td>
      <td>Tiny pyramid puzzle - TINY_PYRAMID_STATE</td>
      <td>map</td>
      <td>Progress finding the even tinier pyramid in Desert Board. Resets to 0 if you enter Rouxls's shop. <br>0 = Default state<br>1 = Tiny pyramid mentioned<br>2 = Rouxls evicted<br>3 = Locked out<br></td>
    </tr>
    <tr>
      <td>1002</td>
      <td>Started the Shadow Mantle fight - FOUGHT_SHADOWMANTLE</td>
      <td>bool</td>
      <td>Whether you've started the Shadow Mantle fight. Speeds up repeat fights, as your death isn't a real Game Over and doesn't reload a save. <br></td>
    </tr>
    <tr>
      <td>1003</td>
      <td>Tenna show game overs - BOARD_LOSSES</td>
      <td>number</td>
      <td>Number of Game Overs attained in Tenna's show. <br></td>
    </tr>
    <tr>
      <td>1004</td>
      <td>Got the maze-crowd treasure - OBTAINED_CROWD_TREASURE</td>
      <td>bool</td>
      <td>Whether you opened the chest in the lower-left corner of that maze with Zapper+Shuttah fights. <br></td>
    </tr>
    <tr>
      <td>1005</td>
      <td>Found the maze crowd - FOUND_MAZE_CROWD</td>
      <td>bool</td>
      <td>Whether you triggered the cheering crowd in the upper-right corner of that maze with Zapper+Shuttah fights. <br></td>
    </tr>
    <tr>
      <td>1006</td>
      <td>Forest cut room count - FOREST_CUT_PROGRESS</td>
      <td>number</td>
      <td>Number of repeating forest rooms passed through looking for the Ice Key. <br></td>
    </tr>
    <tr>
      <td>1007</td>
      <td>Kicked from original game - SWORDROUTE_EVICT</td>
      <td>bool</td>
      <td>Whether you've (recently) done something to get yourself kicked out of the original game. Like dying. <br></td>
    </tr>
    <tr>
      <td>1008</td>
      <td>Found shadow teaser message - FOUND_SHADOWTEASE</td>
      <td>bool</td>
      <td>Whether you found the "See you soon" hidden message in the Sword Route. <br></td>
    </tr>
    <tr>
      <td>1009</td>
      <td>Shadow teaser eyes - SHADOWTEASE_EYES</td>
      <td>bool</td>
      <td>Whether you saw the teaser eyes on the side of the pyramid in Sword Board 1. <br></td>
    </tr>
    <tr>
      <td>1010</td>
      <td>Shadow teaser grin - SHADOWTEASE_GRIN</td>
      <td>bool</td>
      <td>Whether you saw the teaser grin on the side of the pyramid in Sword Board 1. <br></td>
    </tr>
    <tr>
      <td>1011</td>
      <td>Gameshow battles entered - GAMESHOW_BATTLES</td>
      <td>number</td>
      <td>Number of battles entered on Tenna's show? Unaccessed, but there's an empty code block here. <br></td>
    </tr>
    <tr>
      <td>1012</td>
      <td>Letter 1 - GAMESHOW_NAME_1</td>
      <td>map</td>
      <td>First letter selected for Kris's name on the game show. <br>Every number corresponds to a lettter. <br> 0 = A,<br> 1 = B,<br> 2 = C, etc.</td>
    </tr>
    <tr>
      <td>1013</td>
      <td>Letter 2 - GAMESHOW_NAME_2</td>
      <td>map</td>
      <td>Second letter selected for Kris's name on the game show. <br>Every number corresponds to a lettter. <br> 0 = A,<br> 1 = B,<br> 2 = C, etc.</td>
    </tr>
    <tr>
      <td>1014</td>
      <td>Letter 3 - GAMESHOW_NAME_3</td>
      <td>map</td>
      <td>Third letter selected for Kris's name on the game show. <br>Every number corresponds to a lettter. <br> 0 = A,<br> 1 = B,<br> 2 = C, etc.</td>
    </tr>
    <tr>
      <td>1017</td>
      <td>Favorite weather attack - FAVORITE_WEATHER_ATTACK</td>
      <td>map</td>
      <td>Whose attack you liked better, causing the Weather to not Stick Together. <br>0 = Elnina<br>1 = Lanino<br></td>
    </tr>
    <tr>
      <td>1018</td>
      <td>Saw the Nowhere prerequisite board - SAW_NOWHERE_PREREQUISITE_BOARD</td>
      <td>bool</td>
      <td>Whether you saw the board that's a prerequisite for solving Nowhere. Unaccessed. <br></td>
    </tr>
    <tr>
      <td>1019</td>
      <td>Quiz correct answers - QUIZ_RIGHT_ANSWERS</td>
      <td>number</td>
      <td>Number of correct answers (totalled on all characters) in the most recent of Tenna's quizzes. Slightly alters the Tenna-sphinx dialogue. <br></td>
    </tr>
    <tr>
      <td>1020</td>
      <td>Got the Power Croissant for Susie - OBTAINED_POWER_CROISSANT</td>
      <td>bool</td>
      <td>Whether Susie has obtained the Power Croissant, allowing her to pick up boxes, pots, weeds, and Ralsei. <br></td>
    </tr>
    <tr>
      <td>1021</td>
      <td>Walked away - COUCH_WALKAWAY_CH3</td>
      <td>bool</td>
      <td>Whether the couch has begun walking away (if you go right then go back to it) at the start of Chapter 3. <br></td>
    </tr>
    <tr>
      <td>1022</td>
      <td>Tenna left board - TENNA_BOARD_ABSENT</td>
      <td>bool</td>
      <td>Whether Tenna has left the current board, allowing for additional board interactions. <br></td>
    </tr>
    <tr>
      <td>1023</td>
      <td>Cannot grab Ralsei - CANT_GRAB_RALSEI</td>
      <td>bool</td>
      <td>Prevents Susie from picking up Ralsei in Tenna's minigames. <br></td>
    </tr>
    <tr>
      <td>1024</td>
      <td>Board transition freeze - BOARD_TRANSITION_FREEZE</td>
      <td>bool</td>
      <td>Volatile value used to freeze characters on Chapter 3 minigame transitions. <br></td>
    </tr>
    <tr>
      <td>1025</td>
      <td>Board key tracker - UNUSED_BOARD_KEY_COUNT</td>
      <td>number</td>
      <td>Board 1 key count. Unaccessed. See flag 1122 instead. Also incremented if you buy the useless board 2 key. <br></td>
    </tr>
    <tr>
      <td>1027</td>
      <td>S-rank star fallen - DROPPED_S_RANK_ROOM_STAR</td>
      <td>bool</td>
      <td>Whether you interacted with the stars in the S-Rank room, causing one of them to fall on the floor. <br></td>
    </tr>
    <tr>
      <td>1028</td>
      <td>Ramb reward - OBTAINED_RAMB_BOARD_REWARD_1</td>
      <td>map</td>
      <td>Whether you got the first board reward from Ramb (if available based on rank). <br>0 = Default state<br>1 = Got prize<br>2 = Got nothing (Z-Rank)<br></td>
    </tr>
    <tr>
      <td>1029</td>
      <td>Ramb backstage talk - RAMB_BACKSTAGE_DIALOGUE_PROGRESS</td>
      <td>map</td>
      <td>How much you've talked with Ramb backstage. <br>0 = Default state<br>1 = Ramb moved away from the door the first time<br>2 =&nbsp;&nbsp;"I'm glad you"re having REAL fun, Kris. (moves for the second time)" <br>3 = Talked round 3 (unused?)<br></td>
    </tr>
    <tr>
      <td>1030</td>
      <td>Ramb reward - OBTAINED_RAMB_BOARD_REWARD_2</td>
      <td>map</td>
      <td>Whether you got the second board reward from Ramb (if available based on rank). <br>0 = Default state<br>1 = Got prize<br>2 = Got nothing (Z-Rank)<br></td>
    </tr>
    <tr>
      <td>1031</td>
      <td>Entered rank room - ENTERED_CHANGING_ROOM</td>
      <td>bool</td>
      <td>Whether you've interacted to enter the S- or Z-Rank room. Stops Susie's and Ralsei's dialogue on repeat. <br></td>
    </tr>
    <tr>
      <td>1032</td>
      <td>Talked to Ramb first - TALKED_TO_RAMB</td>
      <td>bool</td>
      <td>Whether you've talked to Ramb at least once in the Green Room. Alters repeat interaction. <br></td>
    </tr>
    <tr>
      <td>1033</td>
      <td>Tried racing game - TRIED_RACING</td>
      <td>bool</td>
      <td>Whether you've interacted with the TV with the racing game at least once. Alters repeat interaction. <br></td>
    </tr>
    <tr>
      <td>1034</td>
      <td>Racing game plays - PLAYED_RACING_COUNT</td>
      <td>number</td>
      <td>Number of times you played the unseeable racing game. <br></td>
    </tr>
    <tr>
      <td>1035</td>
      <td>Won racing game - WON_RACING</td>
      <td>bool</td>
      <td>Whether you won the racing game. Susie refuses to play any more afterward. <br></td>
    </tr>
    <tr>
      <td>1037</td>
      <td>Ralsei cheer equips - RAL_CHEER_EQUIP_COUNT</td>
      <td>number</td>
      <td>Number of times you've equipped the Blue Ribbon to Ralsei, giving progress of a cheer chant. <br></td>
    </tr>
    <tr>
      <td>1038</td>
      <td>Pipis inventory sounds - PIPIS_SOUNDS</td>
      <td>map</td>
      <td>Status of the Pipis in your inventory. Increases over time. <br>0 = Default state<br>1 = Chirping<br>2 = Clucking<br></td>
    </tr>
    <tr>
      <td>1039</td>
      <td>Tenna Pipis bonus state - TENNA_PIPIS_STATE</td>
      <td>map</td>
      <td>State of Tenna's Pipis in the Bonus Zone (without Spamton). <br>0 = Default state<br>1 = Tenna panicked<br>2 = Got Pipis<br></td>
    </tr>
    <tr>
      <td>1040</td>
      <td>Got the hero photo - OBTAINED_HERO_PHOTO</td>
      <td>bool</td>
      <td>Whether you've photographed the three heroes for Shuttah. The same flag is reused in some scrapped content. <br></td>
    </tr>
    <tr>
      <td>1041</td>
      <td>Got the half-flower photo - OBTAINED_HALF_FLOWER</td>
      <td>bool</td>
      <td>Whether you've photographed the half flower in Board 2. <br></td>
    </tr>
    <tr>
      <td>1042</td>
      <td>Got the spring photo - OBTAINED_SPRING_PHOTO</td>
      <td>bool</td>
      <td>Whether you've photographed the healing green spring in Board 2. <br></td>
    </tr>
    <tr>
      <td>1043</td>
      <td>Got the cactus photo - OBTAINED_CACTUS_PHOTO</td>
      <td>bool</td>
      <td>Whether you've photographed the only cactus in Board 2. <br></td>
    </tr>
    <tr>
      <td>1044</td>
      <td>Points - POINTS_CH3</td>
      <td>number</td>
      <td>Your point total in Chapter 3. <br></td>
    </tr>
    <tr>
      <td>1045</td>
      <td>Healing practice - SUSIE_HEAL_PRACTICE_COUNT</td>
      <td>number</td>
      <td>The number of times you have used UltraHeal/OKHeal/BetterHeal. Improves the spell. Caps at 5 in Chapter 3, 15 in Chapter 4. <br></td>
    </tr>
    <tr>
      <td>1047</td>
      <td>Outcome - KNIGHT_BATTLE_OUTCOME_CH3</td>
      <td>map</td>
      <td>Whether you beat the Knight... down to 80% of its health. Also saved to ini. <br>0 = Default state<br>1 = Won<br>2 = Lost<br></td>
    </tr>
    <tr>
      <td>1048</td>
      <td>Lancer purchase cost - LANCER_COST</td>
      <td>map</td>
      <td>Amount spent on Lancer in Board 2. Decreases if he is photographed before purchase. <br>0 = Uninitialized<br>9 = 9 points<br>99 = 99 points<br>999 = 999 points<br></td>
    </tr>
    <tr>
      <td>1049</td>
      <td>Board 1 Battles Count - BOARD_1_BATTLES</td>
      <td>number</td>
      <td>Number of battles engaged in on Board 1. <br></td>
    </tr>
    <tr>
      <td>1050</td>
      <td>Defeated - DEFEATED_MANTLE</td>
      <td>bool</td>
      <td>Whether the Shadow Mantle boss was defeated. <br></td>
    </tr>
    <tr>
      <td>1051</td>
      <td>Cheater admits count - ADMITTED_CHEAT_COUNT</td>
      <td>number</td>
      <td>Number of times you admitted to Zappers that you're a cheater, usually triggering a battle. <br></td>
    </tr>
    <tr>
      <td>1052</td>
      <td>Tenna deleted grass - TENNA_DELETED_GRASS</td>
      <td>bool</td>
      <td>Whether Tenna deleted the grass to keep Susie from wasting time on it in the unused Board 3. <br></td>
    </tr>
    <tr>
      <td>1054</td>
      <td>Tenna voice pitch - TENNA_VOICE_PITCH</td>
      <td>map</td>
      <td>Appears to be a volatile factor applied to Tenna's voice bite. Only used for his flashback. <br>0 = Uninitialized<br>1 = Full pitch<br>0.8 = 80% pitch<br></td>
    </tr>
    <tr>
      <td>1055</td>
      <td>Progress - SWORD_ROUTE_PROGRESS</td>
      <td>map</td>
      <td>Progress on the Sword Route, the Chapter 3 side quest for the Shadow Mantle. <br>0 = Not started<br>1 = Got Ice Key<br>2 = She was used up.<br>3 = Got Shelter Key<br>4 = Entered red dungeon<br>5 = Entered shelter<br>6 = Defeated boss<br>1.5 = Entered Ice Palace<br></td>
    </tr>
    <tr>
      <td>1056</td>
      <td>Kris talked with Tenna - KRIS_TENNA_CHAT</td>
      <td>bool</td>
      <td>Whether Tenna tried to justify himself to Kris between rounds. <br></td>
    </tr>
    <tr>
      <td>1057</td>
      <td>Backstage sequence - UNUSED_BACKSTAGE_SEQUENCE</td>
      <td>number</td>
      <td>Unused tracker for a scrapped backstage sequence in Chapter 3. <br></td>
    </tr>
    <tr>
      <td>1058</td>
      <td>Found Tropic Tenna - FOUND_ISLAND_TENNA</td>
      <td>bool</td>
      <td>Whether you found Tenna at the Tropic of Love on the original game, and heard his musings. <br></td>
    </tr>
    <tr>
      <td>1059</td>
      <td>Rouxls battle - ROUXLS_RULES_CARD_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Battle status of the Rouxls Kaard Rules Card battle. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1060</td>
      <td>Got the Elnina controller - OBTAINED_UNUSED_ELNINA_CONTROLLER</td>
      <td>bool</td>
      <td>Whether you got the Elnina Controller for an unused game. The item ID got repurposed as the Odd Controller. <br></td>
    </tr>
    <tr>
      <td>1061</td>
      <td>Shadowmen photo count - SHADOWGUNNER_PHOTOS</td>
      <td>number</td>
      <td>Number of photos taken of the Shadowmen shooting at you from trees. They have bunny ears after 5. <br></td>
    </tr>
    <tr>
      <td>1062</td>
      <td>Got the Curtain Saber - OBTAINED_CURTAIN_SABER10</td>
      <td>bool</td>
      <td>Whether you got the Saber10 from the quiet person behind the S-Rank curtain. <br></td>
    </tr>
    <tr>
      <td>1066</td>
      <td>Heard Ramb explain the fountain - HEARD_RAMB_FOUNTAIN_EXPLANATION</td>
      <td>bool</td>
      <td>Whether Ramb explained (after Board 3) that he saw Kris make the fountain. <br></td>
    </tr>
    <tr>
      <td>1067</td>
      <td>Got Shadow Mantle - OBTAINED_SHADOWMANTLE</td>
      <td>bool</td>
      <td>Whether you've opened the chest containing the Shadow Mantle. <br></td>
    </tr>
    <tr>
      <td>1068</td>
      <td>Talked to Lancer in the Green Room - TALKED_TO_LANCER_IN_GREEN_ROOM</td>
      <td>bool</td>
      <td>Whether you've talked to Lancer in the Green Room (and he phased through the door). <br></td>
    </tr>
    <tr>
      <td>1071</td>
      <td>Skipped intro - COUCH_SKIP_CH3</td>
      <td>bool</td>
      <td>Whether you used the couch to skip to Board 1 in Chapter 3. <br></td>
    </tr>
    <tr>
      <td>1073</td>
      <td>Lancer Quiz Name - LANCER_TV_NAME</td>
      <td>map</td>
      <td>What you (and Ralsei) named Lancer in Tenna's quiz. <br>0 = Lancer<br>1 = Dancer<br>2 = Prancer<br>3 = Mr. Generosity<br></td>
    </tr>
    <tr>
      <td>1074</td>
      <td>Got first S-Rank access - OBTAINED_IN_S_RANK_1</td>
      <td>bool</td>
      <td>Whether you've talked to the Zapper guarding the S-Rank room and gotten in for board 1. <br></td>
    </tr>
    <tr>
      <td>1075</td>
      <td>Got second S-Rank access - OBTAINED_IN_S_RANK_2</td>
      <td>bool</td>
      <td>Whether you've talked to the Zapper guarding the S-Rank room and gotten in for board 2. <br></td>
    </tr>
    <tr>
      <td>1076</td>
      <td>Counterfeit Rank 1 - COUNTERFEIT_S_1</td>
      <td>map</td>
      <td>Buying the counterfeit S-Rank for Board 1. <br>0 = Default state<br>1 = Have counterfeit<br>2 = Reset<br></td>
    </tr>
    <tr>
      <td>1077</td>
      <td>Counterfeit Rank 2 - COUNTERFEIT_S_2</td>
      <td>map</td>
      <td>Buying the counterfeit S-Rank for Board 2. <br>0 = Default state<br>1 = Have counterfeit<br>2 = Reset<br></td>
    </tr>
    <tr>
      <td>1078</td>
      <td>Got moss - OBTAINED_MOSS_CH3</td>
      <td>bool</td>
      <td>Whether you got the Moss in Chapter 3 and the Moss Mystery title. <br></td>
    </tr>
    <tr>
      <td>1079</td>
      <td>Drank the oasis dry - DRANK_OASIS</td>
      <td>bool</td>
      <td>Whether you chose to deplete the oasis by drinking it. Dries up all the trees. <br></td>
    </tr>
    <tr>
      <td>1080</td>
      <td>Susiezilla losses - SUSIEZILLA_LOSS_COUNT</td>
      <td>number</td>
      <td>Times lost at Suziezilla, up to 8. <br></td>
    </tr>
    <tr>
      <td>1081</td>
      <td>Susiezilla result - SUSIEZILLA_RESULT</td>
      <td>map</td>
      <td>Exactly how much you won at Suziezilla. <br>0 = Default state<br>1 = Destroyed by Spamton's big shot without ever hitting him<br>2 = Declared win by Tenna<br>3 = Defeated final wave<br></td>
    </tr>
    <tr>
      <td>1083</td>
      <td>Saw the Lancer-name question - OBTAINED_LANCER_NAME_Q</td>
      <td>bool</td>
      <td>Whether you've faced the question of Tenna forgetting Lancer's name. Unaccessed. <br></td>
    </tr>
    <tr>
      <td>1084</td>
      <td>Ramb game response - RAMB_GAME_OPINION</td>
      <td>map</td>
      <td>Your choice to Ramb of whether you're enjoying Tenna's game. <br>0 = Default state<br>1 = Super fun<br>2 = Eh<br></td>
    </tr>
    <tr>
      <td>1085</td>
      <td>Puzzle Started - UNUSED_BOARD_PUZZLE_STARTED</td>
      <td>bool</td>
      <td>Set when you enter an unused Chapter 3 room with a board puzzle. <br></td>
    </tr>
    <tr>
      <td>1086</td>
      <td>Beat Doom Shadowman - DEFEATED_DOOM_SHADOWMAN</td>
      <td>bool</td>
      <td>Whether you've defeated the Shadowman on the Doom Board, to prompt the Zapper encounter instead. <br></td>
    </tr>
    <tr>
      <td>1087</td>
      <td>Entered Ice Palace - ENTERED_ICE_PALACE</td>
      <td>bool</td>
      <td>Set upon entering the Ice Palace on Sword Board 2 as a checkpoint. <br></td>
    </tr>
    <tr>
      <td>1088</td>
      <td>Cheated dice value - CHEATED_DICE_VAL</td>
      <td>map</td>
      <td>Number on the die in the unused room where a Pippins challenges you to roll even. <br>0 = Uninitialized<br>1 = 1<br>2 = 2<br>3 = 3<br>4 = 4<br>5 = 5<br>6 = 6<br></td>
    </tr>
    <tr>
      <td>1089</td>
      <td>Cooking losses - COOKING_LOSSES_COUNT</td>
      <td>number</td>
      <td>Times lost at the cooking game. <br></td>
    </tr>
    <tr>
      <td>1090</td>
      <td>Parent Lock 1 Intro - PARENT_LOCK_1_SCENE</td>
      <td>bool</td>
      <td>Whether you've completed specifically the introductory scene activating the puzzle for Parental Lock 1. <br></td>
    </tr>
    <tr>
      <td>1091</td>
      <td>Susie noticed sword - SUSIE_NOTICE_SWORD</td>
      <td>map</td>
      <td>Status of Susie noticing Kris has a sword in the minigame if the OddController was obtained. <br>0 = Default state<br>1 = Sword used<br>2 = Susie commented<br></td>
    </tr>
    <tr>
      <td>1092</td>
      <td>Bibliox quest - BIBLIOX_QUEST_PROGRESS_CH3</td>
      <td>map</td>
      <td>Progress obtaining the TripTicket to Nowhere from the Bibliox. <br>0 = Default state<br>1 = Wardrobe mentioned<br>2 = Wardrobe appeared<br>3 = Wardrobe checked<br>4 = Got TripTicket<br>5 = Got post-Mantle hint<br>6 = Got alternate TripTicket<br></td>
    </tr>
    <tr>
      <td>1093</td>
      <td>Cheater jailed - JAILED_CHEATER</td>
      <td>bool</td>
      <td>Whether you confessed to the Zapper that you are cheaters, and went into the highly escapable prison. <br></td>
    </tr>
    <tr>
      <td>1094</td>
      <td>Parental Lock 1 Solved - PARENT_LOCK_1</td>
      <td>bool</td>
      <td>Whether you solved the first parental lock in Chapter 3. <br></td>
    </tr>
    <tr>
      <td>1095</td>
      <td>Parental Lock 2 Solved - PARENT_LOCK_2</td>
      <td>bool</td>
      <td>Whether you solved the second parental lock in Chapter 3. <br></td>
    </tr>
    <tr>
      <td>1096</td>
      <td>Rhythm game failures - RHYTHM_GAME_LOSSES</td>
      <td>number</td>
      <td>Total number of losses on the rock band game. <br></td>
    </tr>
    <tr>
      <td>1097</td>
      <td>ID card puzzle found - UNUSED_ID_CARD_PUZZLE_FOUND</td>
      <td>bool</td>
      <td>Whether you found the water interaction in the unused ID card puzzle. <br></td>
    </tr>
    <tr>
      <td>1098</td>
      <td>Cheater Pippins fled - CHEATER_PIP_LEFT</td>
      <td>bool</td>
      <td>Whether the unused dice-cheating Pippins have fled from being photographed. <br></td>
    </tr>
    <tr>
      <td>1099</td>
      <td>Lancer controllers - LANCER_CONTROL_NUM</td>
      <td>number</td>
      <td>Number of Lancer Controllers obtained. <br></td>
    </tr>
    <tr>
      <td>1100</td>
      <td>Got Cool Trashy's reward - OBTAINED_COOL_TRASHY_REWARD</td>
      <td>bool</td>
      <td>Whether you got Trashy's DeluxeDinner. <br></td>
    </tr>
    <tr>
      <td>1101</td>
      <td>Found - POINT_CHEST_STATE</td>
      <td>map</td>
      <td>Progress with the 10-point chest in the dust pile at the start of Chapter 3. <br>0 = Default state<br>1 = Found chest<br>2 = Got points<br></td>
    </tr>
    <tr>
      <td>1102</td>
      <td>Zapper sneezed - ZAPPER_SNEEZED</td>
      <td>bool</td>
      <td>Whether a Zapper left of the Chapter 3 starting area gave itself away by sneezing. <br></td>
    </tr>
    <tr>
      <td>1103</td>
      <td>Ice key missing - ICE_KEY_FAIL</td>
      <td>bool</td>
      <td>Whether you reached the Ice Palace with no key, thus forgetting something important. <br></td>
    </tr>
    <tr>
      <td>1104</td>
      <td>Got the cut Ribbick item - OBTAINED_CUT_RIBBICK_ITEM</td>
      <td>bool</td>
      <td>Set for a Ribbick trigger in an unused room. <br></td>
    </tr>
    <tr>
      <td>1105</td>
      <td>Cut Ribbick fights - CUT_RIBBICK_FIGHTS</td>
      <td>number</td>
      <td>Counts up with a Ribbick trigger in an unused room. <br></td>
    </tr>
    <tr>
      <td>1106</td>
      <td>Cut weather puzzle - DID_CUT_WEATHER_PUZ</td>
      <td>bool</td>
      <td>Flag for an unused puzzle involving a bridge and the Weather Duo. <br></td>
    </tr>
    <tr>
      <td>1107</td>
      <td>Lanina puzzle found - UNUSED_LANINA_PUZZLE_FOUND</td>
      <td>bool</td>
      <td>Whether you found the water interaction in the unused Rouxls and Lanina puzzle. <br></td>
    </tr>
    <tr>
      <td>1108</td>
      <td>Lanina puzzle grass - UNUSED_LANINA_PUZZLE_GRASS_COUNT</td>
      <td>number</td>
      <td>Amount of grass plucked by Susie in the unused Rouxls and Lanina puzzle. Just keeps you from re-plucking. <br></td>
    </tr>
    <tr>
      <td>1109</td>
      <td>Preegg block X - PRE_EGG_BLOCK_X</td>
      <td>number</td>
      <td>X coordinate of the persistent block needed for the Ch3 egg. <br></td>
    </tr>
    <tr>
      <td>1110</td>
      <td>Preegg block Y - PRE_EGG_BLOCK_Y</td>
      <td>number</td>
      <td>Y coordinate of the persistent block needed for the Ch3 egg. <br></td>
    </tr>
    <tr>
      <td>1111</td>
      <td>Block state - PRE_EGG_BLOCK_STATE</td>
      <td>map</td>
      <td>Status of the puzzle with the persistent block needed for the Ch3 egg. <br>0 = Default state<br>1 = Block saved<br>2 = Puzzle solved<br></td>
    </tr>
    <tr>
      <td>1112</td>
      <td>Solved the Nowhere block puzzle - SOLVED_NOWHERE_BLOCK_PUZZLE</td>
      <td>bool</td>
      <td>Whether you've solved the block puzzle to get to the Chapter 3 Bibliox with the TripTicket. <br></td>
    </tr>
    <tr>
      <td>1113</td>
      <td>Guard Zapper buttons - GUARD_ZAPPER_BUTTONS</td>
      <td>map</td>
      <td>Progress with the Zapper guarding the cold area. <br>0 = Default state<br>1 = Played chest like bongos<br>2 = Shood off<br></td>
    </tr>
    <tr>
      <td>1114</td>
      <td>Guard Zapper fought - GUARD_ZAPPER_FOUGHT</td>
      <td>bool</td>
      <td>Attempting to do nothing against the Zapper guarding the cold area. <br></td>
    </tr>
    <tr>
      <td>1115</td>
      <td>Progress - TENNA_MAILROOM_PROGRESS</td>
      <td>map</td>
      <td>Progress entering Tenna's secret mail room. <br>0 = Default state<br>1 = Discovered<br>2 = Entered<br>3 = Found empty<br></td>
    </tr>
    <tr>
      <td>1116</td>
      <td>Battle points current - POINTS_FROM_BATTLE</td>
      <td>number</td>
      <td>Number of points earned in battles on the current board. Used for the board score. <br></td>
    </tr>
    <tr>
      <td>1117</td>
      <td>Points spent - POINTS_SPENT</td>
      <td>number</td>
      <td>Number of points spent on the current board. Used to include them in the board score as well as held points. <br></td>
    </tr>
    <tr>
      <td>1118</td>
      <td>Last minigame points - LAST_MINIGAME_POINTS</td>
      <td>number</td>
      <td>Number of points earned in the last PHYSICAL CHALLENGE, tracked into the overall round evaluation. <br></td>
    </tr>
    <tr>
      <td>1119</td>
      <td>Watercooler beg count - COOLER_BEG_COUNT</td>
      <td>number</td>
      <td>Number of times begged for mercy from Watercooler. Alters repeat flavortext. <br></td>
    </tr>
    <tr>
      <td>1122</td>
      <td>Count - BOARD_KEY_COUNT</td>
      <td>number</td>
      <td>Board 1 key count. Used to award bonuses for extra keys. Also incremented if you buy the useless board 2 key. <br></td>
    </tr>
    <tr>
      <td>1123</td>
      <td>Entered parental room - ENTERED_PARENT_0</td>
      <td>bool</td>
      <td>Whether you've entered the room before the first Parental Lock, acknowledged by the party. <br></td>
    </tr>
    <tr>
      <td>1124</td>
      <td>Called falling Tenna - TENNA_FALLING_OBJECT_NAME</td>
      <td>map</td>
      <td>What Tenna last called the falling objects on Board 1. Alters Board 2 dialogue. <br>0 = Default state<br>1 = Rocks<br>2 = Peaches<br></td>
    </tr>
    <tr>
      <td>1125</td>
      <td>Started the first cowboy game - STARTED_COWBOY_GAME</td>
      <td>bool</td>
      <td>Whether you reached the first cowboy game in Chapter 3. <br></td>
    </tr>
    <tr>
      <td>1126</td>
      <td>Sneak Caught Topleft - UNUSED_SNEAK_TOP_LEFT_CAPTURE_COUNT</td>
      <td>number</td>
      <td>Number of times captured in the top-left zone of the unused big sneaking section. <br></td>
    </tr>
    <tr>
      <td>1127</td>
      <td>Sneak Caught Topright - UNUSED_SNEAK_TOP_RIGHT_CAPTURE_COUNT</td>
      <td>number</td>
      <td>Number of times captured in the top-right zone of the unused big sneaking section. <br></td>
    </tr>
    <tr>
      <td>1128</td>
      <td>Sneak Caught Botleft - UNUSED_SNEAK_BOTTOM_LEFT_CAPTURE_COUNT</td>
      <td>number</td>
      <td>Number of times captured in the left zone of the unused big sneaking section. <br></td>
    </tr>
    <tr>
      <td>1129</td>
      <td>Sneak Caught Hard1 - UNUSED_SNEAK_HARD_ZONE_1_CAPTURE_COUNT</td>
      <td>number</td>
      <td>Number of times captured in the first "hard" zone of the unused big sneaking section. <br></td>
    </tr>
    <tr>
      <td>1130</td>
      <td>Sneak Caught Hard2 - UNUSED_SNEAK_HARD_ZONE_2_CAPTURE_COUNT</td>
      <td>number</td>
      <td>Number of times captured in the second "hard" zone of the unused big sneaking section. <br></td>
    </tr>
    <tr>
      <td>1131</td>
      <td>Quiz 1 - OVERWORLD_QUIZ_1</td>
      <td>bool</td>
      <td>Whether you completed the 1st overworld quiz while escaping. <br></td>
    </tr>
    <tr>
      <td>1132</td>
      <td>Quiz 2 - OVERWORLD_QUIZ_2</td>
      <td>bool</td>
      <td>Whether you completed the 2nd overworld quiz while escaping. <br></td>
    </tr>
    <tr>
      <td>1133</td>
      <td>Parental Lock 1 Started - PARENT_LOCK_1_START</td>
      <td>bool</td>
      <td>Whether you got a wrong answer for the first parental lock, activating the screen with the puzzle. <br></td>
    </tr>
    <tr>
      <td>1134</td>
      <td>Parental Lock 2 Started - PARENT_LOCK_2_START</td>
      <td>bool</td>
      <td>Whether you've activated the second parental lock puzzle by interacting with it. <br></td>
    </tr>
    <tr>
      <td>1135</td>
      <td>Unlocked stealth - UNLOCKED_STEALTH</td>
      <td>bool</td>
      <td>Whether Susie has suggested the use of stealth. <br></td>
    </tr>
    <tr>
      <td>1136</td>
      <td>PA announcement - UNUSED_PA_ANNOUNCEMENT_FLAG</td>
      <td>bool</td>
      <td>Never set, would have changed the logic of an incomplete "PA" system. <br></td>
    </tr>
    <tr>
      <td>1137</td>
      <td>Found the trash switch - FOUND_TRASH_SWITCH</td>
      <td>bool</td>
      <td>Whether you've activated the trash switch at the end of the first stealth section. <br></td>
    </tr>
    <tr>
      <td>1138</td>
      <td>Got the watercooler item - OBTAINED_UNUSED_WATERCOOLER_ITEM</td>
      <td>bool</td>
      <td>Whether you got an undefined item from an unused watercooler room in Chapter 3. <br></td>
    </tr>
    <tr>
      <td>1139</td>
      <td>Got Revive Mint - OBTAINED_REVIVE_MINT_CH3</td>
      <td>bool</td>
      <td>Whether you got the puzzle-locked Revive Mint in Chapter 3. <br></td>
    </tr>
    <tr>
      <td>1140</td>
      <td>Got one point - OBTAINED_ONE_POINT</td>
      <td>bool</td>
      <td>Whether you got the chest with a singular point in the room with the Zapper who takes you nowhere. <br></td>
    </tr>
    <tr>
      <td>1141</td>
      <td>Bibliox talk count - BIBLIOX_TALK_COUNT_CH3</td>
      <td>number</td>
      <td>Number of times talked to the Chapter 3 in-game Bibliox. Dialogue does not reset. <br></td>
    </tr>
    <tr>
      <td>1142</td>
      <td>Camera reminder puzzle - CAM_REMIND_SOLVE</td>
      <td>map</td>
      <td>Used for the unused camerareminder puzzle in Chapter 3. <br>0 = Default state<br>1 = Solved<br>2 = Solved with Ralsei<br></td>
    </tr>
    <tr>
      <td>1143</td>
      <td>Watercooler Avoid Count - COOLER_AVOID_NUM_COUNT</td>
      <td>number</td>
      <td>Number of times you entered the room with the second Watercooler fight. They get closer up to 5 times, then block the way. Set to 50 after actually doing the fight. <br></td>
    </tr>
    <tr>
      <td>1144</td>
      <td>Watercooler 2 Flirted - COOLER_2_FLIRT</td>
      <td>map</td>
      <td>Status flirting with the second Watercooler. Affects curtain flavortext. <br>0 = Default state<br>1 = Flirted<br>2 = Did not flirt<br>3 = Checked curtain after flirting<br></td>
    </tr>
    <tr>
      <td>1146</td>
      <td>Interacted with the curtain after Watercooler - INTERACTED_WITH_CURTAIN_COOLER</td>
      <td>bool</td>
      <td>Whether you interacted with the curtain after fighting the second Watercooler. <br></td>
    </tr>
    <tr>
      <td>1147</td>
      <td>Paper destroyed - LAWNMOWER_BEAT_PAPER</td>
      <td>bool</td>
      <td>Whether you used the lawnmower to destroy the Shadowmen's contracts. Earns their gratitude if not previously LOST. <br></td>
    </tr>
    <tr>
      <td>1148</td>
      <td>Rouxls Snacks Status - ROUXLS_SNACKS_CH3</td>
      <td>map</td>
      <td>Rouxls's progress when he shows up with the weather duo. <br>0 = Default state<br>1 = Showed up for snacks<br>2 = Took snacks and left<br></td>
    </tr>
    <tr>
      <td>1150</td>
      <td>Parental Lock 3 Progress - PARENT_LOCK_3</td>
      <td>map</td>
      <td>Progress with the third parental lock puzzle. <br>0 = Default state<br>1 = Activated<br>2 = Solved block puzzle<br>3 = Solved bridge puzzle<br>4 = Got camera<br>1.5 = Used TV<br></td>
    </tr>
    <tr>
      <td>1151</td>
      <td>Saw the Spamtenna scene - SAW_SPAMTENNA_SCENE</td>
      <td>bool</td>
      <td>Whether you saw Tenna coat Spamton in foam in self-defense. <br></td>
    </tr>
    <tr>
      <td>1152</td>
      <td>Ralsei horse - HORSE_RALSEI</td>
      <td>bool</td>
      <td>Whether Ralsei forgot to change out of his horse costume. <br></td>
    </tr>
    <tr>
      <td>1153</td>
      <td>Hay Susie Reaction - HAY_RESPONSE</td>
      <td>map</td>
      <td>Set based on how Susie reacts to Ralsei considering eating hay. Depends on whether you've previously eaten moss. <br>0 = Default state<br>1 = It's for sleeping (no moss)<br>2 = Eat spinach (ate moss with Susie)<br></td>
    </tr>
    <tr>
      <td>1154</td>
      <td>Treasure 1 - BONUS_ZONE_TREASURE_1</td>
      <td>bool</td>
      <td>Whether you got the 1st treasure chest (of points) in Tenna's bonus zone. <br></td>
    </tr>
    <tr>
      <td>1155</td>
      <td>Treasure 2 - BONUS_ZONE_TREASURE_2</td>
      <td>bool</td>
      <td>Whether you got the 2nd treasure chest (of points) in Tenna's bonus zone. <br></td>
    </tr>
    <tr>
      <td>1156</td>
      <td>Treasure 3 - BONUS_ZONE_TREASURE_3</td>
      <td>bool</td>
      <td>Whether you got the 3rd treasure chest (of points) in Tenna's bonus zone. <br></td>
    </tr>
    <tr>
      <td>1157</td>
      <td>Points 1 - BONUS_ZONE_POINTS_1</td>
      <td>bool</td>
      <td>Whether you got the 1st coin in Tenna's bonus zone. <br></td>
    </tr>
    <tr>
      <td>1158</td>
      <td>Points 2 - BONUS_ZONE_POINTS_2</td>
      <td>bool</td>
      <td>Whether you got the 2nd coin in Tenna's bonus zone. <br></td>
    </tr>
    <tr>
      <td>1159</td>
      <td>Points 3 - BONUS_ZONE_POINTS_3</td>
      <td>bool</td>
      <td>Whether you got the 3rd coin in Tenna's bonus zone. <br></td>
    </tr>
    <tr>
      <td>1160</td>
      <td>Points 4 - BONUS_ZONE_POINTS_4</td>
      <td>bool</td>
      <td>Whether you got the 4th coin in Tenna's bonus zone. <br></td>
    </tr>
    <tr>
      <td>1161</td>
      <td>Entered - TENNA_BONUS_ZONE</td>
      <td>bool</td>
      <td>Whether you've entered Tenna's Bonus Zone behind the green panel (prior to Pipis scene). <br></td>
    </tr>
    <tr>
      <td>1162</td>
      <td>Bonus Big Chest - BONUS_BIG_CHEST</td>
      <td>bool</td>
      <td>Whether you've opened the giant test in Tenna's Bonus Zone (with a Pippins). <br></td>
    </tr>
    <tr>
      <td>1163</td>
      <td>Recruits checked - CHECK_RECRUITS_CH3</td>
      <td>bool</td>
      <td>Whether you checked the employee list in Chapter 3 to tell if you had missed any recruits. <br></td>
    </tr>
    <tr>
      <td>1164</td>
      <td>Lightmaze Zapper Fought - LIGHTMAZE_FOUGHT</td>
      <td>bool</td>
      <td>Whether you fought the Zapper in the lightmaze room so unused, it has no exits. <br></td>
    </tr>
    <tr>
      <td>1165</td>
      <td>Quiz 3 - OVERWORLD_QUIZ_3</td>
      <td>bool</td>
      <td>Whether you completed an overworld quiz in the big maze room. <br></td>
    </tr>
    <tr>
      <td>1166</td>
      <td>Quiz 4 - OVERWORLD_QUIZ_4</td>
      <td>bool</td>
      <td>Whether you completed an overworld quiz in the big maze room. <br></td>
    </tr>
    <tr>
      <td>1167</td>
      <td>Quiz 5 - OVERWORLD_QUIZ_5</td>
      <td>bool</td>
      <td>Whether you completed an overworld quiz in the big maze room. <br></td>
    </tr>
    <tr>
      <td>1168</td>
      <td>Quiz 6 - OVERWORLD_QUIZ_6</td>
      <td>bool</td>
      <td>Whether you completed an overworld quiz in the big maze room. <br></td>
    </tr>
    <tr>
      <td>1169</td>
      <td>Got Lanina's puzzle points - OBTAINED_UNUSED_LANINA_POINTS</td>
      <td>bool</td>
      <td>Whether you got a 100-point chest in the unused Rouxls and Lanina puzzle room. <br></td>
    </tr>
    <tr>
      <td>1171</td>
      <td>Board 2 Battles Count - BOARD_2_BATTLES</td>
      <td>number</td>
      <td>Number of battles engaged in on Board 2. <br></td>
    </tr>
    <tr>
      <td>1173</td>
      <td>Board rank - RANK_BOARD_1</td>
      <td>map</td>
      <td>Your rank on Board 1. <br>-1 = ?<br>0 = Z<br>1 = C<br>2 = B<br>3 = A<br>4 = S<br>5 = T<br></td>
    </tr>
    <tr>
      <td>1174</td>
      <td>Board rank - RANK_BOARD_2</td>
      <td>map</td>
      <td>Your rank on Board 2. <br>-1 = ?<br>0 = Z<br>1 = C<br>2 = B<br>3 = A<br>4 = S<br>5 = T<br></td>
    </tr>
    <tr>
      <td>1176</td>
      <td>Oddcontroller State - ODD_CONTROLLER_PROGRESS</td>
      <td>map</td>
      <td>Progress obtaining the OddController. <br>0 = Default state<br>1 = Tried game<br>2 = Got controller<br></td>
    </tr>
    <tr>
      <td>1177</td>
      <td>Got Tenna Tie - OBTAINED_TENNA_TIE</td>
      <td>bool</td>
      <td>Whether you got the Tenna Tie from the Ball Machine. <br></td>
    </tr>
    <tr>
      <td>1178</td>
      <td>Got ExecBuffet - OBTAINED_EXECBUFFET</td>
      <td>bool</td>
      <td>Whether you got the Executive Buffet from the Ball Machine. <br></td>
    </tr>
    <tr>
      <td>1179</td>
      <td>Got TensionMax - OBTAINED_TENSIONMAX</td>
      <td>bool</td>
      <td>Whether you got the TensionMax from the Ball Machine. <br></td>
    </tr>
    <tr>
      <td>1180</td>
      <td>Got ReviveMint - OBTAINED_REVIVEMINT</td>
      <td>bool</td>
      <td>Whether you got the Revive Mint from the Ball Machine. <br></td>
    </tr>
    <tr>
      <td>1181</td>
      <td>Got Blue Ribbon - OBTAINED_BLUE_RIBBON</td>
      <td>bool</td>
      <td>Whether you got the Blue Ribbon from the Ball Machine. <br></td>
    </tr>
    <tr>
      <td>1182</td>
      <td>Last bet - GACHA_LASTBET</td>
      <td>number</td>
      <td>Amount previously spent on the gumball machine in Chapter 3, used to compute gold prize odds. Resets upon earning a gold prize. <br></td>
    </tr>
    <tr>
      <td>1184</td>
      <td>Sneaking Fast - SNEAKING_FAST</td>
      <td>bool</td>
      <td>Whether the party has decided to sneak really fast. <br></td>
    </tr>
    <tr>
      <td>1185</td>
      <td>S Rank Room Answer - S_RANK_ROOM_ANSWER</td>
      <td>map</td>
      <td>What you told Susie you were doing in the S-Rank room. <br>0 = Default state<br>1 = Playing games<br>2 = Nothing<br></td>
    </tr>
    <tr>
      <td>1186</td>
      <td>S Rank Return 2 - S_RANK_RETURN_2</td>
      <td>bool</td>
      <td>Whether you've gotten the scene of Ralsei mentioning RPGs after returning from the Sword Island Board. <br></td>
    </tr>
    <tr>
      <td>1187</td>
      <td>Z Rank Door Unlock - Z_RANK_UNLOCK</td>
      <td>map</td>
      <td>Whether you've talked to unlock the Z-Rank door. Changes for each board. <br>0 = Default state<br>1 = Open Board 1<br>2 = Open Board 2<br></td>
    </tr>
    <tr>
      <td>1188</td>
      <td>Watercooler - C_RANK_WATERCOOLER_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Status of the Watercooler encounter in the C-Rank room. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1189</td>
      <td>Unlocked - UNLOCKED_SUSIEZILLA</td>
      <td>bool</td>
      <td>Whether you've purchased access to the Suziezilla game. <br></td>
    </tr>
    <tr>
      <td>1190</td>
      <td>Controls Unjumbled - CONTROL_UNJUMBLE</td>
      <td>map</td>
      <td>Whether you chose to... keep your controls? It's reversed, Ralsei playing as Kris (board 2) is actually the 0 value. <br>0 = You can have a turn<br>1 = Let's all go back to normal<br></td>
    </tr>
    <tr>
      <td>1191</td>
      <td>Manhole used - MANHOLE_ACTIVATION_CH3</td>
      <td>map</td>
      <td>When you last used the Z-Rank manhole to reach the original game. Used to open the return manhole. <br>0 = Default state<br>1 = Opened after board 1<br>2 = Opened after board 2<br></td>
    </tr>
    <tr>
      <td>1192</td>
      <td>S Rank Return 3 - S_RANK_RETURN_3</td>
      <td>bool</td>
      <td>Whether you've gotten the scene of Susie and Ralsei racing after returning with the Shadow Mantle. <br></td>
    </tr>
    <tr>
      <td>1193</td>
      <td>Cooking score - COOKING_BEST_SCORE</td>
      <td>number</td>
      <td>Highest score at the cooking minigame. <br></td>
    </tr>
    <tr>
      <td>1194</td>
      <td>Cooking rank - COOKING_BEST_RANK</td>
      <td>map</td>
      <td>The corresponding rank to your cooking minigame high score. <br>-1 = ?<br>0 = Z<br>1 = C<br>2 = B<br>3 = A<br>4 = S<br>5 = T<br></td>
    </tr>
    <tr>
      <td>1195</td>
      <td>High score - RAISE_BAT_HISCORE</td>
      <td>number</td>
      <td>Highest score on Raise Up Your Bat, Normal Mode <br></td>
    </tr>
    <tr>
      <td>1196</td>
      <td>High rank - RAISE_BAT_HIRANK</td>
      <td>map</td>
      <td>Highest rank on Raise Up Your Bat, Normal Mode <br>-1 = ?<br>0 = Z<br>1 = C<br>2 = B<br>3 = A<br>4 = S<br>5 = T<br></td>
    </tr>
    <tr>
      <td>1197</td>
      <td>High score - SUSIEZILLA_HIGH_SCORE</td>
      <td>number</td>
      <td>High score at Susiezilla. <br></td>
    </tr>
    <tr>
      <td>1198</td>
      <td>High rank - SUSIEZILLA_HIGH_RANK</td>
      <td>map</td>
      <td>The corresponding rank to your Susiezilla high score. <br>-1 = ?<br>0 = Z<br>1 = C<br>2 = B<br>3 = A<br>4 = S<br>5 = T<br></td>
    </tr>
    <tr>
      <td>1199</td>
      <td>Susie Tenna Chat 1 - SUSIE_TENNA_CHAT_1</td>
      <td>bool</td>
      <td>Whether you saw Susie compliment Tenna's show between boards. <br></td>
    </tr>
    <tr>
      <td>1200</td>
      <td>Ralsei Face Thoughts - RALSEI_FACE_THOUGHTS</td>
      <td>map</td>
      <td>Your commentary on Ralsei's face, if not watching Susie. <br>0 = Default state<br>1 = Seen it before<br>2 = It's unique<br>3 = It's cute<br></td>
    </tr>
    <tr>
      <td>1201</td>
      <td>Tenna Opinion Susie - TENNA_OPINION_SUSIE</td>
      <td>map</td>
      <td>Your opinion on Tenna as given to Susie before Board 2. <br>0 = Default state<br>1 = He's fun<br>2 = He sucks<br></td>
    </tr>
    <tr>
      <td>1202</td>
      <td>Opened trash can 1 - OPENED_TRASH_CAN_1_CH3</td>
      <td>bool</td>
      <td>Whether you opened the 1st trash can in Chapter 3, with 10 points inside. <br></td>
    </tr>
    <tr>
      <td>1203</td>
      <td>Opened trash can 2 - OPENED_TRASH_CAN_2_CH3</td>
      <td>bool</td>
      <td>Whether you opened the 2nd trash can in Chapter 3, with nothing inside. <br></td>
    </tr>
    <tr>
      <td>1204</td>
      <td>Opened trash can 3 - OPENED_TRASH_CAN_3_CH3</td>
      <td>bool</td>
      <td>Whether you opened the 3rd trash can in Chapter 3, with the TVSlop. <br></td>
    </tr>
    <tr>
      <td>1205</td>
      <td>Opened trash can 4 - OPENED_TRASH_CAN_4_CH3</td>
      <td>bool</td>
      <td>Whether you opened the 4th trash can in Chapter 3, with nothing inside. <br></td>
    </tr>
    <tr>
      <td>1206</td>
      <td>Opened trash can 5 - OPENED_TRASH_CAN_5_CH3</td>
      <td>bool</td>
      <td>Whether you opened the 5th trash can in Chapter 3, with 2 points inside. <br></td>
    </tr>
    <tr>
      <td>1207</td>
      <td>Opened trash can 6 - OPENED_TRASH_CAN_6_CH3</td>
      <td>bool</td>
      <td>Whether you opened the 6th trash can in Chapter 3, with 50 points inside. <br></td>
    </tr>
    <tr>
      <td>1208</td>
      <td>Susie Tenna Chat 2 - SUSIE_TENNA_CHAT_2</td>
      <td>map</td>
      <td>Progress with Susie questioning Tenna's show between boards. <br>0 = Default state<br>1 = Started scene<br>2 = Finished scene<br></td>
    </tr>
    <tr>
      <td>1209</td>
      <td>Opened trash can 7 - OPENED_TRASH_CAN_7_CH3</td>
      <td>bool</td>
      <td>Whether you opened the 7th trash can in Chapter 3, with nothing inside. <br></td>
    </tr>
    <tr>
      <td>1210</td>
      <td>Elnina Greenroom Talk - ELNINA_GREEN_ROOM_RESPONSE</td>
      <td>map</td>
      <td>What you told Elnina about her relationship in the Green Room. <br>0 = Default state<br>1 = You're strong and independent<br>2 = Your forecast is love<br></td>
    </tr>
    <tr>
      <td>1211</td>
      <td>Lanino Greenroom Talk - LANINO_GREEN_ROOM_RESPONSE</td>
      <td>map</td>
      <td>What you told Lanino about his relationship in the Green Room. <br>0 = Default state<br>1 = You're strong and independent<br>2 = Your forecast is love<br></td>
    </tr>
    <tr>
      <td>1212</td>
      <td>Susiebridge State - SUSIEBRIDGE_STATE</td>
      <td>map</td>
      <td>Progress on the unused Susie bridging minigame. <br>0 = Default state<br>1 = ???<br>2 = Complete<br></td>
    </tr>
    <tr>
      <td>1213</td>
      <td>Got 300 points - OBTAINED_300_POINTS</td>
      <td>bool</td>
      <td>Whether you got the chest of points in the room with a Susie board puzzle. <br></td>
    </tr>
    <tr>
      <td>1214</td>
      <td>Who Asked Okay - PARENTAL_LOCK_CONCERN_TARGET</td>
      <td>map</td>
      <td>Who you asked whether they were okay in the Chapter 3 parental lock room. <br>0 = Default state<br>1 = Susie<br>2 = Ralsei<br>3 = Neither<br></td>
    </tr>
    <tr>
      <td>1215</td>
      <td>Susie Reassurance Response - SUSIE_REASSURANCE</td>
      <td>map</td>
      <td>What you said to Susie (if talking to her) in the parental lock room. <br>0 = Default state<br>1 = I'm not a dream (creepy)<br>2 = Your friendships are real (fake-heroic)<br>3 = Sucks to be you (unwittingly ironic)<br></td>
    </tr>
    <tr>
      <td>1216</td>
      <td>Ralsei Reassurance Response - RALSEI_REASSURANCE</td>
      <td>map</td>
      <td>What you said to Ralsei (if talking to him) in the parental lock room. <br>0 = Default state<br>1 = It's ok to take it easy<br>2 = Stay on task<br></td>
    </tr>
    <tr>
      <td>1217</td>
      <td>Icecream For Susie - ICECREAM_FOR_SUSIE</td>
      <td>map</td>
      <td>What you said to Ralsei about getting ice cream from him to Susie. <br>0 = Default state<br>1 = I'm not going with her<br>2 = I'm saying it's from me<br>3 = Of course<br></td>
    </tr>
    <tr>
      <td>1218</td>
      <td>Festival Ralsei Whoelse - FESTIVAL_RAL_WHOELSE</td>
      <td>map</td>
      <td>Who you told Ralsei you're going to the festival with, if not Susie. <br>0 = Default state<br>1 = Noelle<br>2 = Ralsei<br>3 = Berdly (BERDLY!?)<br>4 = Not going<br></td>
    </tr>
    <tr>
      <td>1219</td>
      <td>Saw the Susiezilla intro - SAW_SUSIEZILLA_INTRO</td>
      <td>bool</td>
      <td>Whether you completed the intro scene for the Susiezilla game. <br></td>
    </tr>
    <tr>
      <td>1220</td>
      <td>Beat Susiezilla - COMPLETED_SUSIEZILLA</td>
      <td>bool</td>
      <td>Whether you reached the elusive BOARD CLEAR of the Suziezilla game. <br></td>
    </tr>
    <tr>
      <td>1221</td>
      <td>Got the Watercooler crater points - OBTAINED_COOLER_CRATER</td>
      <td>bool</td>
      <td>Whether you got the 200 points from underneath the C-Rank Watercooler. <br></td>
    </tr>
    <tr>
      <td>1222</td>
      <td>Got Golden Tenna - OBTAINED_TENNA_STATUE</td>
      <td>bool</td>
      <td>Whether you got the Golden Tenna Statue from the Ball Machine. <br></td>
    </tr>
    <tr>
      <td>1223</td>
      <td>Got Dog Dollar - OBTAINED_DOG_DOLLAR</td>
      <td>bool</td>
      <td>Whether you got the Dog Dollar from the Ball Machine. <br></td>
    </tr>
    <tr>
      <td>1224</td>
      <td>Opened - OPENED_BONUS_ZONE</td>
      <td>bool</td>
      <td>Whether you opened Tenna's secret bonus zone behind a green screen. <br></td>
    </tr>
    <tr>
      <td>1225</td>
      <td>Opened - OPENED_SAMS_ZONE</td>
      <td>bool</td>
      <td>Whether you opened the secret zone where you can choose whether the talking cages love or hate. Behind a green screen. <br></td>
    </tr>
    <tr>
      <td>1226</td>
      <td>Entered - OBTAINED_1225_ROOM</td>
      <td>bool</td>
      <td>Whether you entered the secret 1225 room in the Ball Machine game. Yes, the flag is so close. <br></td>
    </tr>
    <tr>
      <td>1227</td>
      <td>Got the red-antlion photo - OBTAINED_ANTLION_PHOTO</td>
      <td>bool</td>
      <td>Whether you photographed the red antlion in Board 2. <br></td>
    </tr>
    <tr>
      <td>1228</td>
      <td>Entered Cold Place - ENTERED_COLDPLACE</td>
      <td>bool</td>
      <td>Whether you've entered the Cold Place and such has been acknowledged by the party. <br></td>
    </tr>
    <tr>
      <td>1229</td>
      <td>Times caught - LAST_SNEAK_TIMES_FOUND_COUNT</td>
      <td>number</td>
      <td>Number of times caught by the Zapper who later reveals he does not want to be there either. <br></td>
    </tr>
    <tr>
      <td>1230</td>
      <td>Zapper state - SNEAK_ZAPPER_STATE</td>
      <td>map</td>
      <td>Progress with the Zapper who does not want to be there either. <br>0 = Default state<br>1 = Zapper joined<br>2 = Passed room<br></td>
    </tr>
    <tr>
      <td>1231</td>
      <td>Parental Lock 3 Done - PARENT_LOCK_3_DONE</td>
      <td>bool</td>
      <td>Whether you solved the undefined parental lock in Chapter 3, optional on Sword Route. <br></td>
    </tr>
    <tr>
      <td>1232</td>
      <td>Started the second cowboy game - STARTED_COWBOY_GAME_2</td>
      <td>bool</td>
      <td>Whether you reached the second cowboy game in Chapter 3. <br></td>
    </tr>
    <tr>
      <td>1233</td>
      <td>Parental Lock 3 Used - PARENT_LOCK_3_USED</td>
      <td>bool</td>
      <td>Whether you went through the door after the undefined parental lock in Chapter 3. <br></td>
    </tr>
    <tr>
      <td>1234</td>
      <td>Susiezilla Best Time - SUSIEZILLA_BEST_TIME</td>
      <td>number</td>
      <td>The duration of your best Suziezilla run. <br></td>
    </tr>
    <tr>
      <td>1235</td>
      <td>Tenna Mad At Staff - TENNA_MAD_AT_STAFF</td>
      <td>bool</td>
      <td>Whether you've seen the scene where Tenna gets mad the Darkners haven't found the Lightners yet. <br></td>
    </tr>
    <tr>
      <td>1236</td>
      <td>Saw Ramb quit - SAW_RAMB_QUIT_SCENE</td>
      <td>bool</td>
      <td>Whether you've seen the scene where Tenna gets mad Ramb is quitting on him. <br></td>
    </tr>
    <tr>
      <td>1237</td>
      <td>Bought Rouxls's block - OBTAINED_ROUXLS_BLOCK</td>
      <td>bool</td>
      <td>Whether you purchased Rouxls's block for 1 point. <br></td>
    </tr>
    <tr>
      <td>1238</td>
      <td>Moved Ramb to the final game - MOVED_RAMB_TO_FINAL_GAME</td>
      <td>bool</td>
      <td>Whether you've moved Ramb to play the final game. <br></td>
    </tr>
    <tr>
      <td>1239</td>
      <td>Ramb Petrify Story - RAMB_PETRIFICATION_LORE_PROGRESS</td>
      <td>map</td>
      <td>Your progress in learning about why Ramb petrified. <br>0 = Default state<br>1 = Spawned Pippins<br>2 = "No one will shed a tear for him."<br></td>
    </tr>
    <tr>
      <td>1240</td>
      <td>Talked to original &ensp;*Starwalker* - TALKED_TO_STARWALKER_CH3</td>
      <td>bool</td>
      <td>Whether you've talked to Starwalker in the first room after escaping Tenna. <br></td>
    </tr>
    <tr>
      <td>1241</td>
      <td>Ralsei Suspect Zapper - RAL_SUSPECT_ZAPPER</td>
      <td>bool</td>
      <td>Whether you've interacted with the Zapper guarding the parental locks, preventing Ralsei's dialogue from repeating. <br></td>
    </tr>
    <tr>
      <td>1242</td>
      <td>Best Food Stack - BEST_FOOD_STACK</td>
      <td>number</td>
      <td>Number of food items successfully served in a single simultaneous stack in the cooking minigame. Used to track the record on replay. <br></td>
    </tr>
    <tr>
      <td>1243</td>
      <td>Zapper Jail 2 State - ZAPPER_JAIL_2</td>
      <td>map</td>
      <td>Progress on the second highly ineffective jail you are placed in by a Zapper while sneaking. <br>0 = Default state<br>1 = Imprisoned<br>2 = Escaped<br></td>
    </tr>
    <tr>
      <td>1244</td>
      <td>Got the Parental Lock camera - OBTAINED_PARENTAL_LOCK_CAMERA</td>
      <td>bool</td>
      <td>Whether you got the camera in the Parental Lock 3 puzzle. <br></td>
    </tr>
    <tr>
      <td>1245</td>
      <td>Parental Photos Num - NUM_PARENT_PHOTOS</td>
      <td>number</td>
      <td>Number of photos taken in the Parental Lock 3 puzzle. The in-game console crashes after 8. <br></td>
    </tr>
    <tr>
      <td>1246</td>
      <td>Dug up the 100-point hole - OBTAINED_100_DIG</td>
      <td>bool</td>
      <td>Whether you dug up the rare 100-point hole in the room with the many Lancers. <br></td>
    </tr>
    <tr>
      <td>1248</td>
      <td>Level-ups - LEVEL_UP_COUNT_CH3</td>
      <td>number</td>
      <td>The number of times you have leveled up by violently defeating an encounter. Used for certain increases that only occur every 2, 4, or 10 encounters. <br></td>
    </tr>
    <tr>
      <td>1249</td>
      <td>AT/Magic gains - AT_MAGIC_GAIN_COUNT_CH3</td>
      <td>number</td>
      <td>The number of times your AT and Magic have increased due to leveling up (every ten encounters). <br></td>
    </tr>
    <tr>
      <td>1250</td>
      <td>Talked to the jailed Pippins - TALKED_TO_JAILED_PIPPINS</td>
      <td>bool</td>
      <td>Whether you've talked to the imprisoned Pippins selling TV Dinners. Alters repeat interaction. <br></td>
    </tr>
    <tr>
      <td>1251</td>
      <td>Tale - GOULDEN_SON_TALE</td>
      <td>map</td>
      <td>Progress telling of Goulden Son. <br>0 = Default state<br>1 = Interacted with 2<br>2 = 2 knew of 1<br>3 = 1 became 3<br>4 = Told of 3<br>1.5 = Told of 2<br></td>
    </tr>
    <tr>
      <td>1252</td>
      <td>Destination - GOULDEN_SON_DESTINATION</td>
      <td>map</td>
      <td>Used to determine which is Goulden Son and which is Goulden Son 2. The one you interact with first after the lights are gone will be Goulden Son. <br>0 = Default state<br>1 = Right is Goulden Son 2<br>2 = Left is Goulden Son 2<br></td>
    </tr>
    <tr>
      <td>1253</td>
      <td>Opened trash can 8 - OPENED_TRASH_CAN_8_CH3</td>
      <td>bool</td>
      <td>Whether you opened the 8th trash can in Chapter 3, with 120 points inside. <br></td>
    </tr>
    <tr>
      <td>1254</td>
      <td>Stone Lancer Seen - STONE_LANCER_CH3</td>
      <td>bool</td>
      <td>Whether you saw Lancer petrified in Chapter 3 (in the room where you get his controllers). <br></td>
    </tr>
    <tr>
      <td>1255</td>
      <td>Kills - SWORD_ROUTE_KILLS</td>
      <td>number</td>
      <td>Number of enemies killed using your sword in the Chapter 3 minigames. Appears in Kris's stats. <br></td>
    </tr>
    <tr>
      <td>1256</td>
      <td>Grass plucked - PLUCKED_GRASS_COUNT</td>
      <td>number</td>
      <td>The number of times Susie plucks grass in the Chapter 3 minigames. Appears in Susie's stats (up to 99). <br></td>
    </tr>
    <tr>
      <td>1257</td>
      <td>Ralsei carried - CARRIED_RALSEI_COUNT</td>
      <td>number</td>
      <td>The number of times Ralsei was carried in the Chapter 3 minigames. Appears in Ralsei's stats (up to 99). <br></td>
    </tr>
    <tr>
      <td>1258</td>
      <td>Run reminder - RUN_REMINDER_CH3</td>
      <td>bool</td>
      <td>Whether Susie reminded you you can run at the start of Chapter 3. <br></td>
    </tr>
    <tr>
      <td>1259</td>
      <td>Run reminder 2 - SECOND_RUN_REMINDER_CH3</td>
      <td>bool</td>
      <td>Whether Ralsei reminded you you can run in Chapter 3. <br></td>
    </tr>
    <tr>
      <td>1260</td>
      <td>Talked to Ralsei at the eye puzzle - TALKED_TO_RALSEI_AT_EYE_PUZZLE</td>
      <td>bool</td>
      <td>Whether you've talked to Ralsei at the Chapter 3 starting eye puzzle. Alters repeat dialogue. <br></td>
    </tr>
    <tr>
      <td>1261</td>
      <td>Talked to Susie at the eye puzzle - TALKED_TO_SUSIE_AT_EYE_PUZZLE</td>
      <td>bool</td>
      <td>Whether you've talked to Susie at the Chapter 3 starting eye puzzle. Alters repeat dialogue. <br></td>
    </tr>
    <tr>
      <td>1262</td>
      <td>Parental Lock 1 Close - PARENT_LOCK_1_CLOSE_COUNT</td>
      <td>number</td>
      <td>Number of times you got the first parental lock numbers, but in the wrong order. Ralsei has special dialogue for the first couple tries. <br></td>
    </tr>
    <tr>
      <td>1263</td>
      <td>Almost-beaten dialogue - ALMOST_BEAT_KNIGHT</td>
      <td>bool</td>
      <td>Whether you've gotten the one-off pep talk from Gaster for reaching the damage threshold then dying. <br></td>
    </tr>
    <tr>
      <td>1264</td>
      <td>Deaths - KNIGHT_DEATHS_COUNT</td>
      <td>number</td>
      <td>Number of times you died to the Knight -- it doesn't reset your save when you retry. <br></td>
    </tr>
    <tr>
      <td>1265</td>
      <td>Phaser Cannons - PHASER_CANNONS</td>
      <td>bool</td>
      <td>Whether you performed the Phaser Cannons Easter Egg in the cooking minigame. <br></td>
    </tr>
    <tr>
      <td>1266</td>
      <td>Moved Ramb after round 2 - MOVED_RAMB_AFTER_ROUND_2</td>
      <td>bool</td>
      <td>Whether you've talked to Ramb after round 2 for him to move away from the door. <br></td>
    </tr>
    <tr>
      <td>1267</td>
      <td>Lawnmower score - LAWNMOWER_SCORE</td>
      <td>number</td>
      <td>Score in Tenna's lawnmower minigame, minimum 1. Reused for a TVDinner chest. <br></td>
    </tr>
    <tr>
      <td>1268</td>
      <td>Mini Attack Susie - MINI_ATTACK_SUSIE</td>
      <td>bool</td>
      <td>Whether the mini-Kris tried to attack Susie, causing her to offer to let Kris gnaw her hair. <br></td>
    </tr>
    <tr>
      <td>1269</td>
      <td>Shadow Home Seen - SHADOW_HOME</td>
      <td>bool</td>
      <td>Whether you saw the smashed TV using the Shadow Crystal. <br></td>
    </tr>
    <tr>
      <td>1270</td>
      <td>Shadow failed - SHADOW_FAILED_CH3</td>
      <td>bool</td>
      <td>Whether you used the Shadow Crystal in Chapter 3 and saw nothing. 1269 is more interesting. <br></td>
    </tr>
    <tr>
      <td>1271</td>
      <td>Glass Undyne Froze - GLASS_UNDYNE_FROZE</td>
      <td>bool</td>
      <td>Whether you used the Glass in Chapter 3 and saw Undyne frozen in ice. Unused; you cannot visit the Light World in Chapter 3. <br></td>
    </tr>
    <tr>
      <td>1272</td>
      <td>Glass failed - GLASS_FAILED_CH3</td>
      <td>bool</td>
      <td>Whether you used the Glass in Chapter 3 and saw nothing. 1271 is more interesting. <br></td>
    </tr>
    <tr>
      <td>1273</td>
      <td>Japanese mode - GAMESHOW_NAME_JA</td>
      <td>bool</td>
      <td>Whether the start of Chapter 3 (naming Kris on the show) was played in Japanese. <br></td>
    </tr>
    <tr>
      <td>1274</td>
      <td>Backup letter 1 - GAMESHOW_NAME_1_BACKUP</td>
      <td>map</td>
      <td>Secondary tracker for the first letter of Kris's name (used for safety with translation). <br>Every number corresponds to a lettter. <br> 0 = A,<br> 1 = B,<br> 2 = C, etc.</td>
    </tr>
    <tr>
      <td>1275</td>
      <td>Backup letter 2 - GAMESHOW_NAME_2_BACKUP</td>
      <td>map</td>
      <td>Secondary tracker for the second letter of Kris's name (used for safety with translation). <br>Every number corresponds to a lettter. <br> 0 = A,<br> 1 = B,<br> 2 = C, etc.</td>
    </tr>
    <tr>
      <td>1276</td>
      <td>Backup letter 3 - GAMESHOW_NAME_3_BACKUP</td>
      <td>map</td>
      <td>Secondary tracker for the third letter of Kris's name (used for safety with translation). <br>Every number corresponds to a lettter. <br> 0 = A,<br> 1 = B,<br> 2 = C, etc.</td>
    </tr>
    <tr>
      <td>1277</td>
      <td>Pippins chests - PIPPINS_BONUS_STOLE</td>
      <td>number</td>
      <td>Appears? to be the number of chests looted by Pippinses in Tenna's bonus zone. <br></td>
    </tr>
    <tr>
      <td>1278</td>
      <td>Soda - SWORDROUTE_SODA</td>
      <td>map</td>
      <td>Status of the soda left by Susie after obtaining the Shadow Mantle. <br>0 = Default state<br>1 = Soda placed<br>2 = Soda collected<br></td>
    </tr>
    <tr>
      <td>1279</td>
      <td>Hard score - RAISE_BAT_HARD_HISCORE</td>
      <td>number</td>
      <td>High score on Raise Up Your Bat, Hard Mode. (Unused in Chapter 3) <br></td>
    </tr>
    <tr>
      <td>1280</td>
      <td>Hard rank - RAISE_BAT_HARD_HIRANK</td>
      <td>map</td>
      <td>Highest rank on Raise Up Your Bat, Hard Mode. (Unused in Chapter 3) <br>-1 = ?<br>0 = Z<br>1 = C<br>2 = B<br>3 = A<br>4 = S<br>5 = T<br></td>
    </tr>
    <tr>
      <td>1312</td>
      <td>Pink Coins - PINK_COINS</td>
      <td>number</td>
      <td>Your amount of Pink Coins. <br></td>
    </tr>
    <tr>
      <td>1365</td>
      <td>Scissors puzzle flags - SCISSORS_PUZZLE_FLAGS</td>
      <td>number</td>
      <td>Raw bitfield state for Chapter 5 scissors puzzle progress. <br></td>
    </tr>
    <tr>
      <td>1391</td>
      <td>Voice Clips - VOICE_CLIPS_ENABLED</td>
      <td>bool</td>
      <td>Voice Clips toggle in settings. <br></td>
    </tr>
    <tr>
      <td>1399</td>
      <td>Hop Chef progress - HOPSCHEF_PROGRESS_FLAG</td>
      <td>number</td>
      <td>Raw progress state for the Hop Chef challenge. <br></td>
    </tr>
    <tr>
      <td>1404</td>
      <td>Ribbon chest state - RIBBON_CHEST_STATE</td>
      <td>map</td>
      <td>Tracks the Chapter 5 RedRibbon chest and first ribbon equip scenes. <br>0 = Default state<br>1 = Opened chest; Susie can equip ribbons<br>2 = First equipped ribbon on Kris<br>3 = First equipped ribbon on Susie<br>4 = First equipped ribbon on Ralsei<br></td>
    </tr>
    <tr>
      <td>1411</td>
      <td>Flowery Dollars - FLOWERY_DOLLARS</td>
      <td>number</td>
      <td>Your amount of Flowery Dollars. <br></td>
    </tr>
    <tr>
      <td>1421</td>
      <td>Hair - THRASH_FIT_HAIR</td>
      <td>map</td>
      <td>Thrash Fit hair variant. <br>0 = Normal<br>1 = Ponytail<br>2 = Royal Bob<br>3 = Duck Tiara<br>4 = Fresh Swish<br>5 = Princey<br></td>
    </tr>
    <tr>
      <td>1422</td>
      <td>Shirt - THRASH_FIT_SHIRT</td>
      <td>map</td>
      <td>Thrash Fit shirt variant. <br>0 = Dark Jacket<br>1 = Rip Jacket<br>2 = Similar Hood<br>3 = Duck<br>4 = Lancer Shirt<br>5 = Royal Dress<br>6 = Swag Jacket<br>7 = Tuxusie<br></td>
    </tr>
    <tr>
      <td>1423</td>
      <td>Pants - THRASH_FIT_PANTS</td>
      <td>map</td>
      <td>Thrash Fit pants variant. <br>0 = Susie Pant<br>1 = Shorter<br>2 = Bagi<br>3 = Duck<br>4 = White Pant<br>5 = Gray Pants<br>6 = Blackpants2<br></td>
    </tr>
    <tr>
      <td>1424</td>
      <td>Hat - THRASH_FIT_HAT</td>
      <td>map</td>
      <td>Thrash Fit hat variant. <br>0 = No Hat<br>1 = Casual Hat<br>2 = Second Hat<br>3 = Tiara<br>4 = Silk<br></td>
    </tr>
    <tr>
      <td>1425</td>
      <td>Shoes - THRASH_FIT_SHOES</td>
      <td>map</td>
      <td>Thrash Fit shoes variant. <br>0 = Susie Shoesy<br>1 = Brown Leg<br>2 = Black Flats<br>3 = Duck<br>4 = Glass Shoes<br>5 = Brown Shoe<br>6 = Blackshoes3<br></td>
    </tr>
    <tr>
      <td>1435</td>
      <td>Toriel toast request - TALKED_TORIEL_TOAST_REQUEST</td>
      <td>map</td>
      <td>Toriel toast request answer. <br>0 = Default state<br>1 = Yes<br>2 = I'm busy<br></td>
    </tr>
    <tr>
      <td>1438</td>
      <td>Looked at microwave - LOOKED_AT_MICROWAVE</td>
      <td>bool</td>
      <td>Looked at microwave while it was running. <br></td>
    </tr>
    <tr>
      <td>1440</td>
      <td>Castle climb high score - CASTLE_CLIMB_HISCORE</td>
      <td>number</td>
      <td>Castle Town climbing minigame high score. <br></td>
    </tr>
    <tr>
      <td>1443</td>
      <td>Seen "How To Draw Dragons" - SEEN_HOW_TO_DRAW_DRAGONS</td>
      <td>bool</td>
      <td>Seen "How To Draw Dragons" inside the drawer. <br></td>
    </tr>
    <tr>
      <td>1500</td>
      <td>$100 Reward - MONEYFOUNTAIN_DONATION_OVER_100</td>
      <td>bool</td>
      <td>Donated at least 100 Dark Dollars to the money fountain. <br></td>
    </tr>
    <tr>
      <td>1501</td>
      <td>Cutscene - CANDY_BOWL_PROGRESS</td>
      <td>map</td>
      <td>Tracks your progress in the candy bowl cutscene. <br>0 = Default state<br>1 = Approached candy bowl<br>2 = Spilled candy bowl<br></td>
    </tr>
    <tr>
      <td>1502</td>
      <td>Ripple progress - RIPPLE_WORSHIP_PROGRESS</td>
      <td>map</td>
      <td>Tracks your progress in the ripple worship room. <br>0 = Default state<br>1 = Opened the north path<br>2 = Revealed the piano notes<br></td>
    </tr>
    <tr>
      <td>1503</td>
      <td>Organikk at fountain - GERSON_TEA_FINISHED</td>
      <td>bool</td>
      <td>Finished the tea party with Gerson. <br></td>
    </tr>
    <tr>
      <td>1504</td>
      <td>Checked the church cupboard - INTERACTED_WITH_CHURCH_CUPBOARD</td>
      <td>bool</td>
      <td>Interacted with the cupboard while looking for the code to the church's locked door. <br></td>
    </tr>
    <tr>
      <td>1505</td>
      <td>Checked the church books - INTERACTED_WITH_CHURCH_BOOKS</td>
      <td>bool</td>
      <td>Interacted with the books while looking for the code to the church's locked door. <br></td>
    </tr>
    <tr>
      <td>1506</td>
      <td>Checked the church candles - INTERACTED_WITH_CHURCH_CANDLES</td>
      <td>bool</td>
      <td>Interacted with the candles before going inside. <br></td>
    </tr>
    <tr>
      <td>1507</td>
      <td>Prayer target - WHO_KRIS_PRAYED_FOR</td>
      <td>map</td>
      <td>Who you decided to pray for in front of the hope candles. <br>0 = Default state<br>1 = Pray for Susie<br>2 = Pray for Noelle<br>3 = Pray for Asriel<br></td>
    </tr>
    <tr>
      <td>1508</td>
      <td>Checked the church bookshelf - INTERACTED_WITH_CHURCH_BOOKSHELF</td>
      <td>bool</td>
      <td>Interacted with the bookshelf while looking for the code to the church's locked door. <br></td>
    </tr>
    <tr>
      <td>1509</td>
      <td>Candles answer - WHAT_CANDLES_ARE_FOR</td>
      <td>map</td>
      <td>What you told Susie when she asked if the candles were for birthdays. <br>0 = Default state<br>1 = That's right<br>2 = Prayer<br></td>
    </tr>
    <tr>
      <td>1510</td>
      <td>Opened the church closet - OPENED_CHURCH_CLOSET</td>
      <td>bool</td>
      <td>Viewed the cutscene of opening the church closet and getting jumpscared by Jackenstein. <br></td>
    </tr>
    <tr>
      <td>1511</td>
      <td>Piano story - LISTENED_SUSIE_PIANO_STORY</td>
      <td>map</td>
      <td>Viewed the cutscene of Susie telling her story about smashing a piano. <br>0 = Default state<br>1 = Listen (it might be long)<br>2 = Not now<br></td>
    </tr>
    <tr>
      <td>1512</td>
      <td>Piano story response - WILL_KRIS_PLAY_AGAIN</td>
      <td>map</td>
      <td>What you told Susie after her piano story. Unaccessed as of chapter 4. <br>0 = Default state<br>1 = I'll play again someday<br>2 = If you play too<br>3 = I'll never play again<br></td>
    </tr>
    <tr>
      <td>1513</td>
      <td>Talked to Jackenstein in the study - TALKED_TO_JACKENSTEIN_IN_STUDY</td>
      <td>bool</td>
      <td>Talked to Jackenstein in Gerson's study. <br></td>
    </tr>
    <tr>
      <td>1514</td>
      <td>Sugar - WOULD_YOU_LIKE_SUGAR</td>
      <td>map</td>
      <td>What you said to Ralsei asking if you would like sugar during his tea party. <br>0 = Default state<br>1 = No<br>2 = Yes<br>3 = Two lumps please<br></td>
    </tr>
    <tr>
      <td>1515</td>
      <td>Who eats the cake? - WHO_EATS_THE_CAKE</td>
      <td>map</td>
      <td>What you said to Ralsei after he said he never had cake before during his tea party. Unaccessed as of chapter 4. <br>0 = Default state<br>1 = Ralsei eat the cake<br>2 = That's my cake<br></td>
    </tr>
    <tr>
      <td>1516</td>
      <td>Surprise - RALSEI_HAS_A_SURPRISE</td>
      <td>bool</td>
      <td>Whether Ralsei told you he had a surprise if we went into our rooms in Castle Town. <br></td>
    </tr>
    <tr>
      <td>1517</td>
      <td>Got the worship-room chest - OBTAINED_WORSHIP_CHEST</td>
      <td>bool</td>
      <td>Got the Mystic Band / Power Band from the chest in the worship room. <br></td>
    </tr>
    <tr>
      <td>1519</td>
      <td>Secret piano tea answer - GERSON_TEA_FANCY_A_DRINK</td>
      <td>map</td>
      <td>What you said when Gerson asked if you would fancy a drink. <br>0 = Default state<br>1 = Yes<br>2 = No<br>3 = We already had tea<br></td>
    </tr>
    <tr>
      <td>1521</td>
      <td>Waterfall tea answer - GERSON_TEA_DRINK_IT</td>
      <td>map</td>
      <td>What you did after getting sugar in your tea with Gerson. <br>0 = Default state<br>1 = Drink it<br>2 = Don't drink it<br></td>
    </tr>
    <tr>
      <td>1523</td>
      <td>Third tearoom answer - GERSON_TEA_ARE_YOU_SURE</td>
      <td>map</td>
      <td>What you said when Gerson asked you if you were sure you didn't want to have tea now. <br>0 = Default state<br>1 = Not now<br>2 = Actually I will have tea<br></td>
    </tr>
    <tr>
      <td>1524</td>
      <td>First time - CLIMBING_CHALLENGE_FIRST_TIME</td>
      <td>number</td>
      <td>How fast you did the first climbing challenge. <br></td>
    </tr>
    <tr>
      <td>1525</td>
      <td>Second time - CLIMBING_CHALLENGE_SECOND_TIME</td>
      <td>number</td>
      <td>How fast you did the second climbing challenge. <br></td>
    </tr>
    <tr>
      <td>1526</td>
      <td>Mizzle progress - AWAKENED_MIZZLE_PROGRESS</td>
      <td>map</td>
      <td>Tracks the progress of awakening the Mizzle protected by the cups. <br>0 = Default state<br>1 = First cup started charging<br>2 = Mizzle left<br>3 = Started exiting (triggers shortened return path)<br></td>
    </tr>
    <tr>
      <td>1527</td>
      <td>Saw the Noelle-house Weird Route cutscene - FINISHED_NOELLE_HOUSE_WEIRD</td>
      <td>bool</td>
      <td>Viewed the cutscene after coming out of the Noelle's house during the Weird Route. Unaccessed as of chapter 4. <br></td>
    </tr>
    <tr>
      <td>1528</td>
      <td>Hometown cutscene - HOMETOWN_WEIRD_CUTSCENE_PROGRESS</td>
      <td>map</td>
      <td>Tracks the progress of the cutscene in the Weird Route when you walk with Susie in the rain. <br>0 = Default state<br>1 = Got dialogue near Sans' store<br>2 = Got dialogue near church<br></td>
    </tr>
    <tr>
      <td>1529</td>
      <td>Broke the Knight prophecy - BROKE_KNIGHT_PROPHECY</td>
      <td>bool</td>
      <td>Broke the Knight prophecy in the north prophecies room. <br></td>
    </tr>
    <tr>
      <td>1530</td>
      <td>Activated the left shortcut - ACTIVATED_TRUE_CLIMB_LEFT_SHORTCUT</td>
      <td>bool</td>
      <td>Rung the left bell to activate the left shortcut in the climbing room leading to the grand piano. <br></td>
    </tr>
    <tr>
      <td>1531</td>
      <td>Talked to Nubert in Castle Town - TALKED_TO_NUBERT_CH4</td>
      <td>bool</td>
      <td>Talked to Nubert in Castle Town in chapter 4. <br></td>
    </tr>
    <tr>
      <td>1532</td>
      <td>Talked to Rudinn in Castle Town - TALKED_TO_RUDINN_CH4</td>
      <td>bool</td>
      <td>Talked to Rudinn in Castle Town in chapter 4. <br></td>
    </tr>
    <tr>
      <td>1533</td>
      <td>Church sermon choice A - SLEPT_THROUGH_SERVICE</td>
      <td>map</td>
      <td>Whether you chose to sleep through service at church. Unaccessed as of chapter 4. <br>0 = Default state<br>1 = Sleep through service<br>2 = Watch service<br></td>
    </tr>
    <tr>
      <td>1534</td>
      <td>Church sermon choice B - WHAT_YOU_DID_DURING_SERVICE</td>
      <td>map</td>
      <td>What you chose to do during service at church. Unaccessed as of chapter 4. <br>0 = Default state<br>1 = Let's play attention<br>2 = Look in pocket for fun<br></td>
    </tr>
    <tr>
      <td>1535</td>
      <td>Checked the choir door - INTERACTED_WITH_CHURCH_CHOIR_DOOR</td>
      <td>bool</td>
      <td>Interacted with the church's choir room's door before going inside. <br></td>
    </tr>
    <tr>
      <td>1536</td>
      <td>Checked the church office door - INTERACTED_WITH_CHURCH_OFFICE_DOOR</td>
      <td>bool</td>
      <td>Interacted with the church's office's door before going inside. <br></td>
    </tr>
    <tr>
      <td>1537</td>
      <td>Got the Money Fountain chest - OBTAINED_MONEYFOUNTAIN_CHEST</td>
      <td>bool</td>
      <td>Got the Darker Candy / Scarlixir / Revive Mint / Bitter Tear / Gold Widow from the chest in the money fountain room. <br></td>
    </tr>
    <tr>
      <td>1538</td>
      <td>Moved the movable piano - MOVED_MOVABLE_PIANO</td>
      <td>bool</td>
      <td>Moved a movable piano. <br></td>
    </tr>
    <tr>
      <td>1539</td>
      <td>Got the library-connector chest - OBTAINED_LIBRARYCONNECTOR_CHEST</td>
      <td>bool</td>
      <td>Got the Rhapsotea from the chest in the Second Sanctuary's library connector room. <br></td>
    </tr>
    <tr>
      <td>1540</td>
      <td>Got the library chest - OBTAINED_LIBRARY_CHEST</td>
      <td>bool</td>
      <td>Got the Revive Mint from the chest in the Second Sanctuary's library. <br></td>
    </tr>
    <tr>
      <td>1541</td>
      <td>Breakable Bookshelves State Alt - BREAKABLE_BOOKSHELVES_STATE_ALT</td>
      <td>number</td>
      <td>Tracks the state of the breakable bookshelves in the unused alternate Second Sanctuary's library. <br></td>
    </tr>
    <tr>
      <td>1543</td>
      <td>Removed the piano and bookshelves - REMOVED_PIANO_AND_BOOKSHELVES</td>
      <td>bool</td>
      <td>Flag never set, but would have removed the moving piano and bookshelves in the Second Sanctuary's library. <br></td>
    </tr>
    <tr>
      <td>1544</td>
      <td>Alerted the Mizzles - ALERTED_MIZZLES</td>
      <td>bool</td>
      <td>Prevented future Mizzles to start a battle tired, by ringing the bell or waking up an initially tired Mizzle. <br></td>
    </tr>
    <tr>
      <td>1545</td>
      <td>Got the gallery chest - OBTAINED_GALLERY_CHEST</td>
      <td>bool</td>
      <td>Got 500 Dark Dollars from the chest in the Second Sanctuary's gallery. <br></td>
    </tr>
    <tr>
      <td>1547</td>
      <td>Solved the golden piano - SOLVED_GOLDEN_PIANO</td>
      <td>bool</td>
      <td>Played the golden piano and opened the fireplace secret passage in Gerson's study. <br></td>
    </tr>
    <tr>
      <td>1548</td>
      <td>Checked the fireplace mural - INTERACTED_WITH_FIREPLACE_MURAL</td>
      <td>bool</td>
      <td>Interacted with the mural in Gerson's study and read about the cool axe. <br></td>
    </tr>
    <tr>
      <td>1549</td>
      <td>Talked Gerson About Magic Axe - TALKED_TO_GERSON_ABOUT_MAGIC_AXE</td>
      <td>bool</td>
      <td>Talked to Gerson in his study about the Magic Axe. <br></td>
    </tr>
    <tr>
      <td>1550</td>
      <td>Opened the Gerson-chase chest - OPENED_GERSON_CHASE_CHEST</td>
      <td>bool</td>
      <td>Got the Scarlixir from the chest in the Gerson chase room. <br></td>
    </tr>
    <tr>
      <td>1551</td>
      <td>Should Check On Ralsei - SHOULD_CHECK_ON_RALSEI</td>
      <td>map</td>
      <td>What you said to Susie when asked if you should check on Ralsei, after rain starts if you haven't returned to Castle Town in chapter 4 yet. <br>0 = Default state<br>1 = Yeah<br>2 = Nah<br></td>
    </tr>
    <tr>
      <td>1552</td>
      <td>Talked to Napstablook about Undyne - TALKED_TO_NAPSTABLOOK_ABOUT_UNDYNE</td>
      <td>bool</td>
      <td>Talked to Napstablook about Undyne. <br></td>
    </tr>
    <tr>
      <td>1553</td>
      <td>Talked to Napstablook about the shelter - TALKED_TO_NAPSTABLOOK_ABOUT_SHELTER</td>
      <td>bool</td>
      <td>Talked to Napstablook about the Shelter. <br></td>
    </tr>
    <tr>
      <td>1554</td>
      <td>Talked to Catti about Susie in church - TALKED_TO_CATTI_ABOUT_SUSIE_IN_CHURCH</td>
      <td>bool</td>
      <td>Talked to Catti about Susie. <br></td>
    </tr>
    <tr>
      <td>1555</td>
      <td>Locked Kris and Susie out - KRIS_SUSIE_LOCKED_OUT</td>
      <td>bool</td>
      <td>Tried to enter Kris's house after rain started and realized it's locked. <br></td>
    </tr>
    <tr>
      <td>1556</td>
      <td>Checked Gerson's remains - INTERACTED_WITH_GERSON_REMAINS</td>
      <td>bool</td>
      <td>Interacted with the glass container containing Gerson's remains after the cutscene where it's discovered. <br></td>
    </tr>
    <tr>
      <td>1557</td>
      <td>Why We Should Enter Church - WHY_WE_SHOULD_ENTER_CHURCH</td>
      <td>map</td>
      <td>What you said to Susie after she suggested waiting outside the church's Dark World. Unaccessed as of chapter 4. <br>0 = Default state<br>1 = But we aren't logical<br>2 = But Mom could be in there<br></td>
    </tr>
    <tr>
      <td>1558</td>
      <td>Asgore line - NOELLE_BEDROOM_ASGORE_CURRENT_LINE</td>
      <td>map</td>
      <td>Tracks the current line in the Asgore cutscene in Carol's bedroom. <br>0 = Default state<br>1 = We're almost there, aren't we, old friend?<br>2 = This time for sure... Tori will finally see.<br>3 = ... see what really happened.<br>4 = ... that I just wanted to... protect everyone...<br>5 = And this time, she'll have to believe me.<br>6 = ... they all will.<br>7 = Then...<br>8 = We'll all be a happy family again... won't we?<br>9 = ...<br>10 = It sure is beautiful, isn't it...?<br>11 = ... this black shard.<br></td>
    </tr>
    <tr>
      <td>1559</td>
      <td>Kept waiting - KEPT_NOELLE_WAITING</td>
      <td>map</td>
      <td>Whether you did something after opening the gate at Noelle's house while she was waiting for you. <br>0 = Default state<br>1 = Had tea party with Ralsei<br>2 = Had diner with Susie<br></td>
    </tr>
    <tr>
      <td>1560</td>
      <td>Gallery Cutscene Progress - GALLERY_CUTSCENE_PROGRESS</td>
      <td>number</td>
      <td>Tracks the progress of the unused Second Sanctuary's gallery cutscene. Mostly reused for the rotating tower monologue. <br></td>
    </tr>
    <tr>
      <td>1561</td>
      <td>Played MEGALOVANIA - PLAYED_MEGALOVANIA</td>
      <td>bool</td>
      <td>Tried playing Megalovania on the piano and got ran over by the Annoying Dog. <br></td>
    </tr>
    <tr>
      <td>1562</td>
      <td>Searched Dess's belongings - SEARCHED_DESS_BELONGINGS</td>
      <td>bool</td>
      <td>Dug through Dess' stuff in her room. <br></td>
    </tr>
    <tr>
      <td>1563</td>
      <td>Talked to Noelle after throwing away the phone - TALKED_TO_NOELLE_AFTER_PHONE_THROW</td>
      <td>bool</td>
      <td>Talked to Noelle after Susie threw her phone. <br></td>
    </tr>
    <tr>
      <td>1564</td>
      <td>Talked to Susie after throwing away the phone - TALKED_TO_SUSIE_AFTER_PHONE_THROW</td>
      <td>bool</td>
      <td>Talked to Susie after she threw Noelle's phone. <br></td>
    </tr>
    <tr>
      <td>1565</td>
      <td>Asked Asgore about outfit - ASKED_ASGORE_ABOUT_OUTFIT</td>
      <td>bool</td>
      <td>Asked Asgore about his outfit after coming out of Noelle's house. <br></td>
    </tr>
    <tr>
      <td>1566</td>
      <td>Asked Asgore if okay - ASKED_ASGORE_IF_OKAY</td>
      <td>bool</td>
      <td>Asked Asgore if he's okay after coming out of Noelle's house. <br></td>
    </tr>
    <tr>
      <td>1567</td>
      <td>Pressed the Knight-climb bridge switch - PRESSED_KNIGHTCLIMBPOST_SWITCH</td>
      <td>bool</td>
      <td>Pressed the switch making a bridge at the end of the Second Sanctuary. <br></td>
    </tr>
    <tr>
      <td>1569</td>
      <td>Taught Susie BetterHeal - SUSIE_LEARNED_BETTER_HEAL</td>
      <td>bool</td>
      <td>Whether Susie's OKHeal spell improved to BetterHeal, by winning against Gerson or starting the fight against the Sound of Justice. <br></td>
    </tr>
    <tr>
      <td>1570</td>
      <td>Used the item fountain - INTERACTED_WITH_ITEM_FOUNTAIN</td>
      <td>bool</td>
      <td>Interacted with the item fountain in Gerson's study. <br></td>
    </tr>
    <tr>
      <td>1571</td>
      <td>Activated the right shortcut - ACTIVATED_TRUE_CLIMB_RIGHT_SHORTCUT</td>
      <td>bool</td>
      <td>Rung the right bell to activate the right shortcut in the climbing room leading to the grand piano. <br></td>
    </tr>
    <tr>
      <td>1572</td>
      <td>Susie Bellroom Progress - SUSIE_BELLROOM_PROGRESS</td>
      <td>map</td>
      <td>Tracks the progress of Susie in the bell room cutscene. <br>0 = Default state<br>1 = Moved to first point<br>2 = Moved to second point<br></td>
    </tr>
    <tr>
      <td>1573</td>
      <td>Window loops - WINDOWS_LOOPED</td>
      <td>number</td>
      <td>Number of loops done in the Sanctuary's window room. At 8, the Egg door appears. <br></td>
    </tr>
    <tr>
      <td>1574</td>
      <td>Checked the broken TV - INTERACTED_WITH_TV_BROKEN</td>
      <td>bool</td>
      <td>Interacted with the TV at Kris's house, if it wasn't repaired. <br></td>
    </tr>
    <tr>
      <td>1575</td>
      <td>Suggested Tenna - SUGGESTED_TENNA_TO_METTATON</td>
      <td>bool</td>
      <td>Suggested Tenna to Mettaton, if it wasn't repaired. <br></td>
    </tr>
    <tr>
      <td>1576</td>
      <td>Checked the fixed TV - INTERACTED_WITH_TV_FIXED</td>
      <td>bool</td>
      <td>Interacted with the TV at Kris's house, if it was repaired. <br></td>
    </tr>
    <tr>
      <td>1577</td>
      <td>Talked to Swatch - TALKED_TO_SWATCH_IN_CAFE</td>
      <td>bool</td>
      <td>Talked to Swatch in the Cafe, if you've recruited Tasque Manager, Tasque and Shadowguy. <br></td>
    </tr>
    <tr>
      <td>1578</td>
      <td>Talked to Jigsaw Joe - TALKED_TO_JIGSAW_JOE_IN_LOVE_DOJO</td>
      <td>bool</td>
      <td>Talked to Jigsaw Joe now that the dojo has become the Love Dojo. <br></td>
    </tr>
    <tr>
      <td>1579</td>
      <td>Noise count - MADE_NOISE_IN_NOELLE_HOUSE_COUNT</td>
      <td>number</td>
      <td>Number of times you touched a dancing Santa or a bell and made noise in Noelle's house. <br></td>
    </tr>
    <tr>
      <td>1580</td>
      <td>Times Leveled - LEVEL_UP_COUNT_CH4</td>
      <td>number</td>
      <td>The number of times you have leveled up by violently defeating an encounter. Used for certain increases that only occur every 2, 4, or 10 encounters. <br></td>
    </tr>
    <tr>
      <td>1581</td>
      <td>Got the prophecy-maze chest - OBTAINED_PROPHECYMAZE_CHEST</td>
      <td>bool</td>
      <td>Got the Scarlixir from the chest in the Second Sanctuary's statue maze room. <br></td>
    </tr>
    <tr>
      <td>1582</td>
      <td>Opened the bookshelf-puzzle chest - OPENED_BOOKSHELF_PUZZLE_CHEST</td>
      <td>bool</td>
      <td>Got the Absorb Ax from the chest in the bookshelf puzzle room. <br></td>
    </tr>
    <tr>
      <td>1583</td>
      <td>Times Killed By Spawncloud - SPAWN_CLOUD_DEATH_COUNT</td>
      <td>map</td>
      <td>Number of times you died from the spawns chasing you vertically (used to reduce their speed). <br>0 = Default state<br>1 = Died once<br>2 = Died twice<br>3 = Died thrice or more<br></td>
    </tr>
    <tr>
      <td>1584</td>
      <td>Bookshelves - BREAKABLE_BOOKSHELVES_STATE</td>
      <td>number</td>
      <td>Tracks the state of the breakable bookshelves in the Second Sanctuary's library. <br></td>
    </tr>
    <tr>
      <td>1585</td>
      <td>Piano coordinates - MOVING_PIANO_XY</td>
      <td>number</td>
      <td>Combination of X and Y coordinates of the moving piano. <br></td>
    </tr>
    <tr>
      <td>1586</td>
      <td>Got the right-connector chest - OBTAINED_RIGHTCONNECT_CHEST</td>
      <td>bool</td>
      <td>Got the Winglade from the chest in the room on the right of Gerson's study. <br></td>
    </tr>
    <tr>
      <td>1587</td>
      <td>Got the Minor Legend chest - OBTAINED_MINORLEGEND_CHEST</td>
      <td>bool</td>
      <td>Got the Rhapsotea from the chest in the Jockington prophecy room. <br></td>
    </tr>
    <tr>
      <td>1588</td>
      <td>Opened the right piano-piece chest - OPENED_RIGHT_PIANO_PIECE_CHEST</td>
      <td>bool</td>
      <td>Got the Revive Mint from the chest in the right piano piece room. <br></td>
    </tr>
    <tr>
      <td>1589</td>
      <td>Opened the True Climb chest - OPENED_TRUE_CLIMB_CHEST</td>
      <td>bool</td>
      <td>Got the Tension Gem from the chest in the climbing room. <br></td>
    </tr>
    <tr>
      <td>1590</td>
      <td>Got the Jackenstein chest - OBTAINED_JACKENSTEIN_CHEST</td>
      <td>bool</td>
      <td>Got 500 Dark Dollars from the chest in the Jackenstein room. <br></td>
    </tr>
    <tr>
      <td>1591</td>
      <td>Bloody face - RALSEI_BLOODY_FACE</td>
      <td>bool</td>
      <td>Whether Ralsei got blood on his face from Susie at the end of chapter 4. <br></td>
    </tr>
    <tr>
      <td>1592</td>
      <td>Moss - MOSS_OUTCOME_CH4</td>
      <td>map</td>
      <td>Whether you got the moss in chapter 4. <br>0 = Default state<br>1 = Consumed with gusto<br>2 = Left for the next person<br></td>
    </tr>
    <tr>
      <td>1593</td>
      <td>Interacted Gerson Table Second Sanctuary - CHECKED_GERSON_TABLE_SECOND_SANCTUARY</td>
      <td>map</td>
      <td>Interacted with the table in Gerson's study in the Second Sanctuary. <br>0 = Default state<br>1 = Tried to take items<br>2 = Didn't try to take items<br></td>
    </tr>
    <tr>
      <td>1594</td>
      <td>Rhapsotea Extra Dollars - RHAPSOTEA_EXTRA_DOLLARS</td>
      <td>number</td>
      <td>Number of dollars paid extra for the Rhapsoteas in Gerson's study in the Second Sanctuary. <br></td>
    </tr>
    <tr>
      <td>1595</td>
      <td>Room state - WAFER_ROOM_STATE</td>
      <td>map</td>
      <td>Tracks your progression in obtaining the Third Sanctuary Waferguard chest. See also flag 1616. <br>0 = Default state<br>1 = Revealed chest<br>2 = Wafer obtained, area locked (nothing more to do, so the game has blocked off the area)<br></td>
    </tr>
    <tr>
      <td>1596</td>
      <td>Saw the Angel prophecy - SAW_ANGEL_PROPHECY</td>
      <td>bool</td>
      <td>Viewed the cutscene of the gang looking at the angel prophecy. <br></td>
    </tr>
    <tr>
      <td>1597</td>
      <td>Purified - PURIFIED_COUNT</td>
      <td>number</td>
      <td>Number of Titan spawns purified. The Purify ACT will always add two to this flag, even if you've already slain one. <br></td>
    </tr>
    <tr>
      <td>1598</td>
      <td>Slain - SLAIN_COUNT</td>
      <td>number</td>
      <td>Number of Titan spawns slain. <br></td>
    </tr>
    <tr>
      <td>1599</td>
      <td>Used the cup-stack lift - INTERACTED_WITH_CUPSTACK_LIFT</td>
      <td>bool</td>
      <td>Interacted with the cup stack lift. <br></td>
    </tr>
    <tr>
      <td>1600</td>
      <td>Save point - CHECKED_GERSON_STUDY_SAVE_POINT</td>
      <td>map</td>
      <td>Interacted with the save point in Gerson's study. <br>0 = Default state<br>1 = First interaction<br>2 = Second interaction if mural wasn't checked yet<br></td>
    </tr>
    <tr>
      <td>1601</td>
      <td>Used the northwest-connector save point - INTERACTED_WITH_NORTHWEST_CONNECTOR_SAVE_POINT</td>
      <td>bool</td>
      <td>Interacted with the save point in the north-west connector room. <br></td>
    </tr>
    <tr>
      <td>1602</td>
      <td>Used the piano-puzzle save point - INTERACTED_WITH_PIANO_PUZZLE_SAVE_POINT</td>
      <td>bool</td>
      <td>Interacted with the save point in the piano puzzle room before Jackenstein. <br></td>
    </tr>
    <tr>
      <td>1603</td>
      <td>Interacted Superprophecies Savepoint - CHECKED_THIRD_SANCTUARY_MUSIC_SAVE_POINT</td>
      <td>bool</td>
      <td>Interacted with the save point in the room where the Third Sanctuary music starts playing. <br></td>
    </tr>
    <tr>
      <td>1604</td>
      <td>Left Gerson's room without the others - GERSON_LEFT_ROOM_WITHOUT_OTHERS</td>
      <td>bool</td>
      <td>Talked to Gerson after his walk is completed without Susie running ahead. <br></td>
    </tr>
    <tr>
      <td>1605</td>
      <td>Talked Gerson Postsheet Knight - ASKED_GERSON_ABOUT_KNIGHT_AFTER_SHEET_MUSIC</td>
      <td>bool</td>
      <td>Talked to Gerson in his study about the Knight after using the sheet music. <br></td>
    </tr>
    <tr>
      <td>1606</td>
      <td>Missed-something response - THIRD_SANCTUARY_MISSED_SOMETHING_RESPONSE</td>
      <td>map</td>
      <td>Your interaction when asked if you missed something on the other side of your mind. <br>0 = Default state<br>1 = Didn't miss anything (while not having the Egg)<br>2 = Already have the Egg<br></td>
    </tr>
    <tr>
      <td>1607</td>
      <td>Talked Gerson Postjack Letter - ASKED_GERSON_ABOUT_HIS_WORK_AFTER_JACKENSTEIN</td>
      <td>bool</td>
      <td>Talked to Gerson in his study and asked him what he's doing after healing Jackenstein and before getting the sheet music. <br></td>
    </tr>
    <tr>
      <td>1608</td>
      <td>Talked Gerson Postsheet Letter - ASKED_GERSON_ABOUT_HIS_WORK_AFTER_SHEET_MUSIC</td>
      <td>bool</td>
      <td>Talked to Gerson in his study and asked him what he's doing after getting the sheet music. <br></td>
    </tr>
    <tr>
      <td>1609</td>
      <td>Triggered the First Sanctuary temporary save - TRIGGERED_FIRST_SANCTUARY_INTRO_TEMP_SAVE</td>
      <td>bool</td>
      <td>Entered the room with the prophecies at the start of the First Sanctuary (makes a temporary save). <br></td>
    </tr>
    <tr>
      <td>1610</td>
      <td>Got the prophecies chest - OBTAINED_PROPHECIES_CHEST</td>
      <td>bool</td>
      <td>Got the Princess Ribbon from the chest next to the Tail of Hell prophecy. <br></td>
    </tr>
    <tr>
      <td>1611</td>
      <td>Returned Second Jockington Prophecy - RETURNED_SECOND_JOCKINGTON_PROPHECY</td>
      <td>bool</td>
      <td>Returned from the second Jockington prophecy room in the Third Sanctuary. Unaccessed as of chapter 4. <br></td>
    </tr>
    <tr>
      <td>1612</td>
      <td>Checked Gerson's table in the First Sanctuary - CHECKED_GERSON_TABLE_FIRST_SANCTUARY</td>
      <td>bool</td>
      <td>Interacted with the table in Gerson's study in the First Sanctuary. <br></td>
    </tr>
    <tr>
      <td>1613</td>
      <td>Interacted Gerson Table Third Sanctuary - CHECKED_GERSON_TABLE_THIRD_SANCTUARY</td>
      <td>bool</td>
      <td>Interacted with the table in Gerson's study in the Third Sanctuary. <br></td>
    </tr>
    <tr>
      <td>1614</td>
      <td>Got the second-encounter chest - OBTAINED_ENCOUNTER2_CHEST</td>
      <td>bool</td>
      <td>Got 100 Dark Dollars from the chest in the Third Sanctuary's dark maze room. Inaccessible as there isn't actually a chest in this room. <br></td>
    </tr>
    <tr>
      <td>1615</td>
      <td>Started the Third Sanctuary music - STARTED_THIRD_SANCTUARY_MUSIC</td>
      <td>bool</td>
      <td>Entered the room where the Third Sanctuary music plays. <br></td>
    </tr>
    <tr>
      <td>1616</td>
      <td>Got the treasure chest - OBTAINED_TREASURE_CHEST</td>
      <td>bool</td>
      <td>Got the Wafer Guard from the chest in the Third Sanctuary's treasure chest room. <br></td>
    </tr>
    <tr>
      <td>1617</td>
      <td>Checked the useless gloves - INTERACTED_WITH_USELESS_GLOVES</td>
      <td>bool</td>
      <td>Interacted with the hidden chest with the gloves that make you worse at climbing. <br></td>
    </tr>
    <tr>
      <td>1618</td>
      <td>Times Gained AT - AT_MAGIC_GAIN_COUNT_CH4</td>
      <td>number</td>
      <td>The number of times your AT and Magic have increased due to leveling up (every ten encounters). <br></td>
    </tr>
    <tr>
      <td>1619</td>
      <td>Clues gathered - CHURCH_CLUES_GATHERED</td>
      <td>map</td>
      <td>Number of clues gathered at church. <br>0 = Default state<br>1 = 1 clue<br>2 = 2 clues, ready to tell Susie<br></td>
    </tr>
    <tr>
      <td>1620</td>
      <td>Got Noelle's clue - OBTAINED_NOELLE_CLUE</td>
      <td>bool</td>
      <td>Talked to Noelle about the locked door at church. <br></td>
    </tr>
    <tr>
      <td>1621</td>
      <td>Got Alphys's clue - OBTAINED_ALPHYS_CLUE</td>
      <td>bool</td>
      <td>Talked to Alphys about the shelter at church. <br></td>
    </tr>
    <tr>
      <td>1622</td>
      <td>Washed hands during therapy - WASHED_HANDS_THERAPY</td>
      <td>bool</td>
      <td>Used the sink to wash your hands after getting the Egg in chapter 4. Unaccessed as of chapter 4. <br></td>
    </tr>
    <tr>
      <td>1623</td>
      <td>Glass whisper - GLASS_NOELLE_WHISPERING</td>
      <td>bool</td>
      <td>Used the Glass in Noelle's house in chapter 4. <br></td>
    </tr>
    <tr>
      <td>1624</td>
      <td>Sanctuary - SHADOW_SANCTUARY</td>
      <td>bool</td>
      <td>Used the Shadow Crystal in the Sanctuary. <br></td>
    </tr>
    <tr>
      <td>1625</td>
      <td>Final prophecy - SHADOW_FINAL_PROPHECY</td>
      <td>bool</td>
      <td>Used the Shadow Crystal in front of the final prophecy in the Third Sanctuary. <br></td>
    </tr>
    <tr>
      <td>1626</td>
      <td>Failed - SHADOW_FAILED_CH4</td>
      <td>bool</td>
      <td>Whether you used the Shadow Crystal in Chapter 4 and saw nothing. 1624 and 1625 are more interesting. <br></td>
    </tr>
    <tr>
      <td>1627</td>
      <td>Presents - PRESENTS_CHECKED</td>
      <td>number</td>
      <td>Number of presents checked in Noelle's present room. <br></td>
    </tr>
    <tr>
      <td>1628</td>
      <td>Chair skip - CHAIR_SKIP_CH4</td>
      <td>bool</td>
      <td>Whether you used the chair to skip to the First Sanctuary in chapter 4. <br></td>
    </tr>
    <tr>
      <td>1629</td>
      <td>Started Gerson's battle - STARTED_GERSON_BATTLE</td>
      <td>bool</td>
      <td>Started the battle against Gerson. <br></td>
    </tr>
    <tr>
      <td>1630</td>
      <td>Talked to Malius about new fusions - TALKED_TO_MALIUS_ABOUT_NEW_FUSIONS</td>
      <td>bool</td>
      <td>Talked to Malius at the Bakery about NEW FUSIONS. <br></td>
    </tr>
    <tr>
      <td>1631</td>
      <td>Talked Malius Leave - SELECTED_MALIUS_LEAVE_OPTION</td>
      <td>bool</td>
      <td>Selected Malius's Leave dialogue option in chapter 4. <br></td>
    </tr>
    <tr>
      <td>1632</td>
      <td>Talked to Malius - TALKED_TO_MALIUS_CH4</td>
      <td>bool</td>
      <td>Talked to Malius at the Bakery in chapter 4. <br></td>
    </tr>
    <tr>
      <td>1633</td>
      <td>Talked to Topchef - TALKED_TO_TOPCHEF_CH4</td>
      <td>bool</td>
      <td>Talked to Top Chef at the Bakery in chapter 4, if not currently eligible for a SpinCake. <br></td>
    </tr>
    <tr>
      <td>1634</td>
      <td>Pushed back the Spooky Hand - SPOOKY_HAND_PUSHED_BACK</td>
      <td>bool</td>
      <td>Tried to go back after the final prophecy cutscene, and was pushed back by a mysterious hand out of view. <br></td>
    </tr>
    <tr>
      <td>1635</td>
      <td>Knocked on the east door - KNOCKED_EAST_DOOR_END_CH4</td>
      <td>bool</td>
      <td>Knocked on the door at the east of Hometown at the end of chapter 4. <br></td>
    </tr>
    <tr>
      <td>1636</td>
      <td>Run Reminder - RUN_REMINDER_CH4</td>
      <td>bool</td>
      <td>Whether Susie reminded you you can run at the start of Chapter 4. <br></td>
    </tr>
    <tr>
      <td>1637</td>
      <td>Pumpkin Progress - PUMPKIN_PROGRESS</td>
      <td>map</td>
      <td>Tracks the progress of Ralsei's interaction with the pumpkin NPC after the Jackenstein battle. <br>0 = Default state<br>1 = Told a joke<br>2 = Told a story<br></td>
    </tr>
    <tr>
      <td>1638</td>
      <td>Got the dog-climb chest - OBTAINED_DOGCLIMB_CHEST</td>
      <td>bool</td>
      <td>Got the Dog Dollar from the chest in the Annoying Dog climbing race room. <br></td>
    </tr>
    <tr>
      <td>1639</td>
      <td>Used the party ACT on Guei - USED_PARTY_ACTION_ON_GUEI</td>
      <td>bool</td>
      <td>Used S-Action or R-Action during the first Guei encounter, or was reminded if you didn't. <br></td>
    </tr>
    <tr>
      <td>1640</td>
      <td>Attempts - TITAN_ATTEMPT_COUNT</td>
      <td>number</td>
      <td>Number of times you fought the Titan. <br></td>
    </tr>
    <tr>
      <td>1641</td>
      <td>Attempts - SOUND_OF_JUSTICE_ATTEMPT_COUNT</td>
      <td>number</td>
      <td>Number of times you fought the Sound of Justice. <br></td>
    </tr>
    <tr>
      <td>1642</td>
      <td>Finished the Annoying Dog race - FINISHED_ANNOYING_DOG_RACE</td>
      <td>bool</td>
      <td>Finished the climbing race against the Annoying Dog. <br></td>
    </tr>
    <tr>
      <td>1643</td>
      <td>Entry count - ENTERED_NOELLE_KITCHEN_COUNT</td>
      <td>number</td>
      <td>Number of times you entered Noelle's kitchen while being in the vent. Maximum 3. <br></td>
    </tr>
    <tr>
      <td>1644</td>
      <td>Took the Shadow Crystal at the cliff - TOOK_SHADOW_CRYSTAL_IN_CLIFF</td>
      <td>bool</td>
      <td>Whether there is a Shadow Crystal to grab in the left cliff. Also requires other save data. <br></td>
    </tr>
    <tr>
      <td>1645</td>
      <td>Unlocked the Mike Zone door - UNLOCKED_MIKE_ZONE_DOOR</td>
      <td>bool</td>
      <td>Unlocked the Mike zone door using the 6453 combination. <br></td>
    </tr>
    <tr>
      <td>1646</td>
      <td>Got the Shadow Crystal - OBTAINED_SHADOW_CRYSTAL_CH1</td>
      <td>bool</td>
      <td>Obtained the Shadow Crystal from Jevil in chapter 1. <br></td>
    </tr>
    <tr>
      <td>1647</td>
      <td>Got the Shadow Crystal - OBTAINED_SHADOW_CRYSTAL_CH2</td>
      <td>bool</td>
      <td>Obtained the Shadow Crystal from Spamton NEO in chapter 2. <br></td>
    </tr>
    <tr>
      <td>1648</td>
      <td>Got the Shadow Crystal - OBTAINED_SHADOW_CRYSTAL_CH3</td>
      <td>bool</td>
      <td>Obtained the Shadow Crystal from the Knight in chapter 3. <br></td>
    </tr>
    <tr>
      <td>1649</td>
      <td>Got the Shadow Crystal - OBTAINED_SHADOW_CRYSTAL_CH4</td>
      <td>bool</td>
      <td>Obtained the Shadow Crystal from Gerson in chapter 4. <br></td>
    </tr>
    <tr>
      <td>1650</td>
      <td>Talked Cupstack Finalclimb - TALKED_TO_CUP_STACK_DURING_FINAL_CLIMB</td>
      <td>bool</td>
      <td>Talked to the cup stack in the fragile tower room. <br></td>
    </tr>
    <tr>
      <td>1651</td>
      <td>Song line - TEMMIE_SONG_LINE</td>
      <td>map</td>
      <td>Tracks the current line of Temmie singing Don't forget in Alphys' classroom. <br>0 = When the light is running low<br>1 = And the shadows start to grow<br>2 = And the places that you know<br>3 = Seem like fantasy<br></td>
    </tr>
    <tr>
      <td>1652</td>
      <td>Talked to Gerson after the battle - TALKED_TO_GERSON_AFTER_BATTLE</td>
      <td>bool</td>
      <td>Talked to Gerson in his study after defeating him and before saying goodbye to him. <br></td>
    </tr>
    <tr>
      <td>1654</td>
      <td>Interacted with Chairiel with Susie - INTERACTED_WITH_CHAIRIEL_SUSIE</td>
      <td>bool</td>
      <td>Interacted with Chairiel in front of Susie. <br></td>
    </tr>
    <tr>
      <td>1655</td>
      <td>First juice - FIRST_ADDED_JUICE</td>
      <td>bool</td>
      <td>Added juice to your glass at least once at church. <br></td>
    </tr>
    <tr>
      <td>1656</td>
      <td>Weird Route Fail - WEIRD_ROUTE_FAIL_CH4</td>
      <td>bool</td>
      <td>Aborted the Weird Route during chapter 4. Unaccessed as of chapter 4. <br></td>
    </tr>
    <tr>
      <td>1657</td>
      <td>Talked Rudy Church Weird - TALKED_TO_RUDY_AT_CHURCH_WEIRD_ROUTE</td>
      <td>bool</td>
      <td>Talked to Rudy at church during the Weird Route. <br></td>
    </tr>
    <tr>
      <td>1658</td>
      <td>Portal unlocked - MIKE_PORTAL_UNLOCKED</td>
      <td>bool</td>
      <td>Unlocked the way back to Castle Town by finishing chapter 4 and returning to the Third Sanctuary. <br></td>
    </tr>
    <tr>
      <td>1659</td>
      <td>Cutscene - MIKE_PORTAL_CUTSCENE</td>
      <td>bool</td>
      <td>Viewed the cutscene of the pillar of light in the Third Sanctuary. <br></td>
    </tr>
    <tr>
      <td>1660</td>
      <td>Return choice - MIKE_PORTAL_RETURN_CHOICE</td>
      <td>bool</td>
      <td>Chose or not to return to Castle Town after getting to the pillar of light for the first time. <br></td>
    </tr>
    <tr>
      <td>1661</td>
      <td>Trips - MIKE_PORTAL_TRIP_COUNT</td>
      <td>number</td>
      <td>How many times Kris went into the pillar of light to come back to Castle Town. <br></td>
    </tr>
    <tr>
      <td>1663</td>
      <td>Used the microphone crystal - INTERACTED_WITH_MICROPHONE_CRYSTAL</td>
      <td>bool</td>
      <td>Interacted with the microphone crystal in the Mike zone. <br></td>
    </tr>
    <tr>
      <td>1664</td>
      <td>Used the save point in Kris's room - CHECKED_KRIS_ROOM_SAVE_POINT</td>
      <td>bool</td>
      <td>Interacted with the save point in Kris's room. <br></td>
    </tr>
    <tr>
      <td>1665</td>
      <td>Checked Rudy's flowers - INTERACTED_WITH_RUDY_FLOWERS_CH4</td>
      <td>bool</td>
      <td>Interacted with the flowers in Rudy's hospital room in chapter 4. <br></td>
    </tr>
    <tr>
      <td>1666</td>
      <td>It's TV Time! Hiscore - TV_TIME_HISCORE</td>
      <td>number</td>
      <td>Score on the It's TV Time! rhythm game <br></td>
    </tr>
    <tr>
      <td>1667</td>
      <td>It's TV Time! Hard Hiscore - TV_TIME_HARD_HISCORE</td>
      <td>number</td>
      <td>Score on the It's TV Time! rhythm game, Hard Mode <br></td>
    </tr>
    <tr>
      <td>1668</td>
      <td>Knock You Down!! Hiscore - KNOCK_YOU_DOWN_HISCORE</td>
      <td>number</td>
      <td>Score on the Knock You Down!! rhythm game <br></td>
    </tr>
    <tr>
      <td>1669</td>
      <td>Knock You Down!! Hard Hiscore - KNOCK_YOU_DOWN_HARD_HISCORE</td>
      <td>number</td>
      <td>Score on the Knock You Down!! rhythm game, Hard Mode <br></td>
    </tr>
    <tr>
      <td>1688</td>
      <td>Justice Axe - JUSTICE_AXE_REWARD_STATE</td>
      <td>map</td>
      <td>Got the Justice Axe after winning against Gerson. <br>0 = Default state<br>1 = Got the axe<br>2 = Won the fight with inventory full<br></td>
    </tr>
    <tr>
      <td>1689</td>
      <td>Entered with party - ENTERED_MIKE_ZONE_ACCOMPANIED</td>
      <td>bool</td>
      <td>Went past the Mike locked door with Susie and Ralsei. <br></td>
    </tr>
    <tr>
      <td>1690</td>
      <td>Pet the first Mike statue - PET_FIRST_MIKE_STATUE</td>
      <td>bool</td>
      <td>Pet the first cat-eared statue in the Mike zone. <br></td>
    </tr>
    <tr>
      <td>1691</td>
      <td>Didnt Pet First Mike Statue - DIDNT_PET_FIRST_MIKE_STATUE</td>
      <td>map</td>
      <td>Whether you chose not to pet the first statue in the Mike zone when prompted. Unaccessed as of chapter 4. <br>0 = Default state<br>2 = Chose Don't pet<br></td>
    </tr>
    <tr>
      <td>1692</td>
      <td>Saved the terrified Maus - SAVED_TERRIFIED_MAUS</td>
      <td>bool</td>
      <td>Viewed the cutscene of the MAUS turning into the MOUSE. <br></td>
    </tr>
    <tr>
      <td>1693</td>
      <td>Pet the chest Mike statue - PET_CHEST_MIKE_STATUE</td>
      <td>bool</td>
      <td>Pet the tall statue in the Mike hat room which had a chest behind it. <br></td>
    </tr>
    <tr>
      <td>1694</td>
      <td>Statues - MIKE_STATUES_STATE</td>
      <td>number</td>
      <td>Tracks which statues have been pet. <br></td>
    </tr>
    <tr>
      <td>1695</td>
      <td>Started the Mike battle - STARTED_MIKE_BATTLE</td>
      <td>bool</td>
      <td>Started the battle against Mike. <br></td>
    </tr>
    <tr>
      <td>1696</td>
      <td>Saw the fake Mikes' post-battle scene - SAW_FAKE_MIKES_POST_BATTLE_SCENE</td>
      <td>bool</td>
      <td>Viewed the cutscene of the fake Mikes after defeating them. <br></td>
    </tr>
    <tr>
      <td>1697</td>
      <td>Opened the Mike exit door - OPENED_MIKE_DOOR</td>
      <td>bool</td>
      <td>Opened the volume-controlled door before the Mike battle. <br></td>
    </tr>
    <tr>
      <td>1698</td>
      <td>Battat - BATTAT_HIGH_SCORE</td>
      <td>number</td>
      <td>High score on the BATTAT minigame. <br></td>
    </tr>
    <tr>
      <td>1699</td>
      <td>Jongler - JONGLER_HIGH_SCORE</td>
      <td>number</td>
      <td>High score on the JONGLER minigame. <br></td>
    </tr>
    <tr>
      <td>1700</td>
      <td>Pluey - PLUEY_HIGH_SCORE</td>
      <td>number</td>
      <td>High score on the PLUEY minigame. <br></td>
    </tr>
    <tr>
      <td>1701</td>
      <td>Mic Sensitivity - MIC_SENSITIVITY</td>
      <td>number</td>
      <td>Flag never set, but would have been a microphone sensitivity setting. <br></td>
    </tr>
    <tr>
      <td>1702</td>
      <td>Unlocked - UNLOCKED_MIKE_MINIGAMES</td>
      <td>bool</td>
      <td>Unlocked the Mike minigames room after the Mike battle. <br></td>
    </tr>
    <tr>
      <td>1703</td>
      <td>Got the Mike hat-room chest - OBTAINED_TV_ZONE_3_CHEST</td>
      <td>bool</td>
      <td>Got the TV Dinner from the chest in the Mike hat room. <br></td>
    </tr>
    <tr>
      <td>1704</td>
      <td>Escape abort - KRIS_NOELLE_ESCAPE_WEIRD_ABORT</td>
      <td>map</td>
      <td>Failed to enter Kris's body in time during the Weird Route cutscene and let them escape with Noelle. <br>0 = Default state<br>1 = Let Kris and Noelle escape<br>2 = Got put back in closet<br></td>
    </tr>
    <tr>
      <td>1747</td>
      <td>Talked with Toriel last night - TALKED_TORIEL_LAST_NIGHT</td>
      <td>map</td>
      <td>Talked with Toriel about her behavior night before Festival. <br>0 = Default state<br>1 = We were locked out<br>2 = You were way too loud<br></td>
    </tr>
    <tr>
      <td>1780</td>
      <td>Balthizard - BALTHIZARD_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Balthizard encounter at the start of the First Sanctuary. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1781</td>
      <td>Balthizard - BALTHIZARD_OLDMAN_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Balthizard encounter at the start of the First Sanctuary when coming back with Gerson. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1782</td>
      <td>Guei - SECOND_GUEI_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Guei encounter when Gerson turns the lights back on in the dark maze room. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1783</td>
      <td>Mizzle - FIRST_MIZZLE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Mizzle encounter in the room to the right of Gerson's study. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1784</td>
      <td>Winglade - WINGLADE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Winglade encounter at the start of the Second Sanctuary. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1785</td>
      <td>Organikk - SECOND_ORGANIKK_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Organikk encounter in the Second Sanctuary's library connector room. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1786</td>
      <td>Organikk - FIRST_ORGANIKK_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Organikk encounter in the Second Sanctuary's worship room. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1787</td>
      <td>Winglade + Organikk - STEEL_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Winglade/Organikk encounter in the Second Sanctuary's money fountain room. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1788</td>
      <td>Wicabel - FIRST_WICABEL_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Wicabel encounter in the Second Sanctuary's bell room. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1789</td>
      <td>Wicabel + Organikk - FIRST_CACOPHONY_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Wicabel/Organikk encounter in the Second Sanctuary's gallery. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1790</td>
      <td>Wicabel + Organikk - SECOND_CACOPHONY_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Wicabel/Organikk encounter in the Second Sanctuary's room to the right of Gerson's study. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1791</td>
      <td>Bibliox + Winglade - FLAPPING_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Bibliox/Winglade encounter in the Third Sanctuary's bookshelf maze room. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1792</td>
      <td>2 Organikks + Wicabel - THIRD_CACOPHONY_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Organikk/Organikk/Wicabel encounter in the Third Sanctuary's dark maze room. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1793</td>
      <td>Balthizard + Mizzle + Guei - ELEMENTS_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Balthizard/Mizzle/Guei encounter in the Third Sanctuary's angel prophecy room. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1794</td>
      <td>Wicabel - SECOND_WICABEL_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Wicabel encounter in the Third Sanctuary's golden piano room. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1795</td>
      <td>Guei - FIRST_GUEI_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Guei encounter at the start of the First Sanctuary. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1796</td>
      <td>Bibliox - BIBLIOX_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Bibliox encounter in the library. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1797</td>
      <td>Guei + Balthizard - SCENTED_CANDLES_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Guei/Balthizard encounter if you touch a roaming flame in the library. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1798</td>
      <td>Miss Mizzle - SECOND_MIZZLE_ENCOUNTER_OUTCOME</td>
      <td>map</td>
      <td>Tracks the state of the Mizzle encounter in the watercooler room. <br>0 = Default state<br>1 = Violenced (includes SnowGrave)<br>2 = Spared<br>3 = Pacified<br>4 = In combat (Ch. 1)<br>5 = Violenced by uncontrolled Susie (unused in demo due to a bug)<br>6 = Frozen<br></td>
    </tr>
    <tr>
      <td>1846</td>
      <td>Pink progress - PINK_PROGRESS</td>
      <td>map</td>
      <td>Progress through the Pink encounter and hideout sequence. <br>0 = Door closed<br>1 = Door opened<br>1.5 = Save point before the boss<br>2 = Defeated boss<br>3 = Entered hideout<br>4 = Cutscene starts after buying 3 items in hideout<br>5 = Cutscene ends<br></td>
    </tr>
    <tr>
      <td>1904</td>
      <td>Platform mode jump count - PLATMODE_JUMP_COUNT</td>
      <td>number</td>
      <td>Kris's jump count in platform mode. <br></td>
    </tr>
    <tr>
      <td>1905</td>
      <td>Platform mode swing count - PLATMODE_SWING_COUNT</td>
      <td>number</td>
      <td>Kris's swing count in platform mode. <br></td>
    </tr>
    <tr>
      <td>1908</td>
      <td>Defeated Pink - DEFEATED_PINK</td>
      <td>bool</td>
      <td>Whether you defeated Pink. <br></td>
    </tr>
  </tbody>
</table>
</details>