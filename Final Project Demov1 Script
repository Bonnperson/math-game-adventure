# Note: This is the Final Project Demo Script.


# The script of the game goes in this file.

# Declare characters used by this game. The color argument colorizes the
# name of the character.

define maria = Character('maria', color="#E03B8B")

label start:
"The 7 Days War is over. Much of the outskirts lay in Anarchy."
"Here in the H.S.S are the few remaining pillars of Order."
"You are a veteran. Your benefactor have given you the privilege to a stable life."
"We have Won."

label sprites:
show maria smile
"Maria" "Comrade Inspector, I give you warm welcome to the H.S.S. Crossing 141."
show maria talking
"Maria" "My name is Maria. I will be working alongside you."
show maria smile
"Maria" "Remember that you are on the forefront of protecting humanities last fortresses."

label background:
scene bg inside the office

"Maria" "As your secretary I will guide you, but I do hope you'll get the rope."
"Maria" "For I have my own business to tend to."
label bgm:
play music "bgm_ceilinglight.mp3" fadein 1.0 volume 0.5
"Maria" "..."
"Maria" "Lets get down to the basics."
"*She hand you a fake passport.*"

"The passport reads: \"Birthday 11/26/1936 - Date of Citizenship: 12/10/1962 - Ring Scan: Current Age: 21 - X-Ray Scan: Gender: Male - Silicon Scan: 0 Percent Concentration - Gene Purity: 100 Percent.\" "
"Maria" "Do you see something wrong with this passport?"

label choices:
    default learned = False
menu:
    "Yes":
        jump choices1_a
    "No":
        jump choices1_b

label choices1_a:
    "Maria" "Good."
    $ learned = True
    jump choices1_common

label choices1_b:
    "Maria" "Check again, look at the years."
    jump choices1_common

label choices1_common:
    "Maria" "Tell me what's wrong. This is a important element of the vertification process."
menu:
    "He'll have to be 21":
        jump choices1_c
    "He'll have to be 62":
        jump choices1_d

label choices1_c:
    "Maria" "Exactly, this person's age does not match with their Birthday and Citizenship dates. In order for him to be alive he would've needed to live a extra 5 years. Therefore, we can assume this passport is a black market one."
    $ learned = True
    jump choices2_common

label choices1_d:
    "Maria" "Wrong, 21 is the correct age. The Birthday and Citizenship dates don't line up with the person's age. Their age should be 26 not 21."
    jump choices2_common

label choices2_common:
"Maria" "Well that all the time I have now Inspector." 
stop music fadeout 1.0
scene bg inside the office alone
play music "bgm_main menu.mp3" fadein 1.0 volume 0.5

"Maria" "Thank you for playing the Final Project Demo."
