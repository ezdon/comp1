#Task sheet 1 questions

##Task 3a questions
1. GetPlayerName()
2. Create a while loop so if the name is invalid the user will be prompted to enter their name again. If the name is valid, it will be returned out the function
3. A variable that continues/ends the while loop, most likely 'valid'. It's data type is boolean. 
Pseudo code for improvements:

FUNCTION GetPlayerName()
	valid: Boolean
	PlayerName: String
	valid <- FALSE
	WHILE valid = FALSE DO
		PlayerName <- INPUT "Please enter your name"
		IF PlayerName = '' THEN
			OUTPUT "You must enter something for your name!"
			valid <- FALSE
		ELSE
			valid <- TRUE
		END IF
	END WHILE	
END FUNCTION

##Task 3b questions
1. UpdateRecentScores()
##Task 5 questions
1. import datetime
2. UpdateRecentScores()
	DisplayRecentScores()
	ResetRecentScores()
	TRecentScore()
3. By using the strptime() function	

Task Sheet 2 Questions
1. PlayGame
2. DisplayMenu()
3. GetRank()	

Task Sheet 2 PsuedoCode

FUNCTION DisplayOptions()
	OUTPUT "Options Menu"
	OUTPUT ""
	OUTPUT "1. Set Ace to HIGH or LOW"
	OUTPUT "2. Card of same score ends game"
	OUTPUT ""
END FUNCTION

FUNCTION GetOptionChoice()
	OptionChoice: String
	OptionChoice <- INPUT "Select an option from the menu"
	RETURN OptionChoice
END FUNCTION	
	
FUNCTION SetOptions(OptionChoice: String)
	valid: Boolean
	valid <- FALSE
	WHILE valid = FALSE DO
		IF OptionChoice = '1' THEN
			RETURN OptionChoice
			valid = TRUE
		ELSE IF OptionChoice = '2' THEN
			RETURN OptionChoice
			valid = TRUE
		ELSE IF OptionChoice = 'q' THEN
			valid = TRUE
		ELSE
			valid = FALSE
			OUTPUT "Not Valid"
			CALL GetOptionChoice()
		END IF	
	END WHILE
END FUNCTION	

FUNCTION SetAceHighOrLow()
	Valid: Boolean
	AceRank: String
	selection: String
	Valid <- FALSE
	WHILE Valid = FALSE DO
		OUTPUT""
		selection <- INPUT "would you like the ace to be high or low?"
		IF selection = 'h' THEN
			AceRank = 'h'
			Valid = TRUE
		ELSE IF selection = 'l' THEN
			AceRank = 'l'
			Valid = TRUE
		END IF
	END WHILE
	OUTPUT ""
	OUTPUT "----Ace Set!----"
	RETURN AceRank
END FUNCTION	
			
		