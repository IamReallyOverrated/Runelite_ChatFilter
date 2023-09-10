# Runelite Chat Filter
An updated regex for the RuneLite chat filter, no more annoying spam at the GE!

Just paste the whole filter into your Runelite settings: Chat filter -> Filtered Regex
For the best results put Filter Type on Remove messages, so you don't see them at all!


If you'd like to submit an addition to the list please follow these guidelines.

    Check Existing Issues: Before submitting a new regex addition, please check the existing issues to 
    see if a similar pattern has already been suggested or accepted.

    Create a New Issue: Click on the "Issues" tab at the top of the repository and then click the green "New Issue" button.

    Issue Title: Use a descriptive and concise title for your regex addition.

    Description (Optional): Include any relevant information about its purpose and usage. If your title is sufficient this isn't necessary.

    Regex Pattern: In the issue description, provide the regex pattern you would like to suggest.

    Test Cases (Optional): If possible, provide one or more test cases that demonstrate the effectiveness of your regex pattern.
    This helps ensure it accurately matches the intended strings and avoids false positives/negatives. If you're addition is
    too large to provide every test case, provide a few.

    Label: Apply the "Regex Addition" label from the right-hand side labels section to categorize your issue properly.

Submission Example:

    Title : 
    Remove 'Doubling Money' Messages.

    Description:
        Removes doubling money scam at ge.
        
        Pattern:
        ^(?!.*doubling\s+money).*$
    
        Test case 1:
        Input: "Doubling money!! PM me!"
        Output: Match
        
        Test case 2:
        Input: "I have to figure out how to double my money"
        Output: No Match
    
    Label: 
    Regex Addition

