# Runelite Chat Filter
An updated regex for the RuneLite chat filter, no more annoying spam at the GE!

# Never Manually Update Your Filter!
Don't want to copy an paste the filter everytime you want to update it?
Just install the Chat Filter Updater plugin on RuneLite! Details in the How to Install section.

## How to Install
### Automatic Install
Install the 'Chat Filter Updater' plugin in RuneLite.
In RuneLite click the wrench in the top right corner > Click the Gold plug > search for 'Chat Filter Updater' > Click install

### Manual Install
Just paste the whole filter into your RuneLite settings: Chat filter -> Filtered Regex
For the best results put Filter Type on Remove messages, so you don't see them at all!

## Troubleshooting

  ### The default chat filter blocks everything
  At this time you have to disable stripping accents in RuneLite's Chat Filter Plugins. 
  RuneLite's Chat Filter Plugin strips the regex from both chat and it's regex. Causing the blocked accented vowels to block all vowels.
  Blocking accented characters is extremely powerful for catching bot text, as it's used almost exclusively by them. Of course, there's the downside of possibly blocking other languages. So this is subject to change.

## Help everyone reduce spam
The regex list needs constant updates as bots change their spam. You can help by submitting additions to the regex list.

If you'd like to submit an addition follow these steps.

    1. Create a New Issue: Click on the "Issues" tab at the top of the repository and then click the green "New Issue" button.

    2. Issue Title: Use a descriptive and concise title for your regex addition.

    3. Description (Optional): Include any relevant information about its purpose and usage. If your title is sufficient this isn't necessary.

    4. Regex Pattern: In the issue description, provide the regex pattern you would like to suggest.

    5. Test Cases (Optional): If possible, provide one or more test cases that demonstrate the effectiveness of your regex pattern.
    This helps ensure it accurately matches the intended strings and avoids false positives/negatives.

    6. Label: Apply the "Regex Addition" label from the right-hand side labels section to categorize your issue properly.

    7. Click Submit new issue.



## Submission Example:

#### Title: 
    Remove 'Doubling Money' Messages.
#### Description:
    Removes doubling money scam at ge.
    
    Pattern:
    ^(?!.*doubling\s+money).*$

    Test case 1:
    Input: "Doubling money!! PM me!"
    Output: Match
    
    Test case 2:
    Input: "I have to figure out how to double my money"
    Output: No Match 
#### Label: 
    Regex Addition

